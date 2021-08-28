# xyzpub

Convert xpubs and xprvs to different versions.


## Example

```rust
use xyzpub::{convert_version, Version};

let xpub = "xpub6BosfCnifzxcFwrSzQiqu2DBVTshkCXacvNsWGYJVVhhawA7d4R5WSWGFNbi8Aw6ZRc1brxMyWMzG3DSSSSoekkudhUd9yLb6qx39T9nMdj";
let expected_zpub = "zpub6qUQGY8YyN3ZxYEgf8J6KCQBqQAbdSWaT9RK54L5FWTTh8na8NkCkZpYHnWt7zEwNhqd6p9Utq562cSZsqGqFE87NNsUKnyZeJ5KvbhfC8E";

let result = convert_version(xpub, &Version::Zpub).unwrap();

assert_eq!(result, expected_zpub);
```

 ## Useful resources
 - xpub converter: https://jlopp.github.io/xpub-converter/
 - slip132: https://github.com/satoshilabs/slips/blob/master/slip-0132.md
