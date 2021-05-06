<h1 align="center">
  Snake Game - Reinforcement Learning
</h1>
<p align="center">
  A simple snake game automated using Machine Learning - Reinforcement Learning
</p>

![demo](https://raw.githubusercontent.com/Abhijith14/SnakeGame-ML/master/image.gif)

<br>
<br>


## 📕 Installation

### 🕷️ Create an environment
Whatever you prefer (e.g. `conda` or `venv`)
```console
mkdir myproject
$ cd myproject
$ python3 -m venv venv
```

### 🕷️ Activate it
Windows:
```console
venv\Scripts\activate
```
Mac / Linux:
```console
. venv/bin/activate
```
### 🕷️ Install PyTorch and dependencies

For Installation of PyTorch see [official website](https://pytorch.org/).

You also need `PyGame`, `Matplotlib`, `IPython`:
 ```console
pip install pygame, matplotlib, ipython
 ```

If you get an error for numpy, install numpy separately:
 ```console
pip install numpy
```



## 👨‍💻 Usage
Run
```console
python agent.py
```
This will start training the agent. It takes upto 80 - 100 gameplays for the model to be trained good. <br>
If you want to change the number of gameplays, edit this section in function get_action, class Agent in [agent.py](agent.py):
```console
def get_action(self, state):
    self.epsilon = {{ Enter your number of gameplays for training }} - self.n_games
```
You can find the [model file](model/model.pth) inside model folder.<br>
Also while training, you can find the training graph with the number of gameplays vs Scores
![graph](https://raw.githubusercontent.com/Abhijith14/SnakeGame-ML/master/graph.png)

## ⚙️ Customize
Have a look at [game.py](game.py). You can change the game variables according to your own use case. <br>
Change the colours of the game elements over here.
```
# rgb colors
WHITE = (255, 255, 255)
RED = (200,0,0)
BLUE1 = (0, 0, 255)
BLUE2 = (0, 100, 255)
BLACK = (0,0,0)
```
Default BLOCK_SIZE (Size of a block in the game) and SPEED (speed of snake) is set to 20.
```
BLOCK_SIZE = 20
SPEED = 20
```
In the init function of class SnakeGame; the parameters w and h are the width and height of your game window.
```
def __init__(self, w=640, h=480):
        self.w = w
        self.h = h
```
<br>


### 🛠️ Built With

* [Python 3.7](https://www.python.org/) - Creating Project


### ❤️ Authors

* **Abhijith Udayakumar** - *Design & Development* - [Abhijith14](https://github.com/Abhijith14)

<br>
<br>

## 🚨 Forking this repo (please read!)

_**yes, with attribution**_.

I value keeping my work open source, but as you all know, _**plagiarism is bad**_. It's always disheartening whenever I find that someone has copied my work without giving me credit. I spent a non-trivial amount of effort building and designing this project, and I am proud of it! All I ask of you all is to not claim this effort as your own.


### TL;DR

Yes, you can fork this repo. Please give me proper credit by linking back to [Abhijith14/SnakeGame-ML](https://github.com/Abhijith14/SnakeGame-ML). Thanks!
