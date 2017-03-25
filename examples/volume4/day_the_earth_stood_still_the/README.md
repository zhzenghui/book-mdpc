# day_the_earth_stood_still_the (TBV)

TBV

## Il film in breve
TBV

[dettagli](TBV)

## La locandina
<img src="the-day-the-earth-stood-still.png"  width="360px" title="day_the_earth_stood_still_the">


## Il codice
```processing
// Manuale di Programmazione Cinematografica - Volume 4
// Daniele Olmisani, 2016

// The day the Earth stood still


final color PAPER = color(35);
final color INK = color(240);


void setup() {
  size(480, 640);
  noLoop();
}


void draw() {
  
  float s = 0.8 * min(width, height);
  
  translate(0.5*width, 0.3*height);
  
  background(PAPER);
  fill(INK);
  
  noStroke();
  
  ellipse(0, 0, s, 0.15*s);
  filter(BLUR, 6);
  
  ellipse(0, 0, 0.3*s, 0.2*s);
  filter(BLUR, 6);
  
  save("the-day-the-earth-stood-still.png");
}
```