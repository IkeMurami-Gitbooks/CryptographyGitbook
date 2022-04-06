# AES-CTR: Fixed nonce

## Используя подстановки

Attack this cryptosystem piecemeal: guess letters, use expected English language frequence to validate guesses, catch common English trigrams, and so on.

Пример: [https://cryptopals.com/sets/3/challenges/19](https://cryptopals.com/sets/3/challenges/19)

## Статистическое решение

Instead of making spot guesses at to known plaintext, treat the collection of ciphertexts the same way you would repeating-key XOR.

Obviously, CTR encryption appears different from repeated-key XOR, _but with a fixed nonce they are effectively the same thing._

To exploit this: take your collection of ciphertexts and truncate them to a common length (the length of the smallest ciphertext will work).

Solve the resulting concatenation of ciphertexts as if for repeating- key XOR, with a key size of the length of the ciphertext you XOR'd.

Пример: [https://cryptopals.com/sets/3/challenges/20](https://cryptopals.com/sets/3/challenges/20)&#x20;
