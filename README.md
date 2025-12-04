# another i made it i guess
```c
#include <stdio.h>
#include <stdbool.h>

int main(){
    // so basically there different types of data, very similar to python (use printf to print)
    int age = 17;
        printf("Hi! I am %d years old.\n", age);
   // be familiar with format specifier, for int or integers: %d, d mean decimal
   // this is how to comment in C, it uses slash
    int aging = 18;
        printf("I am 17 right now, %d tommorow.\n", aging);
    // there is also this thing called float, just like in python it is floating or decimal numbers, there is always 6 to 7 digits after the decimal bur you can change it by %.thenumberyouwantf (%.1f) somethings like that
    float gpa = 94;
        printf("Your gpa is %f\n", gpa);
     // see? now
     float gwa = 94;
         printf("Your gwa is %.1f\n", gwa);
     // there is this thing called double, it is for 15 to digits number after decimal, it like long floating, you can also control the numbers after it
     double pi = 3.14159365265358979;
         printf("The value of pi is %.5lf\n", pi);
     // there is also char, a character or more like strings, it can store SINGLE char
     char initial = 'V';
         printf("Your initial is %c \n", initial);
    // for storing more than value, use char[ ]
      char nameOfCats[] = "Summer and Winter";
          printf("Your cats names are %s \n", nameOfCats);
     // and last boolean, the true and false, the 0 and 1, it needs to have <stdbool.h> on top
     bool isTired = true;
         if (isTired){
             printf("Damn bro you're tired, take a rest");
         }
         else {
             printf("You're getting comfortable");
         }
     
        return 0;
}


// activity for loops

#include <stdio.h>

int main()
{
    // for loops
    
    printf("Activity 4: Repetitive \n");
    printf("------------------------------\n");
    printf("#1 For loop\nProblem: Square of all odd numbers 23-31 \n");
    printf("Answer: \n");
    
    for (int i=23; i<=31; i+=2) {
        printf("%d^2=%d \n",i, i*i);
    }
    
    
    // while loops
    
    printf("------------------------------\n");
    printf("------------------------------\n");
    printf("#2 While loop\nProblem: Sum of all even numbers between 15-25 \n");
    
    int k=16;
    int sum=0; //
    while (k<=25) {
        sum+=k; // to add them
        k+=2; //for da next number to add to sum and whatever the answer will become new sum and then will add again to the next number who are plus 2 from previous 
    }
    printf("Answer: Sum is %d \n", sum);
    
    printf("------------------------------\n");
    printf("------------------------------\n");
    
    
    
    // do while
    
        printf("#3 Do while loop\nProblem: Ask the user for number divisible by 6 \n");
    printf("Answer: \n");
    
        int j;
        
        do {
            printf("Enter a number divisible by 6: ", j);
            scanf("%d", &j);
    // no i++ here because it is not working kapag nakalagay dito 
        } while (j % 6 != 0); // for computation that j is divided by 6 and the answer should not be zero kasi mali na yun
        
        printf("Correct! %d is divisible by 6", j);
        
        
    return 0;
}


// another activity for user input, can't believe i made this

#include <stdio.h>

int main() {
    printf("=============================================\n");
    printf("\t PERSONAL INFORMATION FORM \t\n");
    printf("=============================================\n");
    
    char Fname[20];
    printf("\nEnter your First name: ");
    scanf("%s", Fname);
    
    char Lname[20];
    printf("\nEnter your Last name: ");
    scanf("%s", Lname);
    
    char num[15];
    printf("\nEnter your number: ");
    scanf("%s", num);
    
    printf("\n---------- Date of Birth ---------- \n");
    
    char month[15];
    int day, year;
    
    printf("\nMonth: ");
    scanf("%s", month);
    printf("\nDay: ");
    scanf("%d", &day);
    printf("\nYear: ");
    scanf("%d", &year);
    
    printf("=============================================\n");
    printf("\t PERSONAL INFORMATION \t\n");
    printf("=============================================\n");

    printf("\nName\t\t: %s %s", Fname, Lname);
    printf("\nDate of Birth\t: %s %d, %d", month, day, year);
    printf("\nMobile number\t: %s", num);
    
    return 0;
}
