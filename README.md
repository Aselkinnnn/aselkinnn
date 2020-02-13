#include "pch.h"
#include <iostream>
#include <string>
#include<list>
using namespace std;

int main()
{
	int y,q=0,i,z=0;
	list<int> listone = { 2, 4, 3 };
	list<int> listtwo = { 5, 6, 4 };
	list<int> listthree = {};

	for (i = 0; i < 3; i++) {
	
		y = listone.back() + listtwo.back();
		y = y + z;
		q = y % 10;
		listthree.push_back(q);
		if(y<=10)
		{
			z = y / 10;
		}
		else { z = 0; }

		listone.pop_back();
		listtwo.pop_back();
	}
	cout << endl << " = " << endl;
	for (i = 0; i < 3; i++) {
		cout << listthree.back() ;
		listthree.pop_back();
	}

	return 0;
}



