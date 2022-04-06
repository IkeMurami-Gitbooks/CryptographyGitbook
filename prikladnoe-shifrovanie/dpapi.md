---
description: Data Protection API
---

# DPAPI

Защита информации с помощью учетных данных пользователя Windows: [https://docs.microsoft.com/en-us/windows/desktop/api/](https://docs.microsoft.com/en-us/windows/desktop/api/)..\
Никаких ключей не надо хранить. Вызываешь CryptUnprotectedData(input, null, null, null, output) - получаешь зашифрованную строку. CryptProtectedData -> расшифровываешь.

Так гугл защищает пароли от др сервисов - плохого не посоветуют)

Минусы - расшифровать можно, только под той же учетной записью что и зашифровывалась

{% embed url="https://github.com/mis-team/dpapick" %}

