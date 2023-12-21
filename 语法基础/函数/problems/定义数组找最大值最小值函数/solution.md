```c++
#include<bits/stdc++.h>
using namespace std;
int n, a[1005];

int maxx(int a[], int len) {
	int max1 = 0;
	for (int i=1; i<=len; i++) {
		max1 = max(max1, a[i]);
	}
	return max1;
}

int minn(int a[], int len) {
	int min1 = 1e5+5;
	for (int i=1; i<=len; i++) {
		min1 = min(min1, a[i]);
	}
	return min1;
}

int main() {
	cin >> n;
	for (int i=1; i<=n; i++) {
		cin >> a[i];
	}
	cout << maxx(a, n) << '\n'; 
	cout << minn(a, n);
	return 0;
}
```