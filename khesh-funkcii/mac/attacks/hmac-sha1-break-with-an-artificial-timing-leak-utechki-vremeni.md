# HMAC-SHA1: Break with an artificial timing leak — утечки времени

Это вообще большая проблема в криптографии — неправильное сравнение.&#x20;

Например, HMAC-SHA1 ломается, если сравнение подписи происходит побайтово (и соответственно, мы получаем информацию раньше или позже).

Пример: [https://cryptopals.com/sets/4/challenges/31](https://cryptopals.com/sets/4/challenges/31)

