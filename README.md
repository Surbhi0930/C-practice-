## Question:- Write a C program to replace 0 and 1
 Code:
 #include <stdio.h>

int main()

    {

        int num,newnum=0;

        printf("Enter number: ");

        scanf("%d", &num);

        if(num == 0)

            newnum=1;

        while(num>0)

        {

            int rem = num%10;

            if(rem == 0)

                rem = 1;

            num = num/10;

            newnum=newnum*10+rem;

        }

       num = 0 ;

       while(newnum>0)

       {

        int r = newnum%10;

        num= num*10 + r;

        newnum =newnum / 10;

       }

        printf("New number is: %d" ,num);

        return 0;

    }

Explanation: In this Program,we ned to ask the user to enter a input.The code extracts the last digit
from the input usimg a while loop and stores it in a variable called "newnum" .If the last digit obtained is 0 then it is 
converted to 1.


 

        





