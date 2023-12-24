```c++
#include<bits/stdc++.h>
using namespace std;
int n, q[125][125];
int res = -100000000;

int main(){
	scanf("%d", &n);
	for (int i=1; i<=n; i++) {
		for (int j=1; j<=n; j++) {
			cin >> q[i][j];
			q[i][j] += q[i-1][j]+q[i][j-1]-q[i-1][j-1];  // 二维前缀和 
		}
	}
	
	for (int i=1; i<=n; i++) {
		for (int j=1; j<=n; j++) {
			// 左上角的点 i, j
			for (int x=i; x<=n; x++) {
				for (int y=j; y<=n; y++) {
					res = max(res, q[x][y]-q[i-1][y]-q[x][j-1]+q[i-1][j-1]);
				}
			} 
		}
	}
	cout << res;
	return 0;
}
```