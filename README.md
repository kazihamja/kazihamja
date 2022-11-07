#include <GL/gl.h>
#include <GL/glu.h>
#include <GL/glut.h>
void display ();
void reshape(int,int);
void init()
{
    glClearColor (0.0,0.0,0.0,0.0 );

}
int main ( int argc, char**argv)
{
    glutInit(&argc,argv);
    glutInitDisplayMode(GLUT_RGB);
    glutInitWindowPosition(200,50);
    glutInitWindowSize(700,500);
    glutCreateWindow("Rifat Assignment");
    glutDisplayFunc(display);
    glutReshapeFunc(reshape);

    init();

    glutMainLoop();
}

void display()
{
    glClear(GL_COLOR_BUFFER_BIT);
    glLoadIdentity();

     glPushMatrix();
         glBegin(GL_POLYGON);
    glColor4f(1.0f, 1.0f, 1.0f, 0.0f);
    glVertex2f(4,5);
    glVertex2f(30,5);
    glVertex2f(33.5,4);
    glVertex2f(1.5,4);
    glEnd();

    glPushMatrix();
         glBegin(GL_POLYGON);
  glColor4f(1.0f, 0.0f, 0.0f, 0.0f);
    glVertex2f(5.5,4);
    glVertex2f(28,4);
    glVertex2f(30.5,3);
    glVertex2f(3.5,3);
    glEnd();

    glPushMatrix();
         glBegin(GL_POLYGON);
       glColor3f(0.0f, 1.0f, 0.0f);
    glVertex2f(7,3);
    glVertex2f(25,3);
    glVertex2f(28,2);
    glVertex2f(4,2);
    glEnd();

     glPushMatrix();
         glBegin(GL_QUADS);
       glColor4f(1.0f, 1.0f, 0.0f, 0.0f);
    glVertex2f(5.5,10);
    glVertex2f(8,10);
    glVertex2f(8,5);
    glVertex2f(5.5,5);
    glEnd();

        glPushMatrix();
         glBegin(GL_QUADS);
       glColor4f(1.0f, 1.0f, 0.0f, 0.0f);
    glVertex2f(10,12);
    glVertex2f(12.5,12);
    glVertex2f(12.5,5);
    glVertex2f(10,5);
    glEnd();

     glPushMatrix();
         glBegin(GL_QUADS);
      glColor4f(1.0f, 1.0f, 0.0f, 0.0f);
    glVertex2f(14.5,14.5);
    glVertex2f(17.5,14.5);
    glVertex2f(17.5,5);
    glVertex2f(14.5,5);
    glEnd();

    glPushMatrix();
         glBegin(GL_QUADS);
      glColor4f(1.0f, 1.0f, 0.0f, 0.0f);
    glVertex2f(19,12);
    glVertex2f(21.5,12);
    glVertex2f(21.5,5);
    glVertex2f(19,5);
    glEnd();

        glPushMatrix();
         glBegin(GL_QUADS);
      glColor4f(1.0f, 1.0f, 0.0f, 0.0f);
    glVertex2f(23.5,10);
    glVertex2f(26,10);
    glVertex2f(26,5);
    glVertex2f(23.5,5);
    glEnd();

     glPushMatrix();
         glBegin(GL_QUADS);
    glColor3f(0.5f, 1.0f, 1.0f);
    glVertex2f(40,18);
    glVertex2f(55,18);
    glVertex2f(55,2);
    glVertex2f(40,2);
    glEnd();


     glPushMatrix();
         glBegin(GL_QUADS);
    glColor3f(0.1f, 0.0f, 0.1f);
    glVertex2f(42,6);
    glVertex2f(45,6);
    glVertex2f(45,3.5);
    glVertex2f(42,3.5);
    glEnd();

     glPushMatrix();
         glBegin(GL_QUADS);
    glColor3f(0.1f, 0.0f, 0.1f);
    glVertex2f(42,10);
    glVertex2f(45,10);
    glVertex2f(45,7.5);
    glVertex2f(42,7.5);
    glEnd();

     glPushMatrix();
         glBegin(GL_QUADS);
    glColor3f(0.1f, 0.0f, 0.1f);
    glVertex2f(42,14);
    glVertex2f(45,14);
    glVertex2f(45,11.5);
    glVertex2f(42,11.5);
    glEnd();

     glPushMatrix();
         glBegin(GL_QUADS);
    glColor3f(0.1f, 0.0f, 0.1f);
    glVertex2f(50,14);
    glVertex2f(53,14);
    glVertex2f(53,11.5);
    glVertex2f(50,11.5);
    glEnd();

     glPushMatrix();
         glBegin(GL_QUADS);
    glColor3f(0.1f, 0.0f, 0.1f);
    glVertex2f(50,10);
    glVertex2f(53,10);
    glVertex2f(53,7.5);
    glVertex2f(50,7.5);
    glEnd();

     glPushMatrix();
         glBegin(GL_QUADS);
    glColor3f(0.1f, 0.0f, 0.1f);
    glVertex2f(50,6);
    glVertex2f(53,6);
    glVertex2f(53,3.5);
    glVertex2f(50,3.5);
    glEnd();



















    glFlush();
    glutSwapBuffers();
}





void reshape (int w,int h)
{
    glViewport(0,0,(GLsizei)w,(GLsizei)h);
    glMatrixMode(GL_PROJECTION);
    glLoadIdentity();
    gluOrtho2D(-5,80,-5,30);
    glMatrixMode(GL_MODELVIEW);
}
