# csPortfolio

* Webpage [here](https://ryggj.github.io/testWeb/dogPage/dogPage/) Repository [here](https://github.com/RyggJ/testWeb)
<br><br>It was tough for me to pick up on a new language so different from Java, but it was much easier to pick up on than Java.
---
* Lightning [here](https://ryggj.github.io/lightning2/) Repository [here](https://github.com/RyggJ/lightning2)
<br><br>I thought it was cool how the while loop drew a bunch of lines rather than just one jagged line, and felt that my biggest achievement here was getting the color of lightning to change based on where the mouse was.
---
* Lightning JS [here](https://ryggj.github.io/lightning2/lightningP5js/index.html) Repository [here](https://github.com/RyggJ/lightning2)
<br><br>This was my first time taking a look at Javascript, and I was not a very big fan of it at first. It seems too vague to do much good, but after learning more and looking at more coding I can see how much potential it really has.
---
* Dice [here](https://ryggj.github.io/dice3/) Repository [here](https://github.com/RyggJ/dice3)
<br><br>I remember tinkering around a lot with this one trying to decide what a winning roll would sum up to, and it was when I began to pick colors that were easy on the eyes ft. sky blue background.
---
* Chemotaxis JS [here](https://ryggj.github.io/chemotaxis4/ChemoJS/) Repository [here](https://github.com/RyggJ/chemotaxis4)
<br><br>I had a difficult time getting this one to both be able to run alone and last long enough to make it past one go but not so long it would take hours to finish.
---
* Starfield [here](https://ryggj.github.io/starfield5/) Repository [here](https://github.com/RyggJ/starfield5)
<br><br>I thought it was cool to see how you could use sine and cosine in computer science to help with circular motion.
---
* Minesweeper [here](https://ryggj.github.io/Minesweeper/) Repository [here](https://github.com/RyggJ/minesweeper)
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
