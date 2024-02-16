//Metodo Burbuja

#include<stdio.h>
#include<iostream>
#include<conio.h>

using namespace std;

int main(){
	int array[10]={4,21,56,-4,456,98,76,69,1,999};
	int aux;
	int c1=0, c2=0;
	int a=1;
	
	
	//Algortimo del metodo burbuja
		cout<<"Elige una opcion:\n OPCION1: Ascendente.\n OPCION2: Descendente. ";
	cin>>a;
	if(a==1){
		for(int i=0;i<9;i++){
			for(int j=0;j<9;j++){
				if(array[j]>array[j+1]){
				aux=array[j+1];
				array[j+1]=array[j];
				array[j]=aux;
				c2=c2+1;
				}
				else{
				c1=c1+1;
				}	
			}
		}
		cout<<"Orden Ascendente: ";
	for(int i=0;i<=9;i++){
		printf("%d\t",array[i]);
	}
	cout<<"\nNumero de comparaciones: "<<c1+c2;
	cout<<"\nNumero de Intercambios: "<<c2;
	cout<<"\n";
	}
	else;{
		for(int i=0;i<9;i++){
			for(int j=0;j<9;j++){
				if(array[j]>array[j+1]){
				aux=array[j+1];
				array[j+1]=array[j];
				array[j]=aux;
				c2=c2+1;
				}
				else{
				c1=c1+1;
				}	
			}
		}
		cout<<"\nOrden Descendente: ";
	for(int i=9;i>=0;i--){
		printf("%d\t",array[i]);
	}
	cout<<"\nNumero de comparaciones: "<<c1+c2;
	cout<<"\nNumero de Intercambios: "<<c2;
	}
	
	for(int i=0;i<9;i++){
		for(int j=0;j<9;j++){
			if(array[j]>array[j+1]){
				aux=array[j+1];
				array[j+1]=array[j];
				array[j]=aux;
				c2=c2+1;
			}
			else{
				c1=c1+1;
			}	
			
		}
	}
	
	getch();
	return 0;
}
