# Good-morning-function
#display good morning, night, afternoon or evening based on the number entered
#include<iostream>
using namespace std;  
string greetings(int time)   //defining the function
{
	if (time < 12)       //using else-if statement
	{
		return "Good Morning! ";
	}
	else if (time>=12 && time<=17)
	{
		return "Good Afternoon! ";
	}
	else if (time >= 18 && time <= 21)
	{
		return "Good Evening ";
	}
	else if (time >= 22 && time <= 24)
	{
		return "Good Night ";
	}
}
int main()     //main function
{
	int userinput;   ///declaring variable 'userinput' with datatype integer
	cout << "What time is it? " << endl;
	cin >> userinput;
	cout << greetings(userinput) << endl;
	return 0;
}
