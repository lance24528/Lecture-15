//# Lecture-15
#include <iostream>
#include <string>
#include <iomanip>
#include <array>
#include <math.h>
using namespace std;

void welcome();
void welcome1();
void goodbye();
int main() {
	welcome1();
	goodbye();
	//welcome();
	return 0;
}
void welcome() {
	
	cout << " Welcome to BSU" << endl;
}
void welcome1() {
	cout << " Welcome to my program " << endl;
}
void goodbye() {
	cout << " End of program " << endl;
}
//Time checker
#include <iostream>
#include <array>
#include <string>
#include <math.h>
using namespace std;


string timeChecker(int userTime)
{
	string response;
	if ((userTime <= 11) && (userTime >= 0)){
		response = "Good morning";
	}
	if ((userTime <= 17) && (userTime >= 12)){
		response = "Good afternoon";
	}
	if ((userTime <= 21) && (userTime >= 18)){
		response = "Good Evening";
	}
	if ((userTime <= 24) && (userTime >= 22)){
		response = "Good Night";
	}
	return response;
}
int main()
{
	int userTime;
	cout << "Enter Time: ";
	cin >> userTime;
	while (cin.fail()) {
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Invalid Input, Enter Time again: ";
		cin >> userTime;
	}
	cout << timeChecker(userTime);
	return 0;
}	
