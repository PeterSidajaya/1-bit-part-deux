# 1-bit-part-deux
Repository pertaining to:
(arxiv link coming soon)

How to use:
For `measurements_5255.mat` for the (5,2,5,5) scenario, when you open it, you will load a variable called `new_x` with size (2,7,5,5). In actuality, the matrix that we want to use is given by

`new_x(1,:,:,:) + 1j * new_x(2,:,:,:)`

I.e., the real and imaginary parts are separated.

Alices’ projective measurements are then given by new_x`(x,a,:)` where `x` is her question and `a` is her answer. Correspondingly, Bob’s are `new_x(5+y,b,:)`.

For (6,2,6,6), it will be a (2,8,6,6) matrix and, after combining the two parts, Alice’s projectors are `new_x(x,a,:)`, while Bob’s are `new_x(6+y,b,:)`.
