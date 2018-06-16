#include <stdio.h>
int minpos (float[], int);
main()
{
  int n;
  float smallest;
  int index, i;
  float x[10]= {12.5, 3.0, 45.1, 8.2, 19.3, 10.0, 7.8, 23.7, 29.9, 5.2};
  printf ("Enter the value of n\n");
  scanf ("%d", &n);
  x[0]= smallest;
  for (i=0; i<=n; i++)
  {
    if (x[i]<smallest)
    {
      smallest = x[i];
      index= i;
    }
  }
  printf ("Within the first %d elements of the array, the first minimum value is stored at %d", n, index);
}
