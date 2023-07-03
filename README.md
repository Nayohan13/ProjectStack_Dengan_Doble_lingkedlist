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
