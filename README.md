#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main() {
    srand(time(0));
    
int randomNum = rand() % 101, guess;
while (guess != randomNum) {
cout << " guess the random number ";
cin >> guess;
if (randomNum == guess) {
    cout << "you answer was correct ";
} else {
  cout << "your answer was wrong ";
}
} 
return 0;
}
