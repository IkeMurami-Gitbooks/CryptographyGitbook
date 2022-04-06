# SHA1-MAC: Length-Extension Attack

Использовать функцию SHA1 как MAC небезопасно:

```
digest = SHA1(KEY || MESSAGE)
```

Атакующий может подделать подпись для своего сообщения, не зная ключа.

Length-Extension Attack: [https://dzone.com/articles/forging-a-sha-1-mac-using-a-length-extension-attac](https://dzone.com/articles/forging-a-sha-1-mac-using-a-length-extension-attac)\
[https://cryptopals.com/sets/4/challenges/29](https://cryptopals.com/sets/4/challenges/29)

