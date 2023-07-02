Hex
===

* [hexyl: A command-line hex viewer ](https://github.com/sharkdp/hexyl)

```javascript
const nonHexRegex = new RegExp('[^0-9a-f]+', 'gi')
export function cleanHexString(hex_string) {return hex_string.toLowerCase().replaceAll(nonHexRegex, "")}
export function* hexToBytes(hex) {
    console.assert(hex.length % 2 == 0)
    for (let c = 0; c < hex.length; c += 2) {
        yield parseInt(hex.substr(c, 2), 16)
    }
}
```
