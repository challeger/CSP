```c++
#include<bits/stdc++.h>
using namespace std;

bool check(int n) {
	int a = n%10, b = n/10%10, c = n/100%10;
	return a*a*a+b*b*b+c*c*c == n;
}

int main() {
	int n;
	cin >> n;
	if (check(n)) cout << "yes";
	else cout << "no";
    return 0;
}
```