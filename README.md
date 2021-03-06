# top-k-kendall-tau python module
Top-k kendall-tau distance.  This python module generalise kendall-tau as defined in:
*Fagin, Ronald, Ravi Kumar, and D. Sivakumar. "Comparing top k lists." SIAM Journal on Discrete Mathematics 17.1 (2003): 134-160*.

It returns a distance: 0 for identical (in the sense of top-k) lists and 1 if completely different.

# Example
Simply call kendall_top_k with two same-length arrays of ratings (or also rankings), length of the top elements k (default is the maximum length possible), and p (default is 0, see [1]) as parameters:

```python
        import kendall
        a = np.array([1,2,3,4,5])
        b = np.array([5,4,3,2,1])
        kendall.kendall_top_k(a,b,k=4)
```

# Requirements
numpy, scipy
