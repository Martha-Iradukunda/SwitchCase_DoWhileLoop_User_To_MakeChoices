# SwitchCase_DoWhileLoop_User_To_MakeChoices
//A simple C++ program to alow a user to select an operator(addition, subtraction, multiplication, and division signs,), input two values to be operated on. Then you will be allowed to redo the process depending on the choice you select. 


#include <iostream>
//@Author-Martha

/* run this program using the console pauser or add your own getch, system("pause") or input loop */
using namespace std;
int main(int argc, char** argv) {
	
	int a,b,reply,oper;
	
	do{
	cout<<"select an operator:\n1. Addition(+)\n2. Subtraction(-)\n3. Multiplication(*)\n4. Division(/)\n";
	cin>>oper;
			
		cout<<"Enter value of a\n";
		cin>>a;
		cout<<"Enter value of b\n";
		cin>>b;
		
       switch(oper){
       	
	    case 1:
		if(oper==1){
		int sum=a+b;
		cout<<"The sum is: "<<sum<<endl;	
		}
		break;
		
		case 2:
		if(oper==2){
		int sub=a-b;
		cout<<"The difference is: "<<sub<<endl;	
		}
		break;
		
		case 3:
		if(oper==3){
		int prod=a*b;
		cout<<"The product is: "<<prod<<endl;
	       }
		break;
		
		case 4:
			if(oper==4){
		int div=a/b;
		cout<<"The quotient is: "<<div<<endl;
	     	}
		break;
		
		default:
		cout<<"You have selected a wrong operator\n";
			break;
}
	cout<<"would you like to continue?Please select:\n1. To continue\n2. To exit\n";
	cin>>reply;	
	
		if(reply!=1&&reply!=2){
		cout<<"Wrong choice!! Please select:\n1. To continue\n2. To exit\n";
		cin>>reply;
	}
	}while(reply==1);
	return 0;
}
