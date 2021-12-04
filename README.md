# helloworld
test
'''cpp
#include <bits/stdc++.h>
using namespace std;
#define N 40000
typedef pair<int, int> PII;

int main()
{
    string s;
    cin >> s;
    int i, j, k, n = s.size(), ans = 0;
    for (int i = 0; i < n; i++)
    {
        if (s[i] != 'Q')
            continue;
        for (int j = i + 1; j < n; j++)
        {
            if (s[j] != 'A')
                continue;
            for (int k = j + 1; k < n; k++)
            {
                if (s[k] == 'Q')
                    ans++;
            }
        }
    }
    cout << ans << endl;
    return 0;
}
'''
