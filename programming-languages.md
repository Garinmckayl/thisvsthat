# Programming Languages

Table of Contents
=================

   * [C vs C++](#C-vs-C++)
      * [Code Comparison](#Code-Comparison-C-vs-C++)
   * [Python vs C++](#Python-vs-C++)
      * [Code Comparison](#Code-Comparison-Python-vs-C++)
   * [Python vs Java](#Python-vs-Java)
      * [Code Comparison](#Code-Comparison-Python-vs-Java)
   * [Javascript vs Python](#Javascript-vs-Python)
      * [Code Comparison](#Code-Comparison-Javascript-vs-Python)
   * [Javascript vs Java](#Javascript-vs-Java)
      * [Code Comparison](#Code-Comparison-Javascript-vs-Java)
   * [Html vs Markdown](#Html-vs-Markdown)
      * [Code Comparison](#Code-Comparison-Html-vs-Markdown)
## C vs C++

C and C++ are somehow similar languages, C++ released as extension for C programming language. 

C is a general-purpose, procedural computer programming language.
C++ is a high-level programming language, C++ adds object-oriented features to its predecessor, C.

### Code Comparison C vs C++

#### **Print Hello World**

<!-- tabs:start -->

#### ** C **

```clike
#include <stdio.h>
int main() {
   // printf() displays the string inside quotation
   printf("Hello, World!");
   return 0;
}
```

#### ** C++ **

```clike
#include <iostream>

int main() {
    std::cout << "Hello World!";
    return 0;
}
```

<!-- tabs:end -->

#### **Display Fibonacci Series**

<!-- tabs:start -->

#### ** C  **

```clike
#include<stdio.h>
int main()
{
    int count, first_term = 0, second_term = 1, next_term, i;
 
    //Ask user to input number of terms 
    printf("Enter the number of terms:\n");
    scanf("%d",&count);
 
    printf("First %d terms of Fibonacci series:\n",count);
    for ( i = 0 ; i < count ; i++ )
    {
       if ( i <= 1 )
          next_term = i;
       else
       {
          next_term = first_term + second_term;
          first_term = second_term;
          second_term = next_term;
       }
       printf("%d\n",next_term);
    }
 
    return 0;
}
```

#### ** C++ **

```clike
#include <iostream>  
using namespace std;  
int main() {  
  int n1=0,n2=1,n3,i,number;    
 cout<<"Enter the number of elements: ";    
 cin>>number;    
 cout<<n1<<" "<<n2<<" "; //printing 0 and 1    
 for(i=2;i<number;++i) //loop starts from 2 because 0 and 1 are already printed    
 {    
  n3=n1+n2;    
  cout<<n3<<" ";    
  n1=n2;    
  n2=n3;    
 }    
   return 0;  
   }  
```

<!-- tabs:end -->


#### **Check if number is palindrome**

<!-- tabs:start -->

#### ** C  **

```clike
#include <stdio.h>
int main()
{
   int num, reverse_num=0, remainder,temp;
   printf("Enter an integer: ");
   scanf("%d", &num);

   /* Here we are generating a new number (reverse_num)
    * by reversing the digits of original input number
    */
   temp=num;
   while(temp!=0)
   {
      remainder=temp%10;
      reverse_num=reverse_num*10+remainder;
      temp/=10;
   } 

   /* If the original input number (num) is equal to
    * to its reverse (reverse_num) then its palindrome
    * else it is not.
    */ 
   if(reverse_num==num) 
      printf("%d is a palindrome number",num);
   else
      printf("%d is not a palindrome number",num);
   return 0;
}
```

#### ** C++ **

```clike
#include <iostream>  
using namespace std;  
int main()  
{  
  int n,r,sum=0,temp,num;    
  cout<<"Enter the Number=";    
  cin>>n;    
 temp=n;
 num=n;
 while(n>0)    
{    
 r=n%10;    
 sum=(sum*10)+r;    
 n=n/10;    
}    
if(temp==sum)    
cout<<num<<" is Palindrome.";    
else    
cout<<num<<"is not Palindrome.";   
  return 0;  
}
```

<!-- tabs:end -->






















## Python vs C++

Python is an interpreted, high-level and general-purpose programming language. 

C++ is a high-level programming language, C++ adds object-oriented features to its predecessor, C.


### Code Comparison Python vs C++

#### **Print Hello World**


<!-- tabs:start -->

#### ** Python **

```clike
print("Hello, World!")
```

#### ** C++ **

```clike
#include <iostream>

int main() {
    std::cout << "Hello World!";
    return 0;
}
```

<!-- tabs:end -->

#### **Display Fibonacci Series**


<!-- tabs:start -->

#### ** Python  **

```clike

nterms = int(input("How many terms you want? "))  
# first two terms  
n1 = 0  
n2 = 1  
count = 2  
# check if the number of terms is valid  
if nterms <= 0:  
   print("Please enter a positive integer")  
elif nterms == 1:  
   print("Fibonacci sequence:")  
   print(n1)  
else:  
   print("Fibonacci sequence:")  
   print(n1,",",n2,end=', ')  
   while count < nterms:  
       nth = n1 + n2  
       print(nth,end=' , ')  
       # update values  
       n1 = n2  
       n2 = nth  
       count += 1  
}
```

#### ** C++ **

```clike
#include <iostream>  
using namespace std;  
int main() {  
  int n1=0,n2=1,n3,i,number;    
 cout<<"Enter the number of elements: ";    
 cin>>number;    
 cout<<n1<<" "<<n2<<" "; //printing 0 and 1    
 for(i=2;i<number;++i) //loop starts from 2 because 0 and 1 are already printed    
 {    
  n3=n1+n2;    
  cout<<n3<<" ";    
  n1=n2;    
  n2=n3;    
 }    
   return 0;  
   }  
```

<!-- tabs:end -->



#### **Check if number is palindrome**

<!-- tabs:start -->

#### ** Python  **

```clike
num = int(input("enter a number: "))
 
temp = num
rev = 0

 # reversed integer is stored in variable rev
while temp != 0:
    rev = (rev * 10) + (temp % 10)
    temp = temp // 10
 
if num == rev:
    print(num,"number is palindrome")
else:
    print(num,"number is not palindrome")
```

#### ** C++ **

```clike
#include <iostream>  
using namespace std;  
int main()  
{  
  int n,r,sum=0,temp,num;    
  cout<<"Enter the Number=";    
  cin>>n;    
 temp=n;
 num=n;
 while(n>0)    
{    
 r=n%10;    
 sum=(sum*10)+r;    
 n=n/10;    
}    
if(temp==sum)    
cout<<num<<" is Palindrome.";    
else    
cout<<num<<"is not Palindrome.";   
  return 0;  
}
```

<!-- tabs:end -->































## Python vs Java

Python is an interpreted, high-level and general-purpose programming language. 

Java is a class-based, object-oriented programming language that is designed to have as few implementation dependencies as possible.


### Code Comparison Python vs Java

#### **Print Hello World**


<!-- tabs:start -->

#### ** Python **

```clike
print("Hello, World!")
```

#### ** Java **

```clike
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```

<!-- tabs:end -->

#### **Display Fibonacci Series**


<!-- tabs:start -->

#### ** Python  **

```clike

nterms = int(input("How many terms you want? "))  
# first two terms  
n1 = 0  
n2 = 1  
count = 2  
# check if the number of terms is valid  
if nterms <= 0:  
   print("Plese enter a positive integer")  
elif nterms == 1:  
   print("Fibonacci sequence:")  
   print(n1)  
else:  
   print("Fibonacci sequence:")  
   print(n1,",",n2,end=', ')  
   while count < nterms:  
       nth = n1 + n2  
       print(nth,end=' , ')  
       # update values  
       n1 = n2  
       n2 = nth  
       count += 1  
}
```

#### ** Java **

```clike
class FibonacciExample1{  
public static void main(String args[])  
{    
 int n1=0,n2=1,n3,i,count=10;    
 System.out.print(n1+" "+n2);//printing 0 and 1    
    
 for(i=2;i<count;++i)//loop starts from 2 because 0 and 1 are already printed    
 {    
  n3=n1+n2;    
  System.out.print(" "+n3);    
  n1=n2;    
  n2=n3;    
 }    
  
}}   
```

<!-- tabs:end -->




#### **Check if number is palindrome**

<!-- tabs:start -->

#### ** Python  **

```clike
num = int(input("enter a number: "))
 
temp = num
rev = 0

 # reversed integer is stored in variable rev
while temp != 0:
    rev = (rev * 10) + (temp % 10)
    temp = temp // 10
 
if num == rev:
    print(num,"number is palindrome")
else:
    print(num,"number is not palindrome")
```

#### ** Java **

```clike
public class Palindrome {

    public static void main(String[] args) {

        int num = 121, reversedInteger = 0, remainder, originalInteger;

        originalInteger = num;

        // reversed integer is stored in variable 
        while( num != 0 )
        {
            remainder = num % 10;
            reversedInteger = reversedInteger * 10 + remainder;
            num  /= 10;
        }

        // palindrome if originalInteger and reversedInteger are equal
        if (originalInteger == reversedInteger)
            System.out.println(originalInteger + " is a palindrome.");
        else
            System.out.println(originalInteger + " is not a palindrome.");
    }
}
```

<!-- tabs:end -->





















## Javascript vs Python

Javascript is a programming language mainly use in browser, but now-a-days it is being use everywhere on the server, on Iot devices. 

Python is an interpreted, high-level and general-purpose programming language.


### Code Comparison Javascript vs Python




<!-- tabs:start -->

#### ** JavaScript **

```html

```

#### ** Java **


```markup

```

<!-- tabs:end -->















## Javascript vs Java


Java is a class-based, object-oriented programming language that is owned by Oracle. 


### Code Comparison Javascript vs Java



<!-- tabs:start -->

#### ** JavaScript **

```html

```

#### ** Java **


```markup

```

<!-- tabs:end -->








## Html vs Markdown

HTML (HyperText Markup Language) is the most basic building block of the Web. 

Markdown is a lightweight markup language with plain-text-formatting syntax.



### Code Comparison Html vs Markdown



<!-- tabs:start -->

#### ** Html **

```html
<h3>Html Page</h3>

<p>This is a simple paragraph with <a href="https://example.com">link</a>.</p>

<h1>Big Header</h1>

<pre><code class="language-js">
var turndownService = new TurndownService()
console.log(
  turndownService.turndown('&lt;h1&gt;Hello world&lt;/h1&gt;')
)</code></pre>

<hr />

<ul>
  <li>List One</li>
  <li>List Two</li>
</ul>
```

#### ** Markdown **

```markup
### Html Page

This is a simple paragraph with [link](https://example.com).

Big Header
==========

    
    var turndownService = new TurndownService()
    console.log(
      turndownService.turndown('<h1>Hello world</h1>')
    )

* * *

*   List One
*   List 
```

<!-- tabs:end -->