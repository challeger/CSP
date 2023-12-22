```c++
#include<bits/stdc++.h>
using namespace std;
string s;
char c;

int count(string s, char c) {
	int len = s.size(), res = 0;
	for (int i=0; i<len; i++) {
		if (s[i] == c or abs(s[i]-c) == 32) res++;
	}
	return res;
}

int main() {
	cin >> s >> c;
	cout << count(s, c);
	return 0;
}
```