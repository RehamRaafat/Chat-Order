#include <bits/stdc++.h>

using namespace std;

int main()
{
    int x;
    vector<string>v;
    map<string,int>cl;
    cin>>x;
    for(int i=0; i<x; i++)
    {
        string s;
        cin>>s;
        v.push_back(s);
    }
    for(int j=x-1;j>=0;j--)
    {
        if (cl[v[j]]==0)
        cout<<v[j]<<endl;
        cl[v[j]]=-1;
    }

    return 0;
}
