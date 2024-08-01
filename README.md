# HAS01 Hashing Algorithm

A Go implementation of the HAS01 hashing algorithm based on the cryptographic sponge construction.

- Supports 256-bit and 512-bit hash outputs
- Processes data in 192-bit blocks
- Implements absorb-squeeze paradigm

## Usage

```go
h := NewHAS01(HashSize256)
h.Write([]byte("your data here"))
hash := h.Sum(nil)
```