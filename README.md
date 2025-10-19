# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```

#include <stdio.h>

int main() {
    int a=44,b=3;
    int res= a << b;
    printf("Result of Left shift of 44 for 3 times is %d",res);

    return 0;
}
```
## OUTPUT

<img width="1463" height="399" alt="image" src="https://github.com/user-attachments/assets/b63d80f9-2d5b-42c4-aa68-8d49615f032e" />








## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```

#include <stdio.h>

int main() {
    int a,b;
    
    printf("Enter two numbers for comparsion:\n");
    scanf("%d %d",&a,&b);
    if(a==b){
        printf("Both Numbers are eqaul!");
    }else{
        printf("Both numbers are not equal.");
    }

    return 0;
}
```

## OUTPUT
 <img width="506" height="244" alt="image" src="https://github.com/user-attachments/assets/a1d2e46e-36a3-43c5-819b-9e922d14f585" />
  <img width="449" height="248" alt="image" src="https://github.com/user-attachments/assets/bd4c46d1-ef04-4e09-9bbf-3313c969f74d" />

## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <string.h>
#include <ctype.h>
#include <stdio.h>

int main() {
    char str[100];
    printf("Enter your string:\n");
    scanf("%[^\n]s",str);
    for(int i=0;i<strlen(str);i++){
        if(isspace(str[i])){
            continue;
        }else{
            str[i]=tolower(str[i]);
        }
    }
    printf("The string after converting to lower case is: %s",str);
    
}
```
## OUTPUT

<img width="1676" height="339" alt="image" src="https://github.com/user-attachments/assets/e4fb9d77-bb70-45fc-b9ee-df8beba087cb" />



## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <string.h>
#include <ctype.h>
#include <stdio.h>

int main() {
    char str[100];
    printf("Enter your string:\n");
    scanf("%[^\n]s",str);
    int i=0,count=0;
    do{
        if(isspace(str[i])){
            count++;
        }
        i++;
    }while(i<strlen(str));
    printf("The number of words in the string is: %d",count+1);
    
}
```
## OUTPUT
<img width="1467" height="313" alt="image" src="https://github.com/user-attachments/assets/55a82377-3b56-4e3b-be63-62888ea18f48" />





## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
#include <string.h>
#include <ctype.h>
#include <stdio.h>

int main() {
    char str1[100], str2[100];
    printf("Enter your first string:\n");
    scanf("%[^\n]s", str1);

    printf("\nEnter your second string:\n");
    scanf(" %[^\n]s", str2); 

    int i = 0, flag = 1;
    while (str1[i] != '\0' || str2[i] != '\0') {
        if (str1[i] != str2[i]) {
            flag = 0;
            break;
        }
        i++;
    }

    if (flag == 1) {
        printf("\nThe strings are same.\n");
    } else {
        printf("\nThe strings are not same.\n");
    }

    return 0;
}

```

## OUTPUT
 <img width="1428" height="339" alt="image" src="https://github.com/user-attachments/assets/9a28e243-b71f-44f0-9a3d-7335d919494c" />


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

