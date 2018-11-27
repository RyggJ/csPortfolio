# csPortfolio

* Webpage [here](https://ryggj.github.io/testWeb/dogPage/dogPage/) Repository [here](https://github.com/RyggJ/testWeb)
<br>It was tough for me to pick up on a new language so different from Java, but it was much easier to pick up on than Java.
---
* Lightning [here](https://ryggj.github.io/lightning2/)
* Lightning JS [here](https://ryggj.github.io/lightning2/lightningP5js/index.html)
* Dice [here](https://ryggj.github.io/dice3/)
* Chemotaxis JS [here](https://ryggj.github.io/chemotaxis4/ChemoJS/)
* Starfield [here](https://ryggj.github.io/starfield5/)
* Minesweeper [here](https://ryggj.github.io/Minesweeper/)

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
