# Water_Mixing
-----------------------------------------------------------------------
/*#include <stdio.h>

int main(void) {
	int t,n,x,y,z,count,i,j,a,b,c;
	scanf("%d",&t);
	while(t--)
	{
	  scanf("%d %d %d %d",&a,&b,&x,&y);
    c=a+x;
    i=a-y;
	  if((a==b)||(b<c)||(b>i))
    {
      printf("YES\n");
    }
    else 
    {
      printf("NO\n");
    }
	}
	return 0;
}*/
--------------------------------------------------------------------------
#include <stdio.h>
#include <stdlib.h>
int main(void) {
	int t,n,x,y,z,temp,count,i,j,a,b,c;
	scanf("%d",&t);
	while(t--)
	{
	  scanf("%d %d %d %d",&a,&b,&x,&y);
    temp=a-b;
    if(temp==0){
        printf("YES\n");
      }
    else if(temp<0)
    {
      if(abs(temp)<=x){
        printf("YES\n");
      }
      else{
        printf("NO\n");
      }
    }
    else{
      if(abs(temp)<=y){
        printf("YES\n");
        }
      else{
        printf("NO\n");
      }
    }
  }
	return 0;
}
