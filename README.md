
#include <glut.h>
void display (){
glClearColor(1,1,1,1);
glClear(GL_COLOR_BUFFER_BIT);
glColor3f(0,1,1);
glEnable(GL_POINT_SMOOTH);
glPointSize(10);
glBegin(GL_POINTS);
glVertex2f(40,60);
glVertex2f(50,50);
glEnd();
   glFlush();
}
void main(){
glutInitWindowPosition(100,100);
glutInitWindowSize(500,500);
glutCreateWindow("Point");
gluortho2D(0,100,0,100);
glutDisplayFunc(display);
glutMainLoop();

}
