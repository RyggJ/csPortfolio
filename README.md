# csPortfolio

* Webpage [dogs](https://ryggj.github.io/testWeb/dogPage/dogPage/) Repository [full of pics](https://github.com/RyggJ/testWeb)
<br><br>It was tough for me to pick up on a new language so different from Java, but it was much easier to pick up on than Java.
---
* Lightning [not thunder](https://ryggj.github.io/lightning2/) Repository [includes p5.js](https://github.com/RyggJ/lightning2)
<br><br>I thought it was cool how the while loop drew a bunch of lines rather than just one jagged line, and felt that my biggest achievement here was getting the color of lightning to change based on where the mouse was.
---
* Lightning JS [still not thunder](https://ryggj.github.io/lightning2/lightningP5js/index.html) Repository [same as Java](https://github.com/RyggJ/lightning2)
<br><br>This was my first time taking a look at Javascript, and I was not a very big fan of it at first. It seems too vague to do much good, but after learning more and looking at more coding I can see how much potential it really has.
---
* Dice [game](https://ryggj.github.io/dice3/) Repository [kinda messy](https://github.com/RyggJ/dice3)
<br><br>I remember tinkering around a lot with this one trying to decide what a winning roll would sum up to, and it was when I began to pick colors that were easy on the eyes ft. sky blue background.
---
* Chemotaxis JS [spooky](https://ryggj.github.io/chemotaxis4/ChemoJS/) Repository [originally in Java](https://github.com/RyggJ/chemotaxis4)
<br><br>I had a difficult time getting this one to both be able to run alone and last long enough to make it past one go but not so long it would take hours to finish.
---
* Starfield [uses trig](https://ryggj.github.io/starfield5/) Repository [with sneak peak of another project](https://github.com/RyggJ/starfield5)
<br><br>I thought it was cool to see how you could use sine and cosine in computer science to help with circular motion.
---
* RGB Color Picker [in beta](https://ryggj.github.io/RGBcolorPicker/) Repository [isn't colorful](https://github.com/RyggJ/RGBcolorPicker)
<br><br>This was a project I started to figure out how to make the visuals behind a color picker. To my surprise, it was a lot simpler than I thought, just a bunch of squares drawn by a nested for loop.
---
* Bloonbounce [is a bit buggy](https://ryggj.github.io/bloonBounce/) Repository [doesn't bounce well](https://github.com/RyggJ/bloonBounce)
<br><br>This was my first project attempting to implement formulas from Physics. I would like to continue work on this because it's a bit buggy as far as hit registration goes.
---
* Minesweeper [is fun](https://ryggj.github.io/Minesweeper/) Repository [not a bomb...](https://github.com/RyggJ/minesweeper)
<br><br>This was probably my favorite project, inspired by programmers on youtube. I enjoyed playing minesweeper, and decided to follow their footsteps by coding my own version. However, I noticed my hand would get tired after clicking on my laptop's mousepad over and over again. To fix this I added controls that implement the keyboard. This also allowed for more accurate flagging, since right-clicking was tetious and sometimes game-costing on the mousepad.
<br>

```Java
 void draw(){
  for(int i=0;i<cols;i++){
    for(int j=0;j<rows;j++){
      blocks[i][j].show();
      if(blocks[i][j].getHit()&&blocks[i][j].getBomb()){
        go=true;
      }
      if(testWin()){
        win=true;
      }
    }
  }
  select();
  if(go==true){
    gameover();
  }
  if(win==true){
    winner();
  }
  if(keyPressed&&key=='r'){
    reset();
  }
} 
```
The code above is my draw() for minesweeper. It runs through a nested for loop to check each "block" in the game. It checks for a gameover (boolean go), which is when a block is hit and contains a bomb (getHit() and getBomb() would both return true). It also checks to see if the player has won yet, by using testWin() (testWin checks to see that all of the spaces that aren't bombs have been hit, and returns true if they have been). After that it runs select() (This method is the one that deals with all keyboard inputs, and keeps track of the selected block). And finally, if go or win are true, the game will end and text will show saying whether or not the player won. Otherwise this checks to see if the player has reset the game, which will completely reset the 2D array I used to store all of the blocks. This was definitely my best project, and I still like working on it often.
