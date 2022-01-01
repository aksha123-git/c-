# c-
#include <iostream>
using namespace std;
template< class T>
void bubble(T a[],int n)
{
    for(int i=0;i<n-1;i++)
       for(int j=n-1;i<j;j--)
          if(a[j]<a[j-1]){
              swap(a[j],a[j-1]);
          }
}
template<class X>
void swap(X &a, X&b){
    X temp =a;
    a=b;
    b=temp;
    
}
int main() {
    int x[5]={10,50,40,30,20};
    float y[5]={1.1,5.5,4.4,3.3,2.2};
    bubble(x,5);
    bubble(y,5);
    cout<<"sorted x-array" ;
    for(int i=0;i<5;i++)cout<<x[i]<<" "<<endl;
    
    cout<<"sorted y-array";
    for(int i=0;i<5;i++)
    cout<<y[i]<<" "<<endl;
    // Write C++ code here
    

    return 0;
}
