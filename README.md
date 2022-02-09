# About
PathTaker is a puzzle game inspired by [Helltaker](https://en.wikipedia.org/wiki/Helltaker), but additionally it lets you design, test and share new custom levels for free! 
# Installation
1. Download the PathTaker zip file [here](https://github.com/GreenMama/PathTaker/raw/main/PathTaker.zip)
1. Unzip PathTaker.zip file to any local folder
1. Run PathTaker.exe

![](https://github.com/GreenMama/PathTaker/blob/main/docs/Install1.png?raw=true)

# Game
## Main menu
![](https://github.com/GreenMama/PathTaker/blob/main/docs/Menu1.png?raw=true)

* **New Game**:  Start a new "classic" game from the 1st level
* **Custom Game**:  Start a new game with custom levels. The game will read level's design from "levels" folder (i.e. level1.csv, level2.csv, and so on) 
* **Continue** or **Esc** button:  return to the game play
* **Quit**:  exit the game

## Controls
* **← Left arrow** : Move the character one square left,
* **→ Right arrow** : Move the character one square right,
* **↑ Up arrow** : Move the character one square up,
* **↓ Down arrow** : Move the character one square down,
* **Esc** : open the main menu.

![](https://github.com/GreenMama/PathTaker/blob/main/docs/Controls1.png?raw=true) ![](https://github.com/GreenMama/PathTaker/blob/main/docs/Controls2.png?raw=true)
## Gameplay
Proceed through a series of puzzle stages with the end goal of reaching a demon girl. On each puzzle stage, push stones and skeleton soldiers, avoid spike traps and keep within a set moves limit.
* Each move reduces the remaining moves limit by 1
* Each stone push or skeleton push reduces the remaining moves limit by 1
* Each spike trap reduces the remaining moves limit by 2 (1 move + 1 extra)

![](https://github.com/GreenMama/PathTaker/blob/main/docs/Gameplay1.png?raw=true)

* Number of remaining **moves** is shown in the upper left corner
* **Level number** is shown in the upper right corner

# Create custom levels
* Create a CSV file in "levels" folder with name "levelX.csv"   (i.e.  level1.csv,  level2.csv, etc)
* 1-st row should contain Moves,N  (N is the number of moves at level start)
* other rows should contain comma separated list of character codes

| Char code | Description | Image |
| --- | --- | --- |
| o | Empty space or v**o**id |  |
| w | Fixed **w**all, cannot be moved |  |
| s | **S**tone, can be moved |  |
| p | S**p**ike trap |  |
| sp | S**p**ike trap + Stone |  |
| p0 | Switching S**p**ike trap, off |  |
| p1 | Switching S**p**ike trap, on |  |
| sp0 | Switching S**p**ike trap, off + Stone |  |
| sp1 | Switching S**p**ike trap, on + Stone |  |
| mr | Skeleton **m**onster |  |
| k | **K**ey |  |
| g | **G**ate |  |
| q | **Q**ueen or demon girl  |  |
| h | **H**ero  |  |


## Examples

**File name:** levels\level1.csv  

**CSV file data:**  
Moves,5    
w,p,q    
w,o,s    
h,mr,o  

**Level in the game:**

![](https://github.com/GreenMama/PathTaker/blob/main/docs/Sample1.png?raw=true)


***

**File name:** levels\level2.csv  

**CSV file data:**  
Moves,9  
w,w,q,w  
w,o,s,o  
p,s,o,o  
h,o,o,o   

**Level in the game:**

![](https://github.com/GreenMama/PathTaker/blob/main/docs/Sample2.png?raw=true)


***

**File name:** levels\level1.csv  

**CSV file data:**  
Moves,40  
o,o,o,o,o,o  
o,w,s,p,q,o  
o,sp,sp0,sp1,s,o  
o,k,p1,p0,g,o  
o,mr,mr,mr,mr,o  
h,o,o,o,o,o   

**Level in the game:**

![](https://github.com/GreenMama/PathTaker/blob/main/docs/Sample3.png?raw=true)

# Play Custom Levels
* Run the game
* Select "Custom Game" item from the main menu

# Enjoy the GAME!

