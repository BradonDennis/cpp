# Bug 1

1. **The incorrect original code or code snippit that you wrote:**

#include <iostream>
using namespace std;

int main() {
    int i, n;
    bool isPrime = true; // this allows to call towards the if/else funtion to test to see if the numbers are prime.

    cout << "Enter a positive integer: ";
    cin >> n; // calls the user to type a number

    // 0 and 1 are not prime numbers
    if (n == 0 || n == 1) { //we first check if the input number is one of those numbers or not. If the input number is either 0 or 1, then the value of isPrime is set to false.
        isPrime = false;
    }
    else {
        for (i = 2; i <= n / 2; ++i) { // tests to see if any adding integer is able to divide into a full number.
            if (n % i == 0) { 
                isPrime = false;
                break;
                } // If the number entered by the user is perfectly divisible by i, then isPrime is set to false and the number will not be a prime number.
             }
          }
    if (isPrime)
        cout << n << " is a prime number"; //displays when isprime is true
    else
        cout << n << " is not a prime number\n";
        //displays when isprime is false
    return 0;
}

2. **What bug does the original code have?**

//  We do not obtain how the true/false value has been achieved.

3. **What misunderstanding of C++ concepts lead you to this incorrect code?**

//  Not adding in a cout to share the integers the code finds.

4. **How to correct the bug?**

//  Add in a cout sharing the said number

5. **The corresponding bug-free code or code snippet is:**

#include <iostream>
using namespace std;

int main() {
    int i, n;
    bool isPrime = true; // this allows to call towards the if/else funtion to test to see if the numbers are prime.

    cout << "Enter a positive integer: ";
    cin >> n; // calls the user to type a number

    // 0 and 1 are not prime numbers
    if (n == 0 || n == 1) { //we first check if the input number is one of those numbers or not. If the input number is either 0 or 1, then the value of isPrime is set to false.
        isPrime = false;
    }
    else {
        for (i = 2; i <= n / 2; ++i) { // tests to see if any adding integer is able to divide into a full number.
            if (n % i == 0) { 
                isPrime = false;
                break;
                } // If the number entered by the user is perfectly divisible by i, then isPrime is set to false and the number will not be a prime number.
             }
          }
    if (isPrime)
        cout << n << " is a prime number"; //displays when isprime is true
    else
        cout << n << " is not a prime number\n";
        //displays when isprime is false
        cout << "The number you gave can be divided by " << i; // shares the exact lowest number the number can be divided by to disprove it being a prime.
    return 0;
}

6. **What is the take-away message from this bug?**

---

# Bug 2

1. **The incorrect original code or code snippit that you wrote:**

```
code with bugs or code snippet with bug goes here

```

2. **What bug does the original code have?**

  

3. **What misunderstanding of C++ concepts lead you to this incorrect code?**

4. **How to correct the bug?**

5. **The corresponding bug-free code or code snippet is:**

```
bug-free code or code snippet goes here

```

6. **What is the take-away message from this bug?**

---

# Bug 3

1. **The incorrect original code or code snippit that you wrote:**

```
code with bugs or code snippet with bug goes here

```

2. **What bug does the original code have?**

  

3. **What misunderstanding of C++ concepts lead you to this incorrect code?**

4. **How to correct the bug?**

5. **The corresponding bug-free code or code snippet is:**

```
bug-free code or code snippet goes here

```

6. **What is the take-away message from this bug?**
