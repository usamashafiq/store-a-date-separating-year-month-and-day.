#include<iostream>
#include<conio.h>
using namespace std;
struct date {
	int day;
	int month;
	int year;

};
int main()
{
	date Dob;
	int c;
	cout << "Enter your Date of Birth : "<< endl;
	cin >> Dob.day >> Dob.month >> Dob.year;
	cout << "input (1) for print Date (d-m-y)  " << endl;
	cout << "input (2) for print Date (m/d/y)  " << endl;
	cout << "input (3) for print Date (d-month in string-y)  " << endl;
	cin >> c;
	switch (c) {

	case 1 : 
		cout << Dob.day << "-" << Dob.month << "-" << Dob.year;
		break;
	case 2:
		cout << Dob.month << "-" << Dob.day << "-" << Dob.year;
		break;
	case 3 :
		cout << Dob.day<<"-";
		switch (Dob.month) {
		case 1:
			cout << "Janury";
			break;
		case 2:
			cout << "Febrary";
			break;
		case 3:
			cout << "March";
			break;
		case 4:
			cout << "April";
			break;
		case 5:
			cout << "May";
			break;
		case 6:
			cout << "June";
			break;
		case 7:
			cout << "July";
			break;
		case 8:
			cout << "Agust";
			break;
		case 9:
			cout << "September";
			break;
		case 10:
			cout << "October";
			break;
		case 11:
			cout << "Nonember";
			break;
		case 12:
			cout << "December";
			break;
		}
		cout <<"-"<< Dob.year;
	}
	_getch();
}

