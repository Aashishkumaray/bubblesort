Q-4.

#include<iostream>
#include<algorithm>
#include<iostream>
using namespace std;
int main(){
    int arr[5]={8,9,1,2,0};
    int n=5;
    for(int i=0;i<n;i++){
        for(int j=0;j<n-1-i;j++){
        if(arr[j]<arr[j+1]){
            swap(arr[j],arr[j+1]);
        }
        }
    }
    for(int i=0;i<n;i++){
        cout<<arr[i]<<" ";
    }
}



Q-5
#include<iostream>
#include<vector>
using namespace std;
int main(){
    int arr[]={4,2,7,9,8};
    int n=5;
for(int i=0;i<n;i++){
    cout<<arr[i];
}
for(int i=0;i<n;i++){
if(arr[i]>arr[i+1]){
swap(arr[i],arr[i+1]);
i++;
}
}
bool flag=true;
for(int i=0;i<n;i++){
   if (arr[i]>arr[i+1]){
    flag=false;
    break;
}
}
if(flag==true)
    cout<<"almost sorted;";
else cout<<" almost  not sorted;";
}
