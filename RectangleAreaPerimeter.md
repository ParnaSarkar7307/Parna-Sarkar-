#include<iostream>
using namespace std;
class Rectangle{
    private : 	
          int length ;
          int breadth;
    public  : 
        Rectangle(){
	      int length =1;
          int breadth=1;}
          
          Rectangle(int l, int b){
		  length = l;
          breadth = b;
		  }
           void setLength(int l){length =l;}
           void setBreadth(int b){breadth =b;}
           int getArea(){return length*breadth;}
           int getPerimeter(){ return 2*(length+breadth);}
           void show(){
           	cout<<"length, breadth, area, perimeter = "<< length<<breadth<< getArea()<<getPerimeter()<<endl;
		   }
           
		   };
int main(){
	Rectangle r1;
	Rectangle r2(4,5);
	r1.setLength(2);
	r1.setBreadth(3);
	r1.show(); 
	r2.show();
	
}
