//# friend-function
//friend function inheritance, c++ Oop
//friend function
#include<iostream>
#include<string>
using namespace std;
class Real{
	private:
		int num;
      friend int getData(Real);//friend function declaration
      public:
      	Real():num(0){}//initial value
	
};
int getData(Real R){//friend function defination
	
	cout<<"Enter any number number"<<endl;
	cin>>R.num;
	
	return R.num;
}
int main(){
	Real r;
cout<<"Number = "<<getData(r)<<endl;	

	return 0;
} 
