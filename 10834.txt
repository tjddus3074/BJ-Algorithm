#include <iostream>
using namespace std;
typedef long long ll;

int main() {
	int n; cin >> n;
	int cnt = 0;

	ll ans = 1;
	for (int i = 0,s; i < n; i++) {
        ll a,b;
		cin >> a >> b >> s;
		if (s == 1) cnt++;
		ans = (ans * b) / a;
	}

	cout << cnt % 2 << " "<< ans << '\n';

}