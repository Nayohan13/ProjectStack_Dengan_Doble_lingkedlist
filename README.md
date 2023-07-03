# ProjectStack_Dengan_Doble_lingkedlist
#include<iostream>
#include<conio.h>
using namespace std;

short stack[5], top = 0, maxstack = 5;

struct node{
	int data;
	node *next;
	node *prev;
};
node *head = NULL;

bool isEmpty(){
	if(head == NULL){
		return true;
	}
	else{
		return false;
	}
}




int main(){
	char tambah;
	
	do{
		int pilih;
		cout<<"======================================================"<<endl;
       	        cout<<"    PROGRAM STACK PADA DOUBLE LINKED CIRCULAR LIST    "<<endl;
	        cout<<"======================================================"<<endl;
     	        cout<<"1. PUSH                                               "<<endl;
      	        cout<<"2. POP                                                "<<endl;
    	        cout<<"3. FULL                                               "<<endl;
	        cout<<"4. EMPTY                                              "<<endl;
    	        cout<<"5. CLEAR                                              "<<endl;
    	        cout<<"6. PRINT                                              "<<endl;
    	        cout<<"======================================================"<<endl;
		cout<<"Masukkan nomor pilihan anda : ";
		cin>>pilih;
		
		switch(pilih)
		{
			case 1 : 
				push();
			break;
			
			case 2 : 
				pop();
			break;
			
			case 3 : 
				full();
			break;
			
			case 4 : 
				empty();
			break;
			
			case 5 : 
				clear();
			break;
			
			case 6 : 
				print();
			break;
		}
		
		cout<<endl;
		cout<<"Apakah anda ingin memilih lagi (Y/T)? : ";
		cin>>tambah;
		cout<<endl<<endl;

system("cls");
		
	} while(tambah == 'Y');
	cout<<endl;
	
	
	system("pause");
	return 0;
}
