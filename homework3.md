

```
from starkware.cairo.common.serialize import serialize_word

func square (x: felt) -> (y: felt) {
  tempvar res = x*x;
  return (y=res);
}

func main{output_ptr: felt*}() {
    tempvar x = 10;
    let (res) = square(x);
    serialize_word(res);
    return ();
}
```
