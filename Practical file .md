----
# **PROGRAMMING FOR PROBLEM SOLVING ESC-18105**
----
![](https://nptel.ac.in/content/college_assets/college_logo/1078_logo.jpg)
----
## **NAME** -*MANISH KUMAR*
## **ROLL NO.** - *1914143*
## **BRANCH** - *CIVIL*
----
# PROGRAMS
----

## 1. SUM OF TWO NUMBERS
```C
#include <stdio.h>

int main()
{
int firstNumber, secondNumber, sumOfTwoNumbers;
    printf("Enter two integers: ");
    scanf("%d %d", &firstNumber, &secondNumber);
    sumOfTwoNumbers = firstNumber + secondNumber;
    printf("%d + %d = %d", firstNumber, secondNumber, sumOfTwoNumbers);
return 0;
}

----
## 2. AVERAGE OF N NUMBERS
```C
#include<stdio.h>

int main()
{
    int n, i;
    float sum = 0, x;

    printf("Enter number of elements:  ");
    scanf("%d", &n);
    printf("\n\n\nEnter %d elements\n\n", n);
    for(i = 0; i < n; i++)
    {
        scanf("%f", &x);
        sum += x;
    }
    printf("\n\n\nAverage of the entered numbers is =  %f", (sum/n));
    return 0;
}

----
## 3. WEEKDAYS
```C

#include<stdio.h>
int main()
{
int code;
printf("Enter weekdays in number");
scanf("%d",&code);
if(code == 1)
printf("Monday");
else if(code == 2)
printf("Tuesday");
else if(code == 3)
printf("Wednesday");
else if(code == 4) 
printf("Thursday");
else if(code==5)
printf("Friday");
else if(code==6)
printf("Saturday");
else if(code==7)
printf("Sunday");
else
printf("invalid code");
return 0;
}

----
## 4. EVEN ODD CHECK
```C
#include<stdio.h>
void main()
{
        int a;
        printf("enter the number\n");
        scanf("%d",&a);
        if(a%2==0)
                printf("EVEN\n");
        else
                printf("ODD\n");
}
```

----
## 5. TABLE OF ANY NUMBER
```C
#include <stdio.h>
int main()
{
    int n, i;
    printf("Enter an integer: ");
    scanf("%d",&n);
    for(i=1; i<=10; ++i)
    {
        printf("%d * %d = %d \n", n, i, n*i);
    }
    
    return 0;
}

----
## 6. **ARMSTRONG NUMBER
```C
#include<stdio.h>
int main()
{
        int sum=0,digit;
        int n, temp;
        printf("enter any positive integer number");
        scanf("%d",&n);
        temp=n;
        while(temp>0)
        {
                digit=temp%10;
                temp/=10;
                sum=sum+digit*digit*digit;
        }
        if(n==sum)
                printf("\n %d is a armstrong number\n",n);
        else
                printf("\n %d is not a armstrong number\n",n);
}
```

----
## 7. **CALCULATOR DIAGRAM
```C**
#include<stdio.h>


void main()
{
        
        puts(" _______________ ");
        puts("|_______________|");
        puts("| 1 | 2 | 3 |   |");
        puts("|___|___|___|   |");
        puts("| 4 | 5 | 6 | + |");
        puts("|___|___|___|___|");
        puts("| 7 | 8 | 9 | - |");
        puts("|___|___|___|___|");
        puts("|     0     | * |");
        puts("|___________|___|");

}
```
----
## 8. BUBBLE SORT
```C
#include<stdio.h>
int main()
{
        int i,n,k,temp;
        printf("\n enter the array size\n");
        scanf("%d",&n);
        int a[n];
        printf("enter %d elements of array\n",n);
        for(i=0;i<n;i++)
                scanf("%d",&a[i]);
        for(k=0;k<n-1;k++)
        {
                for(i=0;i<n-k-1;i++)
                {
                        if(a[i]>a[i+1])
                        {
                                temp=a[i];
                                a[i]=a[i+1];
                                a[i+1]=temp;
                        }
                }
        }
        printf("\n array elements after shorting\n");
        for(i=0;i<n;i++)
                printf("%d\t",a[i]);
        printf("\n");
}
```

## 9. BINARY SEARCH
```C
#include<stdio.h>
        
int check(int b[],int m,int o)
{       
        int p=-1,mid;
 int f=1,l=m;
 mid=(f+l)/2;           

while(f<=l)
 {
        mid=(f+l)/2;
        if(b[mid]==o)
        {
                p=mid;
                break;
        }
        else if(o>b[mid])
        {
                f=mid+1;
        }
        else if (o<b[mid])
        {
                l=mid-1;
        }
        
}       
                        return p;
        
}     
       
void main()
{       
        int n,num,index;
        printf("enter the array size\n");
        scanf("%d",&n);
        int a[n];
        printf("enter the array elements in assending order\n");
        for(int i=1;i<=n;i++)
        {
                scanf("%d",&a[i]);
        }
        printf("now enter the number which you want to check\n whether it is present or not in entered array\n");
        
        scanf("%d",&num);
        index=check(a,n,num);
        if(index==-1)   
        printf("element is not found\n");
        else
        printf("element is found at the position %d \n",index);

}
```
----
## 10. FACTORIAL OF A NUMBER
```C
              
#include<stdio.h>
int main()
{       
        int n;
        printf("enter number\n");
        scanf("%d",&n);
        int p=1;
        for(int i=1;i<=n;i++)
        {
                p*=i;
        }
        printf("%d! = %d \n",n,p);
}
```
----
##  11. FIZZ-BUZZ
```C
#include<stdio.h>
int main()
{
        for(int i=1;i<=30;i++)
                {
                        if(i%15==0)
                                printf("fizzbuzz\n");
                        else if(i%5==0)
                                printf("buzz\n");
                        else if(i%3==0)
                                printf("fizz\n");
                        else {printf("%d\n",i);}
                }
        return 0;
}
```

----
## 12. SUM OF FIRST 100 NUMBERS
```C
#include<stdio.h>
int main()
{
        int sum=0,i=1;
        while(i<101)
        {
                sum =sum+i;
                i++;
        }
        printf("sum of numbers from 0 to 100 is %d\n",sum);
        return 0;
}
```

----
## 13. FIND GREATER BETWEEN TWO NUMBERS
```C
#include<stdio.h>
void main()
{
int a,b;
printf("Enter any two number");
scanf("%d %d",&a,&b);
if(a>b)
{
printf("a is greater");
}
else
{
printf("b is greater");
}
return 0;
}
```
----
## 14. GREATER AMONG THREE NUMBERS
```C
#include <stdio.h>
int main()
{
    double n1, n2, n3;
    printf("Enter three different numbers: ");
    scanf("%lf %lf %lf", &n1, &n2, &n3);
    if( n1>=n2 && n1>=n3 )
        printf("%.2f is the largest number.", n1);
    if( n2>=n1 && n2>=n3 )
        printf("%.2f is the largest number.", n2);
    if( n3>=n1 && n3>=n2 )
        printf("%.2f is the largest number.", n3);
    return 0;
}
```
----
## 15. GREATEST INTEAGER FUNCTION
```C
#include<stdio.h>
int gcd(int a,int b)
{
        int c;
        c=a%b;
        if(c==0)
                return b;
        else 
                gcd(b,c);
}
int main()
{
        int m,n,c;
        scanf("%d%d",&m ,&n);
        c=gcd(m,n);
        printf("\n gcd is %d \n",c);
        return 0;
}
```
 ----
 ## 16. LEAP YEAR CHECK
 ```C
 #include<stdio.h>
int main()
{
        int a;
        printf("enter the year\n");
        scanf("%d",&a);
        if(a%4==0)
        printf("it is a leap year\n");
        else
                printf("it is not a leap year\n");
}
```
----
## 17. LINEAR SEARCH
```C
#include<stdio.h>

int check(int b[],int m,int o)
{int p=-1;
        for(int i=1;i<=m;i++)
        {
                if(b[i]==o)
                 p = i;
        }

                        return p;
        
}

#include <stdio.h>
void main()
{
    int a[10], i, item;
    printf("\nEnter SEVEN elements of an array:\n");
    for (i=0; i<=6; i++)
        scanf("%d", &a[i]);
    printf("\nEnter item to search: ");
    scanf("%d", &item);
    for (i=0; i<=9; i++)
        if (item == a[i])
        {
            printf("\nItem found at location %d", i+1);
            break;
        }
    if (i > 9)
        printf("\nItem does not exist.");
    getch();
}
```
----
##  18. SUM OF TWO MATRIX
```C
#include<stdio.h>       
int main()                      
{                       
        int m,n,o,p,i,j;
        printf("enter the number of rows and columns of matries \n");
        scanf("%d %d",&m,&n);
        int a[m][n] , b[m][n] , c[m][n];
        {               
                printf("enter the elements of first matrix\n");
                for(i=0;i<m;i++)
                {       
                        for(j=0;j<n;j++)
                        {
                                scanf("%d",&a[i][j]);
                        }
                }       
                printf("enter the elements of second matrix\n");
                for(i=0;i<m;i++)
                {               
                        for(j=0;j<n;j++)
                        {
                                scanf("%d",&b[i][j]);
                        }
                }
                printf("the elements of first matrix is \n");
                for(i=0;i<m;i++)
                {               
                        for(j=0;j<n;j++)
                        {
                                printf("%d ",a[i][j]);
                        }
                        printf("\n");
                }
                   printf("the elements of second matrix is \n");
                for(i=0;i<m;i++)
                {       
                        for(j=0;j<n;j++)
                        {       
                                printf("%d ",b[i][j]);
                        }
                        printf("\n");
                }
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                {
                                        c[i][j]=a[i][j]+b[i][j];
                                
                                }
                        }
                }
                      
                printf("sum of given matrices is\n");
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                printf("%d ",c[i][j]);
                        }       
                        printf("\n");
                }       
        }       
                
}               
                        
```


----
## 19. TRANSPOSE MATRIX
```C
#include<stdio.h>
int main()
{ 
        int m,n,i,j;
        printf("enter the number of rows and columns of matrix\n");
        scanf("%d%d",&m,&n);
        int a[m][n],b[m][n] ;
                printf("enter the elements of  matrix row wise\n");
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                scanf("%d",&a[i][j]);
                        }       
                }       
                
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                b[j][i]=a[i][j];
                        }       
                }       
                printf("transpose  of matrix is \n");
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                printf("%d ",b[i][j]);
                        }       
                        printf("\n");
                }       
}               
```
----
## 20. SUM OF DIGITS OF A NUMBER
```C
#include<stdio.h>
int main()
{
        int a,sum=0,c;
        printf("enter the number\n");
        scanf("%d",&a);
        while(a!=0)
        {
        c=a%10;
        sum+=c;
        a=a/10;
        }
        printf("sum of digits is %d\n",sum);
}
```
----
## 21. CHECK PALINDROME NUMBER
```C
#include<stdio.h>
int main()
{
        int sum=0,digit;
        int n, temp;
        printf("enter any positive integer number\n");
        scanf("%d",&n);
        temp=n;
        while(temp>0)
        {
                digit=temp%10;
                temp/=10;
                sum=sum*10+digit;
        }
        if(n==sum)
                printf("\n %d is a palidrome number\n",n);
        else
                printf("\n %d is not a palidrome number\n",n);
}
```
 ----
 ## 22. CALL BY VALUE
 ```C
 #include<stdio.h>
void swap(int a,int b);
void main()
{
int x,y;
printf("\n Enter value for x:");
scanf("%d",&x);
printf("\n Enter value for y:");
scanf("%d",&y);
printf("\n Before calling swap functin\n");
printf("\n Value of x=%d,Value of y=%d\n",x,y);
swap(x,y);
printf("\n After returning from swap function");
printf("\n Value of x=%d,value of y=%d\n",x,y);
}
void swap(int a,int b)
{
int temp;
printf("\n Inside the function \n");
printf("\n Value of a=%d,Value of b=%d before swaping\n",a,b);
temp=a;
a=b;
b=temp;
printf("\n Value of a=%d,Value of b=%d after swaping\n",a,b);
}
```
----
## 23. CALL BY REFERENCE
```C
#include<stdio.h>
void swap(int *,int *);
void main()
{
int x,y;
printf("\n Enter value for x:");
scanf("%d",&x);
printf("\n Enter value for y:");
scanf("%d",&y);
printf("\n Before calling swap functin\n");
printf("\n Value of x=%d,Value of y=%d\n",x,y);
swap(&x,&y);
printf("\n After returning from swap function");
printf("\n Value of x=%d,value of y=%d\n",x,y);
}
void swap(int *a,int *b)
{
int temp;
printf("\n Inside the function \n");
printf("\n Value of a=%d,Value of b=%d before swaping\n",*a,*b);
temp=*a;
*a=*b;
*b=temp;
printf("\n Value of a=%d,Value of b=%d after swaping\n",*a,*b);
}
```
----
## 24. EMPLOYEE DETAILS USING STRUCTURE
```C
#include<stdio.h>
#include<string.h>
struct employee
{
        int code;
        char name[20];
        char department[20];
        float salary;
};
void main()
{
        struct employee e;
        printf("enter employee code\n");
        scanf("%d",&e.code);
        printf("enter employee name\n");
        scanf("%s",&e.name);
        printf("enter employee department\n");
        scanf("%s",&e.department);
        printf("enter employee salary\n");
        scanf("%f",&e.salary);
        printf("information about employee is \n");
        printf("Employee code: %d \n",e.code);
        printf("Employee name: %s \n",e.name);
        printf("Employee department: %s \n",e.department);
        printf("Employee salary: %f \n",e.salary);
}
```
----
## 25. FRACTION PRODUCT USING STRUCTURE
```C
#include<stdio.h>
struct fraction
{
        int num;
        int den;
};
void main()
{
        int rnum,rden;
        struct fraction f1,f2;
        printf("enter numerator and denominator of first fraction\n");
        scanf("%d%d",&f1.num,&f1.den);
        printf("enter numerator and denominator of second fraction\n");
        scanf("%d%d",&f2.num,&f2.den);  
        rnum=f1.num*f2.num;
        rden=f1.den*f2.den;
        printf("\nproduct is : %d/%d\n",rnum,rden);
}
```

