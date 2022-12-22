# test-pages
test github pages

```
#include <stdio.h>

/* an array of unspecified size of pointers
 * to functions that return pointers to 
 * functions with a return type of void
 */ 
void (*(*f[])())();
typedef void (*func)();

func func1()
{printf("func1\n");}

func func2()
{printf("func2\n");}

int main()
{
	f[0] = func1;
	f[0]();

	f[0] = func2;
	f[0]();
}
```
