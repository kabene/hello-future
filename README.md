# Hello Future

> On February 2, 2020, GitHub will capture a snapshot of every active public repository, to be preserved in the GitHub Arctic Code Vault. This data will be stored on 3,500-foot film reels, provided and encoded by Piql, a Norwegian company that specializes in very-long-term data storage. The film technology relies on silver halides on polyester. This medium has a lifespan of 500 years as measured by the ISO; simulated aging tests indicate Piql’s film will last twice as long.

## What ?

This is just a dumb repository to store what future generation may remember or want to forget :D

If you had one last piece of code to share, what would it be ?
If you had one last word, what would it be ?

Fill free to star :sparkles: and fork :fork_and_knife: this repository before February 2, 2020 and create your own public version for posterity.

See you in 500 years


## Code for posterity

In 2020, computer still don't know how to use floating numbers :D

```js
0.1 + 0.2 === 0.3 // false
```
## Details
If in 500 years they will forget what's a floating numb or wikipedia shut down or even every computer 'll be quantum:

As the name implies, floating point numbers are numbers that contain floating decimal points. For example, the numbers 5.5, 0.001, and -2,345.6789 are floating point numbers. Numbers that do not have decimal places are called integers.

Computers recognize real numbers that contain fractions as floating point numbers. When a calculation includes a floating point number, it is called a "floating point calculation." Older computers used to have a separate floating point unit (FPU) that handled these calculations, but now the FPU is typically built into the computer's CPU.

## Why in 2020 computer don't know how to use this 

Well, if you have done programming in languages like Java or C, you must be aware of different data types used to store values. The two data types we would be considering in the discussion ahead are integer and float.

Integer data types store whole numbers, while float data types store fractional numbers.

Before we proceed, let’s understand one small concept: How are numbers represented for computational purposes? Very small and very large numbers are usually stored in scientific notation. They are represented as:

Also, a number is normalized when it is written in scientific notation with one nonzero decimal digit before the decimal point. For example, a number 0.0005606 in scientific notation and normalized will be represented as:


Significant is the number of significant digits which do not include zeroes, and base represents the base system used — which is decimal(10) here. Exponent represents the number of places the radix point needs to be moved left or right to be represented correctly.

Now, there are two ways to display numbers in floating point arithmetic: single precision and double precision. Single precision uses 32 bits, and double precision uses 64 bits for floating-point arithmetic.

Unlike many other programming languages, JavaScript does not define different types of numeric data types and always stores numbers as double precision floating point numbers, following the international IEEE 754 standard.

This format stores numbers in 64 bits, where the number (the fraction) is stored in bits 0 to 51, the exponent in bits 52 to 62, and the sign in bit 63.

IEEE754 Double Precision Standard

Let’s represent 0.1 in 64 bit following the IEEE754 standard.

![alt text](https://miro.medium.com/max/670/1*imL6DhMjEkovKn1k78IKfQ.png)
The first step is converting (0.1)base 10 to its binary equivalent (base 2).
To do so, we will start by multiplying 0.1 by 2 and will separate out the digit before the decimal to get the binary equivalent.

![alt text](https://miro.medium.com/max/207/1*z_sj8Rfqx068U7AHoymx9w.png)
On repeating this for 64 bits, we are going to arrange them in ascending order to get our mantissa, which we are going to round off to 52 bits as per the double precision standard.
![alt text](https://miro.medium.com/max/700/1*JN46HCzRJly7YlqwybCoMQ.png)
Mantissa

Representing it in scientific form and rounding off to the first 52 bits will yield:
![alt text](https://miro.medium.com/max/700/1*PLER7zKzNr7nD-SXoApRBw.png)

The mantissa part is ready. Now for the exponent we shall use the below calculation:

![alt text](https://miro.medium.com/max/466/1*ozI1EwDXAdJc-hMHLYL5ig.png)
Here, 11 represents the number of bits we are going to use for 64 bit representation of the exponent, and -4 represents the exponent from the scientific 

The final representation of the number 0.1 is :
![alt text](https://miro.medium.com/max/700/1*Fd8C4frGrb8oaegRkVw7cg.png)

Similarly, 0.2 would be represented as:
![alt text](https://miro.medium.com/max/700/1*-ri9RCDE11ya5dOPRHBtEg.png)
Adding the two after making the exponents same for both would give us:
![alt text](https://miro.medium.com/max/700/1*2UcE_Li_QNaHELT84vDFtQ.png)
When represented in floating point, this becomes:
![alt text](https://miro.medium.com/max/700/0*iu3FdpO09mq1O_jL.png)
This is represented by 0.1 + 0.2.
That is precisely the reason behind getting 0.1 + 0.2 = 0.30000000000000004.

## One last word

"You can't have runtime errors if your code doesn't compile"

## More (if internet is still a thing)
- https://archiveprogram.github.com
- https://en.wikipedia.org/wiki/Floating-point_arithmetic
