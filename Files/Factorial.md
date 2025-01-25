# Factorial

Factorial is an operation in math that is the product of all integers from $n$ to $1$, where $n>0$.

## Math

In math, factorial is represented with an exclamation point ($!$), but you could represent it as a function.

### Explicit formula

$$f(x)=\prod^x_{n=1}{n}$$

#### Examples

$f(6)=1\cdot2\cdot3\cdot4\cdot5\cdot6=720\\\\
f(4)=1\cdot2\cdot3\cdot4=24\\\\
f(10)=1\cdot2\cdot3\cdot4\cdot5\cdot6\cdot7\cdot8\cdot9\cdot10=3,628,800$

### Recursive formula

$$f(x)=x\cdot f(x-1)\\\\
f(1)=1$$

#### Examples

$f(2)=2\cdot f(1)=2\cdot1=2\\\\
f(5)=5\cdot f(4)=5\cdot4\cdot f(3)=5\cdot4\cdot3\cdot f(2)=5\cdot4\cdot3\cdot2\cdot f(1)=5\cdot4\cdot3\cdot2\cdot1=120$

## Coding

### JavaScript and TypeScript
```javascript
function factorial(n) {
  for (i = n - 1; i > 0; i--) {
    n = n * i;
  }
  return n;
}
```

```typescript
function factorial(n: number): number {
  for (i: number = n - 1; i > 0; i--) {
    n = n * i;
  }
  return n;
}
```

### C/C++
```cpp
int factorial(int n) {
  for (int i = n - 1; i > 0; i--) {
    n = n * i;
  }
  return n;
}
```

### Python
```python
def factorial(n):
    i = n
    while i > 0:
        n = n * i
        i -= 1
    return n
```

### Java
```java
static int factorial(int n) {
  for(int i = n - 1; i > 0; i--)
    n = n * i;
  }
  return n;
}
```
