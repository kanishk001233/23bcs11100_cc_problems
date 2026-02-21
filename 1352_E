#include <iostream>
#include <vector>
using namespace std;

int main()
{
    long long t;
    cin >> t;

    while(t--)
    {
        long long n;
        cin >> n;

        vector<long long> a(n);
        vector<long long> b(n + 1, 0);

        for(long long i = 0; i < n; i++)
        {
            cin >> a[i];
        }

        for(long long i = 0; i < n; i++)
        {
            long long sum = a[i];

            for(long long j = i + 1; j < n; j++)
            {
                sum = sum + a[j];

                if(sum > n)
                {
                    break;
                }

                b[sum] = 1;
            }
        }

        long long abc = 0;

        for(long long i = 0; i < n; i++)
        {
            if(b[a[i]] == 1)
            {
                abc++;
            }
        }

        cout << abc << endl;
    }

    return 0;
}
