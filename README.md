
#include<iostream>
#include<bits/stdc++.h>
#include<math.h>
using namespace std;

int main()
{
    int n;
    cin>>n;
    char s[n];
    cin>>s;
    int count=0;
    
    for(int i=0;i<n-2;i++)
    {
        if(s[i]=='0' && s[i+1]=='1' && s[i+2]=='0')
        {
       
            count++;
            i+=2;
        }
    }
    
    cout<<count<<endl;
    return 0;
}
