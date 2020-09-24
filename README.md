<div align="center">

## Function is left value


</div>

### Description

For anyone who thought that function can only be right value - See this code.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Vitaly](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/vitaly.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |C, C\+\+ \(general\), Microsoft Visual C\+\+
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__3-32.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/vitaly-function-is-left-value__3-988/archive/master.zip)

### API Declarations

```
#include <iostream.h>
```


### Source Code

```
#include <iostream.h>
int &find(int n);
int vect[10]={0,1,17,2,8,25,32,15,48,5};
int main()
{
	int i;
	for(i=0;i<10;i++)
		cout << vect[i] << " ";
	cout << endl;
	find(25)=100;
	for(i=0;i<10;i++)
 		cout << vect[i] << " ";
	cout << endl;
	return 0;
}
int &find(int n)
{
	int i;
	for(i=0;i<10 && vect[i] != n;i++);
		if(n==vect[i])
			return(vect[i]);
		else
			return(vect[0]);
}
```

