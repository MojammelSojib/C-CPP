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

int main() {
   int year;
   cout << "Enter any year: ";
   cin >> year;

   if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
       cout << "Leap Year";
   }
   else {
       cout << "Not Leap Year";
   }

   return 0;
}

// conditional operator / Ternary Operator

#include<iostream>
using namespace std;

int main() {
   int num1,num2;
   num1=90;
   num2=34;

   int max =(num1>num2)?num1:num2;
   cout<<max;
   return 0;
}
// conditional operator / Ternary Operator
#include<iostream>
using namespace std;

int main() {
   int num;
   cout<<"Enter any integer : ";
   cin>>num;

   (num%2==0)?cout<<num<<" is even " :cout<<num<<" is odd";

   return 0;
}

//while loop
#include<iostream>
using namespace std;

int main(){
    int i=1;//initalization
    while(i<=100)//condition check
    {
        cout<<i<<endl;
        i++;//increment
    }
    cout<<"End of while loop";
   return 0;
}

//do while
#include<iostream>
using namespace std;

int main(){
    int i=0;//initalization
    do{
        cout<<i<<endl;
        i++;//increment
    }
    while(i<=100);

    cout<<"End of while loop";
   return 0;
}

//Multiplication table
#include<iostream>
using namespace std;

int main(){

    int num;
        cout<<"Enter any integer number : ";
        cin>>num;

        for(int i=1;i<=10;i++)
        {
            cout<<num<< " X "<< " = "<<(num*i)<<endl;
        }

    cout<<" The  End ";
   return 0;
}

#include<iostream>
using namespace std;
int main()
{
    int sum=0,n;
    cout<<"Enter the last number : ";
    cin>>n;
    cout << "The sum of the sequence 1+2+3+..+" << n << " is: "<<endl;

     for(int i=1;i<=n;i=i+1)
    {
        sum=sum+i;
    }
    cout<<sum;
    return 0;
}




