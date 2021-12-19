# lecture-15



root calculator with pow func
#include <iostream>
#include <string>
#include <math.h>
using namespace std;
int main()
{
	cout << "Enter a number you want the square root and cube root of" << endl;
	int x;
	cin >> x;
	while (cin.fail())
	{
		cout << "Invalid command enter the numbers again: " << endl;
		cin.clear();
		cin.ignore(1000, '\n');
		cin >> x;
	}

	cout << "The square-root of "<<x <<" is " << sqrt(x) << endl;
	cout << "The cube-root of " << x << " is " << cbrt(x) << endl;
	//cout << "The cube-root of "<< x << " is " << pow(x, 0.333333333333333) << endl;
	//cout << "The square-root of "<< x << " is " << pow(x, 0.5) << endl;
	return 0;
}
  
  
  
  Lecture 15 p2 function time
  #include <iostream>  
using namespace std;
/* return type set to string as this function will return a string value back  to main program */

string greetings(int time) {
	//evaluate int value passed in and set return message 
	if (time < 12) {
		return "Good Morning";
	}
	else if(time >=12 && time <=17)  {
		return "Good Afternoon";
	}
	else if (time >= 18 && time <= 21) {
		return "Good Evening";

	}
	else if (time >= 22 && time <= 24) {
		return "Good Night";
	}

}
int main() {
	cout << "What time is it? Enter the time in 24 format" << endl; //ask the user for time 
	int userInput; //variable to store user response
	cin >> userInput; //get user input

	//output string returned by function 
	cout << greetings(userInput) << endl;
	return 0;
}
