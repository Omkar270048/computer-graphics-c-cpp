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
