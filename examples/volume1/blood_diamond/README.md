# Alice in Wonderland

di Clyde Geronimi, Wilfred Jackson, Hamilton Luske

1951 - Animazione, Avventura

http://www.imdb.com/title/tt0043274/

## Il film in breve
Le ragazzine troppo curiose fanno fanno strani incontri e rischiano di perdere la testa.

## La locandina
<img src="alice-in-wonderland.png"  width="360px" title="Alice in Wonderland">


## Il codice
```processing
// Manuale di Programmazione Cinematografica - Volume 1
// Daniele Olmisani, 2016

// Blood Dimond


final color PAPER = color(120);
final color INK1 = color(255);
final color INK2 = color(165, 10, 30);


void setup() {
  size(480, 640);
  noLoop();
}


void draw() {
  
  float d = min(width, height) / 15.0;
  
  translate(width/2.0, height/3.0);
  
  background(PAPER);
  noStroke();
  
  fill(INK1);

  beginShape();
    vertex(-3*d, -d);
    vertex( 3*d, -d);
    vertex( 4*d,  0);
    vertex(  0, 5*d);
    vertex(-4*d,  0);
  endShape(CLOSE);
  
  translate(0, 7*d);
  
  fill(INK2);
  
  triangle(0, -d/0.7, d/2.0, 0, -d/2.0, 0);
  ellipse(0, 0, d, d);
  
  save("blood-diamond.png");
}```