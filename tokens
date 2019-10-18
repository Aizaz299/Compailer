#include <iostream>
#include <fstream>
#include <string>
#include <string.h>
#include <istream>
#include <queue>
using namespace std;

enum DataTypes{ Comma, Semicolon, PLUS, MINUS, MULTPLY, DIVIDE, LB, RB,
LP, RP, EQUAL, NOT_EQUAL, GREATER, LESS, NOTHING };

struct TokenRecord
{
DataTypes value; //?
string  stringval;
//int numval;

};
TokenRecord getToken(char ch)
{
TokenRecord obj;

if (ch == ',')
{
obj.value = Comma;
obj.stringval = ch;
return obj;
}
else if (ch == ';')
{

obj.value = Semicolon;
obj.stringval = ch;
return obj;
}
else if (ch == '+')
{

obj.stringval = ch;
obj.value = PLUS;
return obj;
}
else if (ch == '-')
{

obj.stringval = ch;
obj.value = MINUS;
return obj;
}
else if (ch == '/')
{

obj.stringval = ch;
obj.value = DIVIDE;
return obj;
}
else if (ch == '*')
{

obj.stringval = ch;
obj.value = MULTPLY;
return obj;
}
else if (ch == '(')
{

obj.stringval = ch;
obj.value = LB;
return obj;
}
else if (ch == ')')
{

obj.stringval = ch;
obj.value = RB;
return obj;
}
else if (ch == '{')
{
obj.stringval = ch;
obj.value = LP;
return obj;
}
else if (ch == '}')
{
obj.stringval = ch;
obj.value = RP;
return obj;
}
else if (ch == '=')
{
obj.stringval = ch;
obj.value = EQUAL;
return obj;
}
else if (ch == '>')
{
obj.stringval = ch;
obj.value = GREATER;
return obj;
}
else if (ch == '<')
{
obj.stringval = ch;
obj.value = LESS;
return obj;
}
else if (ch == '!')
{
obj.stringval = ch;
obj.value = NOT_EQUAL;
return obj;
}
else
{
obj.stringval = ch;
obj.value = NOTHING;
return obj;
}

obj.value = NOTHING;
return obj;
}



enum seasons { spring , summer, autumn , winter  };
int main()
{




ofstream out;
out.open("codebind.txt");
string str = "";
out << str;  // entering in file
out.close();

ifstream in;
in.open("codebind.txt");
char ch;

TokenRecord obj;

//comment
while (in.get(ch))
{
if (ch == '//')   //how movig forward?
{
in.get(ch);
if (ch == '//')
{
while (ch != '\n') // will get til space and assumed as comment
{
in.get(ch);
}
}
}

//check space taba or new line
if (ch == ' ' || ch == '\t' || ch == '\n')
{
in.get(ch);
}

obj = getToken(ch);  //function call

cout << obj.stringval<< obj.value << endl;

}

system("pause");
return 0;
}
