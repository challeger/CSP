```c++
#include<bits/stdc++.h>
using namespace std;
string s;

void tobig(string& a) {
	int len = a.size();
	for (int i=0; i<len; i++) {
		if (a[i]>='a' and a[i]<='z') a[i] -= 32;
	}
}

void tosmall(string& a) {
	int len = a.size();
	for (int i=0; i<len; i++) {
		if (a[i]>='A' and a[i]<='Z') a[i] += 32;
	}
}

int main() {
	cin >> s;
	tobig(s);
	cout << s << '\n';
	tosmall(s);
	cout << s << '\n';
	return 0;
}
```