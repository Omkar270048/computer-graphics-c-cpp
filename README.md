# computer-graphics-cpp

Basic Layout</br>
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

Drawing line</br>
```c++
line(x1, y1, x2, y2);
```

Drawing arc
```c++
arc(x, y, start_angle, end_angle, radius);
```
