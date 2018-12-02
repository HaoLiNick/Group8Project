# 2048 Final Project_Group:eight:  
## Who are We :couple::two_men_holding_hands:
---
|Name|UNI|Section|
|---|---|---|
|Fanpei Liu|fl2486|Sec002|
|Hao Li|hl3205|Sec002|
|Yaojun Qin|yq2249|Sec002|
|Yanghuizi Zhao|yz3458|Sec002|
## Introduction 
<br>2048 is popular single-player sliding block puzzle game created by Italian web developer Gabriele Cirulli. It is available online and on our phone. The team used Python to write our own 2048. The game’s objective is to slide numbered tiles on a grid to combine them to create a tile with the number 2048.</br>

## What it looks like :outbox_tray:
![Alt Text](https://raw.githubusercontent.com/HaoLiNick/Group8Project/master/GAMING.png)

## How to play it! :video_game:
Type a/d/w/s as :arrow_left::arrow_right::arrow_up::arrow_down: and enter in the box to play the game. It will print "You Win!" when you reach the number 2048, "You lost!" when you run out of space and cannot merge anymore. Keep typeing a/d/w/s until lost! 
![Alt Text](https://raw.githubusercontent.com/HaoLiNick/Group8Project/master/YOU_LOSE.png)

## Explanation :memo:
<br> 
1. `from random import * ` When you `from random import *`, all the definitions from random become part of the     current name space. This means you don't have to prefix anything with random. The team only need this         package to finish the project.

2. an `init_matrix()` method that will initialize a 4*4 Matrix.

3. a `pop2(matrix)`/ `def pop4(matrix)` method that will pop number 2 and 4 corresponding.
 
4. a `decide2or4(matrix)` method will determines if the new pop number is 2 or 4, then display on the matrix.

5. a `display(v)` method will display as matrix, like the second output. 
   ![Alt Text](https://raw.githubusercontent.com/HaoLiNick/Group8Project/master/Display.png)

6. a `game_results_before_next(matrix)` method will determines the current status is win/lose/TBD before the      next move. Win:reach the number 2048. TBD:1st case(There is still a zero in Matrix) 2nd case(There are two    number have the same number next to each other) Lost:Otherwise

7. a `align(vList, direction)` method will align row numbers that are non-zero, remove 0s from the row then      replace those 0s in the right or left ex:direction==left, [0,4,0,2] become [4,2,0,0].

8. a `merge(vList,direction)` method will find the same number check if they are next each other. If they do,    double one of them the number and make another one equal to zero. ex:direction==left, [2,2,2,2] become        [4,4,0,0].

9. a `handle(vList,direction)` method will run the align and merge function as cycle until the merge function    return False.

10. a `operation(matrix)` method will sign a/d/w/s to left/right/up/down corresponding, base on the moving         direction recalculate the matrix value.

11. a `main()` method will display the game. It will print "You Win!" when you reach the number 2048, "You         Lost!" when you run out of space and cannot merge anymore.

12. `if __name__== "__main__":`
    `main()` Using this code to start the game and you can begin to play.
</br>