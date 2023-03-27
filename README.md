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

Drawing ellipse
```c
ellipse(x, y, startingAngle, endingAngle, radius1, radius2);

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

Draw circle, rectangle, ellipse & half ellipse in 4 region
```c
//draw circle, rectangle, ellipse & half ellipse in 4 region

#include<iostream.h>
#include<graphics.h>
#include<conio.h>
#include<stdlib.h>

void main(){
	int gd = DETECT, gm;
	initgraph(&gd, &gm, "c:\\turboc3\\bgi");
	int xcen = getmaxx()/2;
	int ycen = getmaxy()/2;
	line(xcen, 0, xcen, getmaxy());
	line(0, ycen, getmaxx(), ycen);
	circle(xcen/2, ycen/2, 50);
	rectangle(xcen+50, ycen-200, xcen+200, ycen-50);
	ellipse(xcen/2, ycen+ycen/2, 0, 360, 100, 50);
	ellipse(xcen+xcen/2, ycen+ycen/2, 0, 180, 100, 50);
	
	getch();
	closegraph();
}
```
Draw circle, rectangle, square, ellipse, line at the centere of screen
```cpp
#include<iostream.h>
#include<conio.h>
#include<graphics.h>
void main(){
	int xcen, ycen;
	int gd = DETECT, gm;
	initgraph(&gd, &gm, "c:\\turboc3\\bgi");
	xcen = getmaxx()/2;
	ycen = getmaxy()/2;
	
	line(xcen, 0, xcen, getmaxy());
	line(0, ycen, getmaxx(), ycen);
	
	circle(xcen, ycen, 200);
	
	rectangle(xcen-200, ycen-200, xcen+200, ycen+200);
	rectangle(xcen-120, ycen-180, xcen+120, ycen+180);
	
	ellipse(xcen, ycen, 0, 360, 50, 100);
	getch();
	
}
```

Concentric circles
```cpp
#include<iostream.h>
#include<conio.h>
#include<graphics.h>
void main(){
	int xcen, ycen, i, color = 1;
	int gd = DETECT, gm;
	initgraph(&gd, &gm, "c:\\turboc3\\bgi");
	xcen = getmaxx()/2;
	ycen = getmaxy()/2;
	
	for(i = 20; i<=200; i+= 20){
		setcolor(color++);
		circle(xcen, ycen, i);
	}
	
	getch();
	
}                                      
```





