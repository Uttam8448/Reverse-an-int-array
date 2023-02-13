# Reverse-an-int-array
#Repositrary for reversing an array

#include<iostream>
 using namespace std;
 void Reverse(int *arr,int size){
 	void Print(int *arr,int size1);
	int	i=0;
	int j=size-1;
	while(i<=j){
		int temp=arr[i];
		arr[i]=arr[j];
		arr[j]=temp;
		i++;
		j--;
	}
	Print(arr,size);
 }
 void Print(int *arr,int size1){
 	cout<<"\n";
 	for(int i=0;i<size1;i++){
 		cout<<arr[i]<<" ";
	 }
 }
 
 int main()
 {	int brr[10]={9,6,7,8,-2,3,4,-9,-6,5};
 	cout<<"Array : ";
	Print(brr,10);
 	cout<<"\nReversed array for 10 elements : ";
 	Reverse(brr,10);
 	int arr[9]={9,6,7,8,-2,4,-9,-6,5};
 	cout<<"\nArray : ";
	Print(arr,9);
	cout<<"\nReversed array for 9 elements : ";
 	Reverse(arr,9);
	return 0;
 }
