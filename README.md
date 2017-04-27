# classes
//class declaration
class Rectangle{
  constructor(heigth,width){
    this.heigth=heigth;
    this.width=width;}
}

//class expression
//unnamed
var Rectangle= class{
constructor(heigth,width){
    this.heigth=heigth;
    this.width=width;};
}

//named
var Rectangle= class Rectangle{
  constructor(heigth,width){
    this.heigth=heigth;
    this.width=width;
  }}
  
  //both class declatation and expression can't be hoisted
  
  var obj = {
  log: ['test'],
  get latest() {
    if (this.log.length == 0) return undefined;
    return this.log[this.log.length - 1];
  }
}
console.log(obj.latest); // Will return "test".

var obj={
  word:['something'],
  
  get theLatest(){}
    if(this.word.length==0) return undefined;
    return this.word[this.word.length-1];
  }
  }
