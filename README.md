# Lecture-15

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
