#include<iostream>
using namespace std;
int main()
{
    cout<<"Hello World"<<endl;

    return 0;
}

#include<iostream>
#include<conio.h>
using namespace std;

int main()
{
    double farn,cels;
    cout<<"Enter celius : \n";
    cin>>cels;

    farn = 1.8* cels+ 32;

    cout<<"Fahrenheit = "<<farn;

    getch();

}

toupper() && tolower
#include<iostream>
using namespace std;
int main()
{
    char ch;

    cout<<"Enter any letter : ";
    cin>>ch;

    ch = tolower(ch);
    if (ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u') {
        cout<<"Vowel";
    }
    else {
    cout<<"Consonant";
    }

    return 0;

}

//Leap Year program
#include<iostream>
using namespace std;
int main()
{
   int year;
   cout<<"Enter any year : ";
   cin>>year;

   if(year%4==0 && year%100==0)
   {
       cout<<"Leap YEar";
   }
   else if(year%400==0)
   {
       cout<<"Leap Year";
   }
   else
   {
       cout<<"Not Leap Year";
   }
    return 0;

}

