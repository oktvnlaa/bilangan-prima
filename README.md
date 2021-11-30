# bilangan-prima
#include <iostream>
using namespace std;

int main(){
	int a, i;
	bool bilanganprima = true;
	cin>>a;
	
	if(a==0 || a==1){
		bilanganprima = false;
		
	}else{
		for (i=2; i<=a/2; i++){
			if (a%i==0){
				bilanganprima = false;
				break;
			}
		}
	}
	cout<<endl;
	if (bilanganprima)
	cout<<a<<" adalah bilangan prima";
	else
	cout<<a<<" bukan bilangan prima";
	return 0;
	}
