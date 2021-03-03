## AES
- 2 sunucu üzerinde eşzamanlı olarak belirli algoritmalarla aynı anahtara ulaşması ile AES anahtarı oluşturulur. 
(During the initial key exchange process used to set up the symmetrical encryption (used to encrypt the session), asymmetrical encryption is used.)
- AES encryption networkü şifrelemek için kullanılır.
## RSA
- RSA'a kimlik doğrulama için ihtiyaç duyulur.
- RSA'da Public key ile Private key ilişkilidir.
- RSA'da Public key açık olarak rahat rahat paylaşılabilir, Public key'den Private key geri oluşturulamaz.
- RSA'da mesaj Public key ile şifrelenip yollanır Private key ile decrypt edilir.
- RSA'da public key ile mesaj şifrelenip yollandığı için iletişim tek yönlüdür. (2 pair ile client ve serverde ayrı ayrı oluşturulursa işler karışır tabii.)
- The client creates a key pair and then uploads the public key to any remote server it wishes to access. 
- The server can use the public key in this file to encrypt a challenge message to the client. If the client can prove that it was able to decrypt this message, it has demonstrated that it owns the associated private key. The server then can set up the environment for the client.
## Hash
- Their main distinguishing attributes are that they are never meant to be reversed, they are virtually impossible to influence predictably, and they are practically unique.

https://www.linkedin.com/pulse/comparing-ecc-vs-rsa-ott-sarv/
https://www.digitalocean.com/community/tutorials/understanding-the-ssh-encryption-and-connection-process
