# RSA bla bla
- RSA temelde p ve q olan 2 asal sayının çarpımının kolay hesaplanmasına dayanmaktadır. Ayrıca bu çarpımın sonucunda ortaya çıkan sayının çarpanların geriye dönük hesaplanması oldukça zordur.
- İlk başlangıç noktası olarak asal sayı olan p ve q sayıları seçilir. p eşit değildir q'ya şartıyla.

- p=11
- q=13

## Public Key (n,e)
- Şuan bir örnek yaptığımız için asal sayılar küçüktür. Çarpanlara ayırmayı zorlaştırmak için  asal sayıların çok daha büyük olması gerekir. Şu anda, birkaç bin bit basamaklı  n değerleri güvenli iletişim için kullanılmaktadır.
- Açık anahtar, (product, modulus) n'den ve bir üs değeri olan (exponent) e'den oluşur.
- Üs değeri(e) önceden seçilmiş olabilir ve tüm anahtarlama işlemleri için aynı(sabit) olabilir.

- n=pxq = 143 (8bit)
- e=23 

## Secret Key ( d,φ(n),p,q )
- RSA secret key'i hesaplamak için Euler φ fonksiyonunu kullanır.
- φ(n) ile e'nin en büyük ortak böleni 1 olmalıdır.
- Φ(n)'nin değerini belirlemek için n'yi bilmek yeterli değildir. Sadece p ve q bilgisiyle φ(n)'i verimli bir şekilde belirleyebiliriz.

- φ(n) = (p − 1) × (q − 1) = 120

- Gizli anahtar ayrıca e × d - 1'in φ (n) 'nin katı olması özelliğine sahip bir d'den oluşur. Aşağıdaki formül ile ifade edilebilir, hesaplanabilir.

- e × d = 1 (mod φ(n)) (extended Euclidean algorithm)