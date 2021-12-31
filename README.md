# 90DAYSDSA
QAUDRATIC EQUATION CODE -
#include <iostream>
#include <cmath>
#include <math.h>
using namespace std;
int findDIS(int A, int B, int C)
{
    int X,X1, X2;
    int dis = B*B-4*A*C;
    if(dis<0){
        cout<<"it has no real solution";
    }
    else if(dis=0){
        X=-B/2*A;
        cout<<"it has one real solution"<<" "<<X;
    }
    else{
        X1=(-B+sqrt(dis))/2*A;
        X2=(+B+sqrt(dis))/2*A;
        cout<<"it has two distinct real solutions"<<" "<<X1<<" "<<X2;
    }
    return dis;
}

int main()
{
    int A,B,C;
    cin>>A>>B>>C;
    findDIS(A,B,C);
    return 0;
}
