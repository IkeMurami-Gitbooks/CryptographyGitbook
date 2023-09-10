# SHA1-MAC: Length-Extension Attack

## Description

Использовать функцию SHA1 как MAC небезопасно:

```
digest = SHA1(KEY || MESSAGE)
```

Атакующий может подделать подпись для своего сообщения, не зная ключа.

Length-Extension Attack: [https://dzone.com/articles/forging-a-sha-1-mac-using-a-length-extension-attac](https://dzone.com/articles/forging-a-sha-1-mac-using-a-length-extension-attac)\
[https://cryptopals.com/sets/4/challenges/29](https://cryptopals.com/sets/4/challenges/29)

## Short

* **Bad**: `hash(KEY || MESSAGE || PADDING)`
* Usable: `hash(MESSAGE || KEY || PADDING)`
* **Good**: `hmac(MESSAGE || KEY || PADDING)`

## Tools

* [https://github.com/bwall/HashPump](https://github.com/bwall/HashPump)
* [https://github.com/iagox86/hash\_extender](https://github.com/iagox86/hash\_extender)
