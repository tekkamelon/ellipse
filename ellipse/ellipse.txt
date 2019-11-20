void setup(){
  size(700,700);
  background(255);
  noFill();
}

void draw(){
  float r = random(0,mouseY);
  float g = random(0,mouseX);
  float b = random(0,255);
  float x = mouseX+random(-50,50);
  float y = mouseY+random(-50,50);
  float a = random(1,100);
 
  stroke(r,g,b);
  ellipse(x,y,a,a);
  
  if(mousePressed == true){
    background(255);
  }
  
  if(keyPressed == true){
    background(0);
  }
}
