# pattern-with-4loops-and-rows-input-frm-user.c
// Online C compiler to print pattern with given rows // example enter no. of rows=6  ABCDEFEDCBA  BCDEFEDCB   CDEFEDC    DEFED     EFE      F    
// Online C compiler to print pattern with given rows
// example enter no. of rows=6

ABCDEFEDCBA
 BCDEFEDCB
  CDEFEDC
   DEFED
    EFE
     F
     
#include <stdio.h>
int main() {
    int i,j,n;
    printf("enter rows=");
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        for(j=0;j<=i-1;j++)
         printf(" ");
        for(j=i;j<=n-1;j++)
         printf("%c",65+j);
        for(j=n-2;j>=i;j--)
         printf("%c",65+j);
        printf("\n");
    }
    return 0;
}
