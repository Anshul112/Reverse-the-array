# Reverse-the-array
 Given an array, the task is to reverse the array


#include<bits/stdc++.h>
using namespace std;

int main()
{
    int n;
    cout<<"Enter the size of array :";
    cin>>n;
    int a[n];
    cout<<"Enter elements :-\n";
    for(int i=0;i<n;i++)
    {
        cin>>a[i];
    }
    int i = 0;
    int j = n-1;
    while(i<j)
    {
        int temp = a[i];
        a[i] = a[j];
        a[j] = temp;
        i++;
        j--;
    }
    cout<<"Reverse array is :\n";
    for(int i=0;i<n;i++)
    {
        cout<<a[i]<<" ";
    }
    return 0;
}
