#include <stdio.h>
#define MAXLEN 100

typedef struct {

    int element[MAXLEN];
    int top;

}stack;


stack init()
{
    stack S;
    S.top=-1;
    return S;
}

int isEmpty(stack S)
{
    if(S.top==-1)
        return 1;
    else
        return 0;
}

int isFull(stack S)
{
    if(S.top==MAXLEN-1)
        return 1;
    else
        return 0;
}

int top (stack S)
{
 if (isEmpty(S))
    printf("Empty stack n");
 else
    return S.element[S.top];
}

stack push(stack S,int x)
{
    if(isFull(S))
    {
        printf("OVERFLOW\n");;
    }
    else{
        ++S.top;
        S.element[S.top]=x;
    }
    return S;
}


stack pop(stack S)
{
    if(isEmpty(S))
    {
        printf("UNDERFLOW\n");
    }
    else{
        --S.top;
    }
    return S;
}

void print (stack S)
{
int i;
for (i=S.top; i>=0; i--)
printf("%d ",S.element[i]);
}



int main ()
{   int choice=0;
    stack S;
    S=init();
    printf("*********Stack operations using array*********");

printf("\n----------------------------------------------\n");
    while(choice != 4)
    {
        printf("Chose one from the below options...\n");
        printf("\n1.Push\n2.Pop\n3.Show\n4.Exit");
        printf("\n Enter your choice \n");
        scanf("%d",&choice);
        switch(choice)
        {
            case 1:
            {   int el;
                printf("Enter an element to enter into stack \n");
                scanf("%d",&el);
                S=push(S,el);
                break;
            }
            case 2:
            {
                S=pop(S);
                break;
            }
            case 3:
            {
                print(S);
                break;
            }
            case 4:
            {
                printf("Exiting....");
                break;
            }
            default:
            {
                printf("Please Enter valid choice ");
            }
        };
    }
}
