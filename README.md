# addition-of-two-complex-number




#include<iostream>
using namespace std;

class complex
{ private:
	int a,b;
	public:
		void setdata(int x,int y)
		{a=x;
		b=y;
		}
		friend complex add(complex,complex);
		void showdata();
};

complex add(complex X,complex Y)
{
	complex temp;
	temp.a=X.a+Y.a;
	temp.b=X.b+Y.b;
	return temp;
 } 
 void complex::showdata() 
 { cout <<"a="<<a<<" "<<"b="<<b<<"\n";
 }
 int main()
 {
 	complex c1,c2,c3;
 	c1.setdata(2,4) ;
 	c1.showdata() ;
 	c2.setdata(5,6) ;
 	c2.showdata();
 	c3=add(c1,c2);
 	c3.showdata() ;

 }
