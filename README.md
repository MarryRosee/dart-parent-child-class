# dart-parent-child-class
dart-parent-child-class





void main() {
  
  print("train infoooo000000000000000");
  
  var v1=Train("train","blue",["1134pk"],{'price':'60000'},{500});
  
   print("bike infoooo0000000000000000");
  
   var v2=Bike("bike","green",modelnumber:[5,33],price:{'name':'bike'},speed:{1,3,5});

  var v3=Animal();//i am parent i am calling myself
  
  var v4=Cat();//i am child i am calling myself and parent
  
   var v5=Cat.c1();//i am child i am calling myself and parent
  
  var v6=Sparrow("sparrow");
  

  
}
class Vechicle
{
  
  
}


class Train extends Vechicle
{
  late String name;
  late String color;
  late List modelnumber;
  late Map price;
  late Set speed;
  
  Train(String name,String color,List modelnumber,Map price,Set speed)
  {
    this.name=name;
    this.color=color;
    this.modelnumber=modelnumber;
    this.price=price;
    this.speed=speed;
    
   
    print("vechiclename:$name  ");
    print("vechiclecolor:$color");
    
    for(var item in modelnumber){
      
      
      print("vechiclemodel $item");
    }
    
    
    
      for(var item in price.values){
      
      
      print("vechicleprice $item");
    }
    
    
      for(var item in speed){
      
      
      print("vechiclespeed $item");
    }
    
    
    
  }
  
  
}

class Bike extends Vechicle
{
  
  
  
   Bike(String name,String color,{List? modelnumber,Map? price,Set? speed})
  {
   print("$name $color $modelnumber $price $speed");
     
     
     
     
     
  
}
}

class Autoraksha extends Vechicle
{
  
 
  
}

class Animal
  
{
  Animal()
  {
    
    print("i am parent class");
    
  }
  
 
  
}


class Cat extends Animal
{
  Cat(){
    
    
     print("i am cat child class");
  }
  
   Cat.c1(){
    
    
     print("i am cat 1 child class");
  }
  
}



class Sparrow extends Animal{
  
  Sparrow(String name){
     print("i am sparrow child class");
    
  }
  
  
  
}













