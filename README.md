// C++ program to illustrate the above
// given pattern of numbers.
#include<bits/stdc++.h>
using namespace std;

int main()
{
int n = 5, i, j, num = 1, gap;
gap = n - 1;

for ( j = 1 ; j <= n ; j++ )
{
    num = j;
    for ( i = 1 ; i <= gap ; i++ )
        cout << " ";

    gap --;
    for ( i = 1 ; i <= j ; i++ )
    {
        cout << num;
        num++;
    }
    num--;
    num--;
    for ( i = 1 ; i < j ; i++)
    {
        cout << num;
        num--;
    }
    cout << "\n";
}
return 0;
}
