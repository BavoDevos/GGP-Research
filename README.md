# GGP-Research : Snake neural net using genetic algorithms 
in this readme file i will quickly go over the basics of what my project is, explain quickly what neural networks are and the advantages and disadvantages. I will then talk about my journey throughout this project and finally conclude it with a conclusion where i go over my personal conclusion, my future with neural networks and the future of neural networks in general.


# About this project
This project was made using a in-house framework developed by my professors at DAE, using this framework i made a version of the snake game and added a neural network to it that plays the game, can this neural network learn to play ?

# What is a neural network
A neural network is a type of algorithm made to simulate the structure and function of human brains. It consists of layers of interconected neurons which are organized in a way so that the network can learn and make decisions based on any input given.The neurons of a neural network are usually divided into 3 types of layers, we have the inputlayer which takes in raw data, the outputlayer produces the final results. In between these layers there are one or more hiddenlayers whcih process the data.


![A simple visual representation of a neural network](https://www.investopedia.com/thmb/5-hnhHpOzLM2GVXPlSstg8tJYLw=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/dotdash_Final_Neural_Network_Apr_2020-01-5f4088dfda4c49d99a4d927c9a3a5ba0.jpg)

# Advantages And Disadvantages of a neural network

Advantages :
- Ability to learn from data : Neural networks are able to learn from input-output pairs which allow them to improve performance over time. This is especially useful for taks where the desired result is not know or where relation from input to output is complex
- Ability to generalize : Neural networks are well known to generalize from the examples they were trained on which allow them to be used in a wide range of applications.
- Versatile : Neural networks are versatile, they can be used for a lot of problems we face.

Disadvantages : 
- Complexity : Neural networks are a complex system with many adjustable parameters which make them difficult to design and especially optimize.
- Training required : unlike what i would call a "hardcoded ai" the neural network needs to train and can sometimes fail to train effectively.
- Blackbox models : As stated before neural networks are complex which also makes it hard to understand how they process the data and produce the outputs they produce, it is not a very transparant model.
- Overfitting : Neural networks have the tendancy to overfit to training meaning they perform well on training data but perform very poorly on new unseeen data.

# My journey

**The beginning**

I started this project with no prior knowledge of neural networks, I had no idea how they worked and as such had to begin learning. I began my research by watching multiple videos on the topic and reading as many articles and papers as i could. It immediately made me extremely interested in the concept of a neural network. It took me a while to fully understand how they really work but once i did i could begin on the next part.

**Making the snake game**

I now was faced with the next challenge which was making the game itself. It had to be efficient so it could run a whole lot of games of snake without completely setting my laptop on fire. For this task i used the framework we had been using in our classes. With some struggle i was able to put together a simple version of the game with graphics.

![A gif of the framework rendering 2000's snake games at once](https://media.giphy.com/media/Rr3g42qTgppumRrBYo/giphy.gif)

**The neural network**

Now that i had a working game i had to move onto the actual neural network, i decided to use 13 inputs with 2 hidden layers both 20 large and 4 outputs. I had the following inputs and outputs :

inputs:

- distance to the food on the left
- distance to the food on the right
- distance to food upwards
- distance to food downwards
- distance to wall left
- distance to wall right
- distance to wall upwards
- distance to wall downwards
- distance to closest bodypart on left
- distance to closest bodypart on right
- distance to closest bodypard upwards
- distance to closest bodypart downwards
- direction the snake is moving

outputs:

- move up
- move right
- move down
- move left

My neural network used genetic algorithms to learn, i applied this by calculating a "fitness score" which means i awarded the snake for living and eating and penalised it for dying by going into a wall or its own body. I also made it so the snake could only move a handfull of moves without eating before dying, kind of like starving. This then would estimate which model was the best i would take the best and the second best one and mutate them by adjusting the weights slightly. Outside this i also had a group which would be completely random as to prevent my model from becoming to genitcally the same.

**my results**
Now i had finished my neural network and it was time to see how it performed.

![my neural network in action](https://media.giphy.com/media/ktK8tlFp84YQozw9TU/giphy.gif)

My neural network did not perform as good as i had expected or hoped it would but that was also to be expected from my very first attempt. The snake would learn the very basics fast it would avoid the first wall maybe the second but thats as far as it ever evolved. It was clear i had some mistakes along the way which we are seeing only now.

# conclusion and future

**personal conclusion**

I was obviously not very happy with my end results but this has shown me a lot of things i would have never learned. Personally if i was given the task to make an ai for snake i would not do it with a neural network, i would perfer making a AI which follows hamiltonian paths and cuts it off where it can. If i had to do it with neural networks i would completely rewrite my mutation functions as i think my model fails there. A more genetically varried pool would prevent my model from getting stuck as it does now. I would also change the inputs i give.

**personal future**

This has been an extremely informative research and it has made me very interested in neural networks. Personally i will be looking more into neural networks and i will continue making my own neural networks. Infact i want to remake this project with the knowledge i have gained and hopefully make a model which will perform much better than this one does now. I also want to see where else i can apply neural networks and if they can be used to solve problems i would otherwise tackle in a completely different way.

**Future of neural networks**

Neural networks is a rapidly evolving technology that will more than likely see itself wiggle into the gaming industry in both good and bad ways. Soon we might see neural networks doing real-time decision making which would allow for more sophisticated and dynamic NPCs. However we will also see new ways of "botting" in games, a good example of this already is the "Nexto" bot which is a neural network that has taken the fanbase of the game by storm, this neural network has landed itself in the top 10% of players. The neural network has the same amount of neurons as real life gecko's. This is an obvious issue which competitive games will be facing now.

