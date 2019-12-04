#include<string.h>
#include <stdio.h>
#include<stlib.h>
char *mid(char src[],int start,int num)
{
    if(start>strlen(src))
    printf("error");
    else
    {
        char *p=calloc(num,sizeof(src[0]));
        int i=0;
        for(;i<num;i++)
        p[i]=src[i+start-1];
        p[i]='\0';
        return p;
    }
}
int main()
{
    int start,num;
    char *s;
    printf("daal!\n");
    scanf("%s",s);
    printf("kaha se kitna?");
    scanf("%d %d",&start,&num);
    printf("%s",mid(s,start,num));
    return 0;
}
