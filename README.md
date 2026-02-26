#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;

int main() {
	srand(time(0));

	int randomNum = rand() % 101, guess;

	int guessCount = 0;

	while (guess != randomNum) {
		cout << "Guess the random number: ";
		cin >> guess;
		guessCount++;

		if (randomNum == guess) {
			cout << "Your answer was correct ";
			cout << "in " << guessCount << " guesses.\n";
		} else {
			cout << "Your answer was wrong. ";

			if (guess < randomNum) {
				cout << "Too low!\n";
			} else {
				cout << "Too high!\n";
			}
		}
	}

	return 0;
}
