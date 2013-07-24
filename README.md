sparse_matrix
=============

a mini project in datastructure course for multiplying and adding two large sparse matrices

sparse matrix is a matrix with large number of entries filled with zero's.
we can add or multiply these matrices by normal addition and row - col multiplication. but by doing so we are unnecessarily
making a lot of 0 * 0 multiplications and  0 + 0 additions.

in this project we are making an attempt to give better solution to this problem by avoiding un necessary computations.

how are we doing this??
    here we are computing addition and multiplication of matrices by representing the matrices in a linked list.
    this linked list has entries which are only the non-zero elements found in the matrix. and it does not store any 
    information about the zero elements.
    
    each node in the list has a row, col, val fields each representing the row number, column number and the value at 
    the position indicated by row and column.
    
    using this linked list representation of the matrices, we are adding and multiplying two matrices.
