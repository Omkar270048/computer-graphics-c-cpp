# computer-graphics-cpp

Basic Layout
```c++
#include<graphics.h>
#include<stdio.h>
#include<conio.h>

void main(){
	int gdriver = DETECT, gmode;
	/*
    		code goes here
  	*/
	getch();
	closegraph();
}
```

Drawing line
```c++
line(x1, y1, x2, y2);
```

Drawing arc
```c++
arc(x, y, start_angle, end_angle, radius);
```

Drawing Circle
```c++
circle(x, y, radius);
```

Drawing Rectangle
```c++
rectangle(x1, y1, x2, y2);
```

Drawing Hut
```c
// Drawing hut

#include<iostream.h>
#include<graphics.h>
#include<conio.h>
#include<stdlib.h>

void main(){
	int gd = DETECT, gm;
	initgraph(&gd, &gm, "c:\\turboc3\\bgi");
	
	line(100, 100, 400, 100 );
	line(100, 100, 50, 200);
	line(50, 200, 400, 200);
	line(400, 400, 400, 200);
	line(400, 100, 400, 200);
	line(150, 200, 150, 400);
	line(100, 100, 150, 200);
	rectangle(50,  200, 400, 400);
	getch();
	closegraph();
}
```

