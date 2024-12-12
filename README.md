# Mixed Precision Training
Mixed precision is a computing approach that uses a combination of multiple numerical precisions such as FP-16(half precision), FP-32(single-precision), FP-64(double precision)

## Why mixed precision training or mixed precision in general
Lower precision needs less memory to train more extensive networks. As a result, the training process is more efficient since it takes less memory bandwidth. Finally, the lower the precision, the speedier the mathematical operations may be carried out.
Shorten the training or inference time. 

## Dealing with quantization loss
Loss scaling is used to preserve small gradient values.

## Terminology
## Mantissa (Significand)
The mantissa represents the significant digits of a number in scientific notation. It determines the precision of the floating-point format.
   Precision and the Mantissa.
     ### The number of bits allocated to the mantissa decides how many significant figures the format can store.
     ### More bits = higher precision, meaning numbers can be represented with greater accuracy.

## Exponent

