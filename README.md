#include <iostream>
#include <vector>
using namespace std;

int main() {
    int chosenNumber = 7;       // fixed chosen number
    int userGuess;              // user input
    vector<int> guesses;        // store all guesses

    cout << "Guess the number!" << endl;

    while (true) {
        cout << "Enter your guess: ";
        cin >> userGuess;
        guesses.push_back(userGuess);

        if (userGuess > chosenNumber) {
            cout << "Too high" << endl;
        } else if (userGuess < chosenNumber) {
            cout << "Too low" << endl;
        } else {
            cout << "Correct!" << endl;
            break;  // exit loop when correct
        }
    }

    cout << "\nYour guesses were: ";
    for (int g : guesses) {
        cout << g << " ";
    }
    cout << endl;

    return 0;
}
# 202511263_DSA_viviana
202511263_DSA_viviana_assignment
