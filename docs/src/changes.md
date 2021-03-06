# Changes
## v0.2.5, Jan 26, 2020
- fixed allocations in  Base.+
- added updateindex! method 
- provide fdrand and fdrand! matrix constructors
- automatic benchmarks in examples

## v0.2.4, Jan 19, 2020
- Allow preconditioner creation directly from CSC Matrix
- Rename AbstractPreconditioner to AbstractExtendablePreconditioner

## v0.2.3, Jan 15, 2020
- Started to introduce preconditioners (undocumented)

## v0.2.3, Jan 8, 2020
- added norm, cond, opnorm methods
- resize! instead of push! when adding entries should trigger less allocation operations

## v0.2.2. Dec 23, 2019
- What used to be `_splice`  is now `+` and allows now real addition (resulting in a CSC matrix)
- Added constructors of LNK matrix from CSC matrix and vice versa
- reorganized tests

## v0.2.1 Dec 22, 2019
- Tried to track down the source from which I learned the linked list based struct in order
  to document this. Ended up with SPARSEKIT of Y.Saad, however I believe this 
  already was in SPARSEPAK by Chu,George,Liu.
- Internal rename of SparseMatrixExtension to SparseMatrixLNK. 

## v0.2 Dec 21, 2019
- more interface methods delegating to csc, in particular mul! and ldiv!
- lazy creation of extendable part: don't create idle memory
- nicer constructors
  
## V0.1, July 2019
- Initial release

