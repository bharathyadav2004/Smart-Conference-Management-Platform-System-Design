
include <stdio.h>
int main()
{
int n, res;
printf("Enter a number: "); scanf("%d", &n);
if (n >= 1 && n <= 100)
{
res = n * n;
printf("\n Square of %d is %d\n", n, res);
 
}
else if (n<= 0 || n > 100) printf("Beyond the range");

return 0;
}

# Output
Inputs	        Outputs
I1 : -2	      O1 : Beyond the range
I2 : 0	      O2 : Beyond the range
I3 : 1	      O3 : Square of 1 is 1
I4 : 100	  O4 : Square of 100 is 10000 
I5 : 101	  O5 : Beyond the range
I6 : 4	      O6 : Square of 4 is 16
I7 : 62	      O7 : Square of 62 is 3844

