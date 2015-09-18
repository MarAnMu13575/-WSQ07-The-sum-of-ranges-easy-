# -WSQ07-The-sum-of-ranges-easy-


#include <iostream>
using namespace std;

int main()
{
	 int Sum = 0;
	 int  First, Last;

	cout << "This program allows you to calculate the sum of ";
	cout << "numbers\nfrom a lower to a higher values in a range\n";
	cout << "Enter the first: ";
	cin >> First;
	cout << "Enter the last:  ";
	cin >> Last;

	// Make sure that the last number is higher than the first
	// If not, inverse them
	if( First > Last )
	{
		int Temp; //Can store only one piece of data

		Temp  = First;
		First = Last;
		Last  = Temp;
	}

	for( int Counter = First; Counter <= Last; Counter++ )
		Sum += Counter;

	cout << "\nSum of numbers from " << First << " to " << Last
	     << " = " << Sum << endl;

	return 0;
}
