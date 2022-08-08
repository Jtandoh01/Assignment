# Assignment

#include<iostream>
#include<conio.h>
using namespace std;

int main()
{ //prime numbers between 1 and a positive number n
    int n;
    cout<< "enter a number: ";
    cin>> n;
    if(n<2){
        cout<< "invalid input...";
        getch();
        return -1;
    }
    for(int i = 2;i<n; i++){
        int flag = 0;
        for(int j=2; j<= i/2; j++){
            if(i%j==0){
               flag= 1; break;
               }
        }
        if(flag==0) cout<< i << " is prime"<< endl;
    }
    getch();
    return 0;

}
