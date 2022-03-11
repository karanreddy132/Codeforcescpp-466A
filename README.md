# Codeforcescpp-466A
#include <bits/stdc++.h>

using namespace std;

int main(){
  int n,m,a,b;

  cin >> n >> m >> a >> b;

  if(b > a*m){
    cout << n*a;
  }
  else{
    if(b < (n%m)*a){
      cout << ((n/m)+1)*b;
    }
    else{
      cout << (n/m)*b + (n%m)*a;
    }
  }
  return 0;
}
