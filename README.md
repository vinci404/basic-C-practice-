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
