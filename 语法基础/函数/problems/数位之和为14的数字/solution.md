```c++
#include<bits/stdc++.h>
using namespace std;
int n, m;

int get_sum(int x) {
	int sum = 0;
	while (x) {
		sum += x%10;
		x /= 10;
	}
	return sum;
}

int main() {
	int n, m, flag=0;
	cin >> n >> m;
	for (int i=n; i<=m; i++) {
		if (get_sum(i) == 14) {
			cout << i << '\n';
			flag = 1;
		}
	}
	if (flag == 0) cout << -1;
	return 0;
}
```