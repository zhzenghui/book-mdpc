---
permalink: /examples/volume3/bee_movie/
---
# Bee Movie (2007)

Animazione, Avventura, Commedia

## Il film in breve
Barry B. Benson, a bee just graduated from college, is disillusioned at his lone career choice: making honey. On a special trip outside the hive, Barry's life is saved by Vanessa, a florist in New York City. As their relationship blossoms, he discovers humans actually eat honey, and subsequently decides to sue them.

[dettagli](https://www.imdb.com/title/tt0389790/)

## La locandina
<img src="bee-movie.png"  width="360px" title="Bee Movie">


## Il codice
```java
// Manuale di Programmazione Cinematografica - Volume 3
// Daniele Olmisani, 2016

// Bee Movie


final color PAPER = color(70, 25, 20);
final color INK = color(250, 220, 55);

final int STRIPES = 3;


void setup() {
  size(480, 640);
  noLoop();
}

void draw() {
  
  float dH = height / (2*STRIPES);
  
  background(PAPER);
  
  fill(INK);
  noStroke();
  
  for (int i=0; i<STRIPES; i++) {
    
    rect(0, 0, width, dH);
    translate(0, 2*dH);
  }
  
  save("bee-movie.png");
}
```
