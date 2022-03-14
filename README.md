# super
import java.util.*;
class figure
{
int l,w;
figure(int x,int y)
{
l=x;
w=y;
}
void area()
{
System.out.println("area of figure");
}
}
class rectangle extends figure
{
rectangle(int a,int b)
{
super(a,b);
}
void area()
{
System.out.println("area of rectangle"+l*w);
}
}
class triangle extends figure
{
triangle(int t,int y)
{
super(t,y);
}
void area()
{
System.out.println("area of triangle"+l*w/2);
}
}
class Main 
{
public static void main(String args[])
{
rectangle obj1=new rectangle(40,30);
obj1.area();
triangle obj2=new triangle(30,60);
obj2.area();
}
}
