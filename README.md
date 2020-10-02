# Class-and-Objects
Semana 11

Figura cuadrado1, cuadrado2;
void setup(){
  size(500,500);
  smooth();
  noStroke();
  cuadrado1 = new Figura(100,450,50,100,4);
  cuadrado2 = new Figura(300,450,50,100,4);}
void draw(){
  background(30,0,0);
  cuadrado1.move();
  cuadrado2.move();
  cuadrado1.display();
  cuadrado2.display();
  fill(random(0,255),random(0,255),random(0,255));}
class Figura{
  float z,u,a,b,velocidad;
  Figura(float xpos,float ypos,float w,float h,float sp){
    z = xpos;
    u = ypos;
    a = w;
    b = h;
    velocidad = sp;}
  void display(){
  rect(z,u,a,b);}
  void move(){
  z += random(-velocidad, velocidad);
    u += random(-velocidad, -velocidad); } }
