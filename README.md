# btap#include <iostream>
using namespace std;
int main() {
  int n;
  cout << "n = ";
  cin >> n;
  int n_dao = 0;
  if(n <= 0){
    cout << "nhập lại " << endl;
  }
  else{
    for(int i = n; i > 0; i = i / 10){
         n_dao = n_dao *10 +i%10;
    }
    if(n_dao == n){
      cout << "là số thuận nghịch" << endl;
    }
    else{
      cout << "không là số thuận nghịch " << endl;
    }
  }
  return 0;
}

