# Mixed Precision Training
Mixed precision is a computing approach that uses a combination of multiple numerical precisions such as FP-16(half precision), FP-32(single-precision), FP-64(double precision)

## Why mixed precision training or mixed precision in general
Lower precision needs less memory to train more extensive networks. As a result, the training process is more efficient since it takes less memory bandwidth. Finally, the lower the precision, the speedier the mathematical operations may be carried out.
Shorten the training or inference time. 

## Dealing with quantization loss
Loss scaling is used to preserve small gradient values.

# Terminology
## Mantissa (Significand)
The mantissa represents the significant digits of a number in scientific notation. It determines the precision of the floating-point format.
   - Precision and the Mantissa.
     - The number of bits allocated to the mantissa decides how many significant figures the format can store.
     - More bits = higher precision, meaning numbers can be represented with greater accuracy.

## Exponent
The exponent determines the scale or range of the number. It allows numbers to be represented as very large or very small by moving the decimal point.
   - Dynamic Range and the Exponent
       - The number of bits allocated to the exponent determines the dynamic range, which is the range of representable values (from smallest to largest).
       - A larger exponent allows for a broader range of numbers but does not improve precision.

## Bfloat16 vs FP16
Bfloat16 (Brain Floating Point) and FP16 (Half Precision Floating Point) are both 16-bit floating-point formats designed for computational efficiency, especially in machine learning and AI workloads. However, they have distinct differences in representation and use cases. 
   * Bfloat16 sacrifices mantissa bits to retain an 8-bit exponent (same as FP32), providing a wide dynamic range similar to FP32 but with reduced precision.
   * FP16 provides more precision due to its 10-bit mantissa but has a smaller range because of its 5-bit exponent
   
