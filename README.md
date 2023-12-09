# Mixed Precision Training
Mixed precision is a computing approach that uses a combination of multiple numerical precisions such as FP-16(half precision), FP-32(single-precision), FP-64(double precision)

## Why mixed precision training or mixed precision in general
Lower precision needs less memory to train more extensive networks. As a result, the training process is more efficient since it takes less memory bandwidth. Finally, the lower the precision, the speedier the mathematical operations may be carried out.
Shorten the training or inference time. 

## Dealing with quantization loss
Loss scaling is used to preserve small gradient values.

