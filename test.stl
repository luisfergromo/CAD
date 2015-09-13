Sfd=30;

module Cuadrado(){
    difference(){
      cube([7,7,2]);
        
    }
   }
module circulo(){ 
cylinder (r=10,h=2);
 }
module cilindroExterno(){
       cylinder(r=5,h=2);
     }
  
//rotate(a=45,v=[0,0,0]){
//    translate([0,0,0]) Cuadrado();}
module Circulito(){ 
difference(){
    circulo([0,0,0]); 
    cilindroExterno([0,0,0]);
    }
}
module linterna(){
Circulito();
Cuadrado();
translate([-7,-7,0]){
    Cuadrado();}
}
module test(){
translate([10,10,0]){
linterna();
translate([-10,-10,0]){cilindroExterno();}
translate([-20,-20,0]) {Circulito();}
translate([-20,-20,0]) {linterna();}
    }
}
test();
rotate([0,0,90]){
    test();}
