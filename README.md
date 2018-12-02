
# 2048 Final Project_Group8(Sec2)

## Introduction
<br>2048 is popular single-player sliding block puzzle game created by Italian web developer Gabriele Cirulli. It is available online and on our phone. The team used Python to write our own 2048. The game’s objective is to slide numbered tiles on a grid to combine them to create a tile with the number 2048.</br>

## What it is looks like
![Alt Text](https://raw.githubusercontent.com/HaoLiNick/Group8Project/master/run.png)

## Data Collection
<br>0.from random import * 
When you "from random import *", all the definitions from random become part of the current name space. This means you don't have to prefix anything with random.

1.an `init_matrix()` method that will initialize a 4*4 Matrix

2.a `pop2(matrix)`/ `def pop4(matrix)` method that will pop number 2 and 4 corresponding
 
3.a `decide2or4(matrix)` method will determines if the new pop number is 2 or 4, then display on the matrix

4.a `display(v)` method will display the matrix

5.a `game_results_before_next(matrix)` method will determines the current status is win/lose/TBD before the next move

6.a `align(vList, direction)` method will align row numbers that are non-zero, remove 0s from the row then replace those 0s in the right or left ex:direction==left, [0,4,0,2] become [4,2,0,0]

7.a `merge(vList,direction)` method will find the same number check if they are next each other. If they do, double one of them the number and make another one equal to zero. ex:direction== left, [2,2,2,2] become [4,4,0,0]

8.a `handle(vList,direction)` method will run the align and merge function as cycle until the merge function return False.

9.a `operation(matrix)` method will sign a/d/w/s to left/right/up/down corresponding

10.a `run()` method will display the game and you can begin to play, it will print"You Win!" when you reach the number 2048, "You lost!" when you ran out of space</br>