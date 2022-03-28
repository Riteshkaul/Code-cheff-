#include <iostream>
#include<bits/stdc++.h>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while (t--)
	{
	    int n;
	    cin>>n;
	    int day[n];
	    for(int i=0;i<n;i++)
	    {
	        cin>>day[i];
	    }
	    sort(day,day+n);
	    int save =n;
	    for(int i=0;i<n;i++)
	    {
	        if(day[i]==day[i+1])
	        {
	            save--;
	        }
	        
	    }
	    cout<<save<<endl;
	}
	return 0;
}
