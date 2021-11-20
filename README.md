<p align="center">
  <h1 align="center">Word to Binary Convert</h1>
  <p align="center"> Convert Your Loveletter to Binary </p>
</p> 

## Simple Knowledge

A binary number is a number expressed in the base-2 numeral system or binary numeral system, a method of mathematical expression which uses only two symbols: typically "0" and "1". The base-2 numeral system is a positional notation with a radix of 2. Each digit is referred to as a bit, or binary digit.

## CPP Code 

Copy code and test on Any Editor

```cpp
#include <bits/stdc++.h>
using namespace std;
int main()
{
    string a;
    cin>>a;
    for(int i=0;i<int(a.size());i++)
    {
    
        //convert each character to its decimal representation
        int b=int(a[i]);
        vector<int> c;
        
        //convert from dec to bin
        while(b!=0)
        {
            c.push_back(b%2);
            b/=2;
        }
        
        //Input characters
        cout<<a[i]<<" = ";
        
        //completing the missing bits
        for(int j=0;j<int(8-c.size());j++)
            cout<<0;
        
        //the output
        for(int j=c.size()-1;j>=0;j--)
            cout<<c[j];
        cout<<"\n";
    }
    cout<<"\nConvert completed..";
    return 0;
}
```


## Demo Output
```cpp
a = 01100001
z = 01111010
a = 01100001
m = 01101101

Convert completed..
```

## Contributing

Contributions are always welcome!
