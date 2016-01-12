# Visuals
This is a collection of my most recent projects developed using visual studios.
#include <iostream>
#include <string>

using namespace std;

struct MovieData
{
	string title, director;
	int year, time;

	MovieData(string t, string d, int y, int t2)
	{
		title = t, 
		director = d, 
		year = y, 
		time = t2;
	}
};

void displayMovie(MovieData &md)
{ 
	string title, 
		director;
	int year, time;

	cout << "Title        : " << md.title << endl;
	cout << "Director     : " << md.director << endl;
	cout << "Year Released: " << md.year << endl;
	cout << "Running time : " << md.time << endl;
}

int main()
{
	MovieData movie1("The Hangover", "Todd Phillips", 2009, 100),
		movie2("Inception", "Stephen Spielberg", 2010, 148);

	displayMovie(movie1);
	displayMovie(movie2);
	
	system("pause");
	return 0;
}
