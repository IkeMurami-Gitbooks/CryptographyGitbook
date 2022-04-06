# Чтение сертификатов и ключей

pkcs7 - не является сам сертификатом - контейнер, содержащий в себе несколько других сертификатов (часто формат файла: ".p7s").

{% embed url="http://citforum.ru/security/cryptography/openssl/" %}

Создание ключей: \
privkey: openssl genrsa -out key.priv 4096 \
pubkey: openssl rsa -in key.priv -out key.pub -pubout

Вывести отпечаток серта: \
\-fingerprint -sha1 (или sha256, md5)

openssl pkcs7 -in test.cert -inform der -text -noout -print\_certs \
pkcs7 - тип контейнера (видел: pkcs7, x509, pkcs12, smime) \
\-in  - файл сертификата \
\-inform  - необязательный параметр, возможно:)) , позволяет указать тип кодировки сертификата - der или pem. В случае неправильно указанного формата, вылетит ошибка => можно узнать тип кодировки. \
Замечание: der - бинарные данные, pem - в base64 закодированные данные (те же самые) \
\-text - отобразить в текстовом виде (utf8) \
\-noout - не выводить в консоль \
\-print\_certs - вывести (все же в консоль:)) ) информацию о сертификатах (информация будет прям читабельной!!!! )

Несколько примеров с x509 \
openssl x509 -in cert.text -text -noout

посмотреть der-закодированный сертификат: \
openssl x509 -in cert.der -inform der -text -noout

transform: \
PEM2DER: openssl x509 -in cert.crt -outform der -out cert.der \
DER2PEM: openssl x509 -in cert.crt -inform der -outform pem -out cert.pem

Просмотр ключа: openssl rsa -in test.key \[-inform der] \[-check] \
Просмотр экспонент и т.п.: openssl rsa -inform der -text -noout < key.der
