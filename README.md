#include <stdio.h> 
main() { int A[50]; int VAL, POS, N, I; 
 /* Data entry */ 
 do {printf("Enter the table dimension (max = 50): "); 
 scanf("%d", &N );} 
 while ((N < 1) || (N > 50)); 
 for (I=0; I<N; I++) { 
 printf("A[%d] : ", I); 
 scanf("%d", &A[I]); 
 } 
 printf("Give an element to search for: "); 
 scanf("%d", &VAL ); 
 
 /* Searching for position of the value */ 
 POS = -1; 
 for (I=0 ; (I<N); I++) 
 if (A[I]==VAL){ POS=I; 
 printf("The value %d is located at the position %d. 
\n", VAL, POS); 
 } 
 if (POS==-1) 
 printf("The value you are looking for is not exist in 
the table.\n"); 
 system("pause"); 
 return 0; 
 }
