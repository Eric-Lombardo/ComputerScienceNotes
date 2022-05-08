# COMP228

## Week 1 (binary decimal, hexadecimal, floating-point)

- A bit is the most basic unit of information in a computer
- a byte is a group of 8 bits
  - The smallest adressable (able to be accessed by memory)
- "0x" represents hexadecimal (base 16)
- **Positive numbers are true binary**

### Excess-M
- typically used for floating point representation
- in excess-m (also called **offset** binary representation) if we have 4 biuts, we then choose the middle as our "base" and any number below/above this base will be -ve or +ve. This ensures an equal bumber of +ve and -ve values
```
-7   0000 (0)
... 
-1   0110 (6)
0    0111 (7 "base")
+1   1000 (8)
...
+8   1111 (15)


2^(n-1) - 1 = base (where n is amount of bits)
2^(4-1) - 1 = 7 (in the example above)

```

![](/images/week1/convert-binary-to-decimal.png)
![](/images/week1/base-ten-numbering-system.png)
![](/images/week1/base-tw0-numbering-system.png)
![](/images/week1/convert-decimal-to-binary.png)
![](/images/week1/counting-in-hexadecimal.png)
![](/images/week1/counting-dec-bin-hexa.png)
![](/images/week1/convert-hexa-to-dec.png)
![](/images/week1/convert-dec-to-hexa.png)
![](/images/week1/convert-hexa-to-bin.png)
![](/images/week1/convert-bin-to-hexa.png)
![](/images/week1/octal-to-bin.png)
![](/images/week1/integer-representation.png)
![](/images/week1/add-signed-mag.png)
![](/images/week1/add-signed-mag-overflow.png)
![](/images/week1/sub-signed-mag.png)
![](/images/week1/sub-neg-signed-mag.png)
![](/images/week1/sub-neg2-signed-mag.png)
![](/images/week1/sign-mag-problems.png)
![](/images/week1/one-complement.png)
![](/images/week1/one-complement2.png)
![](/images/week1/one-complement3.png)
![](/images/week1/two-complement.png)
![](/images/week1/two-complement2.png)
![](/images/week1/two-complement3.png)
![](/images/week1/two-complement4.png)
![](/images/week1/overflow.png)
![](/images/week1/unsigned-int-range.png)
![](/images/week1/unsigned-int-range2.png)
![](/images/week1/signed-int-range.png)
![](/images/week1/signed-int-range2.png)
![](/images/week1/floating-point.png)
![](/images/week1/floating-point-add.png)
![](/images/week1/floating-point-multiply.png)
![](/images/week1/floating-point-ieee.png)
![](/images/week1/floating-point-sum.png)
![](/images/week1/floating-point-multi.png)
![](/images/week1/floating-point-epsilon.png)
![](/images/week1/fraction-conversion.png)
![](/images/week1/booths-algo.png)
![](/images/week1/carry-vs-overflow.png)
![](/images/week1/multi-div-by-two.png)
![](/images/week1/multi-div-by-two2.png)
![](/images/week1/multi-div-by-two3.png)
![](/images/week1/character-codes.png)
![](/images/week1/conclusion.png)
