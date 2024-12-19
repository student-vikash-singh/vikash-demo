#include<iostream>
using namespace std ;
int getmin(int num [],int n ){
    int min = INT16_MAX;
    for(int i =0; i<n; i++){
        if (num[i]<min){
            min =num[i];
    }
    }
    return min;
}
int getmax(int num[],int n){
    int max=INT16_MIN;
    for(int i=0; i<n; i++){
        if(num[i]>max){
            max=num[i];
        }
        
    }
    return max;
}
     int main (){
    int size;
    cin>>size;
     int num [100];
     for(int i=0; i<size; i++){
        cin>>num[i]; 
     }  
     
     cout<<"getmaximum value is :"<<getmax( num,size)<<endl;
     cout<<"getminimum value is :"<<getmin(num,size)<<endl;
     
     
}
