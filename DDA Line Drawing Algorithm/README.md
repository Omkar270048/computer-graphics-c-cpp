```c
#include <stdio.h>
#include <graphics.h>

void DDA(int x1, int y1, int x2, int y2) {
  int dx = x2 - x1;
  int dy = y2 - y1;
  int steps = abs(dx) > abs(dy) ? abs(dx) : abs(dy);
  float xIncrement = dx / (float) steps;
  float yIncrement = dy / (float) steps;
  float x = x1;
  float y = y1;
  int i;
  for(i=0; i<=steps; i++) {
	  putpixel((int)x, (int)y, WHITE);
	  x += xIncrement;
	  y += yIncrement;
	}
}

int main() {
  int gd = DETECT, gm;
  int x1, x2, y1, y2;
  initgraph(&gd, &gm, "c:\\turboc3\\bgi");
  x1 = 50;
  y1 = 50;
  x2 = 200;
  y2 = 200;
  DDA(x1, y1, x2, y2);
  getch();
  closegraph();
  return 0;
}
```
