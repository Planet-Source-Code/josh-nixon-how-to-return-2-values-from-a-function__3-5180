<div align="center">

## How to return 2 values from a function


</div>

### Description

Will return 2 values from a function by passing 2 variables by reference.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Josh Nixon](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/josh-nixon.md)
**Level**          |Beginner
**User Rating**    |4.6 (23 globes from 5 users)
**Compatibility**  |C\+\+ \(general\)
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__3-32.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/josh-nixon-how-to-return-2-values-from-a-function__3-5180/archive/master.zip)

### API Declarations

```
#include <iostream.h>
#include <conio.h>
```


### Source Code

```
#include <iostream.h>
#include <conio.h>
short Math_Stuff(int, int*, int*);
int main()
{
 int Num = 0, MCube = 0, MSquared = 0;
 short Error;
  clrscr();
  cout<<"Enter in number to square and cube: ";
  cin>>Num;
   Error = Math_Stuff(Num, &MCube, &MSquared);
   if(!Error)
    {
	cout<<"The number is: "<<Num;
	cout<<endl<<"The cube of "<<Num<<": "<<MCube;
	cout<<endl<<"The square of "<<Num<<": "<<MSquared;
	getch();
    }
   else
    cout<<"An error has occured";
return 0;
}
short Math_Stuff(int N, int *Cube, int *Sqaured)
{
 short Value = 0;
  if(N > 20)
  Value = 1;
  else
  *Sqaured = (N*N);
  *Cube = (N*N*N);
  Value = 0;
  return Value;
}
```

