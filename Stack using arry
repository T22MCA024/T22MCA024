#include<stdio.h>
#define size 5
struct stack
{
	int a[10];
	int top;
};
struct stack push(struct stack,int);
int pop(struct stack*);
void display(struct stack);
 int main()
{
	 
	 struct stack s;
	 int ele,ch ;
	 s.top=-1;
	 do
	 {
	 	printf("1.push an element:\n 2. pop of an element: 3. display element:\n 4.exit\n");
	 	scanf("%d",&ch);
	  switch(ch)
	 {
	 	 case 1 : s = push(s,ele);
	 	          break;
	 	case 2  :ele=pop(&s);
	 	         break;
	 	case 3 : display(s);
	 	          break;
	 	case 4: printf("exit from loop");
	 	           break;
	 	default:printf("enter correct choice");
	 	            break;
	 	}
	 	printf("\n");
	 }
	 while(ch<=4);
}
struct stack push(struct stack s,int ele)
{
	printf("enter new element");
	scanf("%d",&ele);
    if(s.top<(size-1))
    {
    	s.top++;
    	s.a[s.top]=ele;
    }
    else
    {
    	printf("over flow");
    }
    printf("top value index:\n",s.top);
    return s;
    }
    int pop(struct stack *s)
    {
    	int ele;
    	if(s->top==-1)
    	{
    		printf("over flow");
    	}
    	else
    	{
    		ele=s->a[s->top];
    		s->top--;
    		printf("eliminated element=%d",ele);
    		
    	}
    	printf("now top is at the index of a[%d]\n",s->top);
    	return ele;
    	}
    	void display(struct stack s)
    	{
    		int i;
    		if(s.top==-1)
    		{
    			printf("stack is empty\n");
    		}
    		else
    		{
    			for(i=s.top;i>=0;i--)
    			{
    				printf("a[%d]=%d\n",i,s.a[i]);
    			}
    		}
    	}
	



