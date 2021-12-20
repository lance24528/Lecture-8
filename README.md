//Days of the month

#include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;

int main() {	

	int m;
	cout << "Enter the number corresponding to the the month\n\n1: January\n2: February\n3: March\n4: April\n5: May\n6: June\n7: July\n8: August\n9: September\n10: October\n11: November\n12: December\n" << endl;
	cin >> m;
	switch (m) {
	case 1: cout << "\nJanuary has 31 days"; break;	
	case 2: cout << "\nFebruary month has 28 days or 29 days if it is a leap year"; break;
	case 3: cout << "\nMarch has 31 days"; break;
	case 4: cout << "\nApril has 30 days"; break;
	case 5: cout << "\nMay has 31 days"; break;
	case 6: cout << "\nJune has 30 days"; break;
	case 7: cout << "\nJuly has 31 days"; break;
	case 8: cout << "\nAugust has 31 days"; break;
	case 9: cout << "\nSeptember has 30 days"; break;
	case 10: cout << "\nOctober has 31 days"; break;
	case 11: cout << "\nNovember has 30 days"; break;
	case 12: cout << "\nDecember has 31 days"; break;
	default: cout << "\nInvalid input, Try again"; break;
	}
	return 0;
}
  
//Fuel me up
  
#include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;

int main() {	

	char fuel; int L; double dieselp = 2.77, petrolp = 2.66;
	cout << "Gas Station, Do you want fuel? If yes Enter the number of liters you want, If no Input 0\nFuel: ";
	cin >> L;	
	if (L > 0)
	{	
		cout << "What type of gas do you want? Input P for petrol and D for diesel" << endl;
		cin >> fuel;
		switch (fuel)
		{
		case 'P': case 'p': cout << L << " Liters of Petrol, You need to pay aed: " << petrolp * L << endl; break;
		case 'D': case 'd': cout << L << " Liters of Diesel, You need to pay aed: " << dieselp * L << endl; break;
		default: cout << "Invalid Input, Try again\n"; break;
		}
	}
	else
	{
		cout << "Thank you for passing by the Gas Station";
	}
	return 0;
}
  
//Switching Temperature
  
#include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;

int main() {	

char temp; 	double tempN;
cout << "Temperature Converterinator\nInput the letter F if you want to convert from Fahrenheit to celcius\nOr Input the letter C if you want to convert from Celcius" << endl;
	cin >> temp;
	if (temp == 'C' || temp == 'c' || temp == 'F' || temp == 'f') {
		cout << "Input temperature (Number): ";
		cin >> tempN;
		if (!cin.fail()) {
			switch (temp)
			{
			case 'C': case 'c': cout << tempN << " = Celcius to Fahrenheit = " << (tempN * 9 / 5) + 32 << endl; break;
			case 'F': case 'f': cout << tempN << " = Fahrenheit to Celcius = " << (tempN - 32) * 5 / 9 << endl; break;
			default: cout << "Invalid Input, Try again"; break;
			}
		}
		else
		{
			cout << "Invalid Input, Try again";
		}
	}
	else
	{
		cout << "Invalid Input, Try again";
	}
	return 0;
}
  
//Switch Grade Calculator
  
  #include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;

int main() {	

	cout << "Switch Grade Calculator\n\nEnter your name: ";
	string fname; int mark; char grade = 'z';
	getline(cin, fname); cout << "Marks: "; cin >> mark;
	if (mark <= 40)char grade = 'F';
	if (mark >= 40 && mark <= 49)  grade = 'E';
	if (mark >= 50 && mark <= 59)  grade = 'D';
	if (mark >= 60 && mark <= 69)  grade = 'C';
	if (mark >= 70 && mark <= 79)  grade = 'B';
	if (mark >= 80 && mark <= 100)  grade = 'A'; 
	if (cin.fail()) cout << "Invalid Input, Try again"; 
	switch (grade){
	case 'A': case 'a': cout << fname << " you got = " << grade; break;
	case 'B':case 'b': cout << fname << " you got = " << grade; break;
	case 'C':case 'c': cout << fname << " you got = " << grade; break;
	case 'D':case 'd': cout << fname << " you got = " << grade; break;
	case 'E':case 'e': cout << fname << " you got = " << grade; break;
	case 'F':case 'f': cout << fname << " you got = " << grade; break;
	default: cout << "Invalid Input, Try again"; break;
	}
	return 0;
}
