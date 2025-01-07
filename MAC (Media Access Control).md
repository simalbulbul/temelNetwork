### MAC (Media Access Control)

MAC adresleri ağ iletişiminde cihazlar arasında veri alışverişini sağlamak için kritik bir rol oynar. Bu katman, fiziksel katmandan aldığı veriyi işler ve ağdaki cihazların birbirini tanımasını sağlar. Veri bağı katmanında haberleşme, cihazların birbirine gönderdiği verinin doğru cihaz tarafından alınmasını sağlamak için MAC adresleri üzerinden gerçekleştirilir. 

- MAC adresi, bir cihazın Ethernet kartına üretim aşamasında atanır ve dünya üzerindeki tüm cihazlarda benzersizdir.
- Yapısı: 6 oktet ve toplamda 48 bitten oluşur.
Örnek: 00:1A:2B:3C:4D:5E

**MAC Adresinin Yapısı**

Bu adresin ilk üç okteti cihazın üretici firmasını belirtirken, son üç okteti üretici tarafından belirlenen benzersiz bir numarayı ifade eder. Üretici firmaların bu numaraları nasıl aldığına gelince, firmalar Ethernet kartı üretmeye karar verdiklerinde IANA (Internet Assigned Numbers Authority) adlı kuruluşa başvurarak bir üretici ID’si alır. Bu ID, o firmaya özel olarak atanır ve firmanın ürettiği her cihazda bu ID'nin ilk üç oktet olarak yer almasını sağlar.

1. İlk 3 Oktet:

- Üretici firmayı temsil eder ve bu kod IANA (Internet Assigned Numbers Authority) tarafından atanır.
Örneğin, bir Ethernet kartı üretmek isteyen firma IANA'ya başvurur ve kendisine özel bir ID (örneğin 00:1A:2B) alır.

2. Son 3 Oktet:
- Üretici firmanın, cihazlarına özgü olarak belirlediği sayılardır. Bu, cihazın seri numarası gibi düşünülebilir.

**PC'de MAC Adresini Bulmak**
Bilgisayarınızın MAC adresini öğrenmek oldukça kolaydır.

1. Komut Satırını Açın:
- Başlat Menüsü → cmd yazarak komut satırını açın.

2. Komutu Girin:
- Aşağıdaki komutu yazın ve Enter'a basın:
`ipconfig /all`

2. Çıktıyı İnceleyin:
- "Fiziksel Adres" veya "Physical Address" kısmında cihazınızın MAC adresini görebilirsiniz.

Örnek Çıktı: 00-1A-2B-3C-4D-5E


![a1](https://github.com/user-attachments/assets/43b8adc3-a89d-4c78-b607-8c60f7f6179e)
