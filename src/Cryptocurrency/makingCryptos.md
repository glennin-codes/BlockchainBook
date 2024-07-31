# Pimitives For Making Cryptocurencies

- Hash function.
- Signature.

## Hash function.

You have some data of any size you run it into a hash function and produced an output of a fixed size.

```Rust
hash (data) -> Output
```

"Avalanche effect" : change 1 bit of input ,about half the output bits should change.

Genearly hash functions are defined onf what they shouldnt do.

    1. Preimage resistance.
    2. 2nd Preimage resistance.
    3. Colission resistance.

**Preimage resistance**
- if your are given output `y` from a hash function that takes in data `x` .You cannot find `x`.
where
 ```C
hash(x)==y
```
(You can find it eventualy but that will take 2^256 operations (10^78));

**2nd Preimage resistance**
  - if you have x,y such that

  ```py
  hash(x) == y
  ```
  you cannot find `x'` where 
```js
  hash(x') == y
```
 in that
```rust
 x!==x'
 ```

**Colission resistance.**


