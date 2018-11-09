# csPortfolio

* WebPage [here](https://ryggj.github.io/testWeb/dogPage/dogPage/)
* Lightning [here](https://ryggj.github.io/lightning2/)
* Lightning JS [here](https://ryggj.github.io/lightning2/lightningP5js/index.html)
* Dice [here](https://ryggj.github.io/dice3/)
* Chemotaxis JS [here](https://ryggj.github.io/chemotaxis4/ChemoJS/)
* Starfield [here](https://ryggj.github.io/starfield5/)

```Java
  class bloon{
  int bloonX=(int)(Math.random()*800+100);
  double bloonY=Math.random()*100+450;
  double bloonV=100;
  double bloonTime=0;
  double xInc=(Math.random()*7)-3;
  int colorPick=(int)(Math.random()*5);
  int bloonR,bloonG,bloonB;
  boolean popped=false;
  void move(){
    bloonTime+=.001;
    if(bloonX>960||bloonX<0){
      xInc*=-1;
    }
    bloonX+=xInc;
    bloonY-=(bloonV*bloonTime)+(.49*bloonTime*bloonTime);
    bloonV-=9.8*bloonTime;
    if (bloonY>500){
      contact();
    }
  }
```
