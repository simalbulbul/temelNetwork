### TCP (Transmission Control Protocol)

- TCP, bağlantı odaklı bir protokoldür, yani veriyi iletmeye başlamadan önce, veri gönderen ve alıcı arasındaki bağlantıyı kurar. Bu, veri iletiminde güvenlik ve hata kontrolü sağlar. Veriler belirli bir sırayla ve hata kontrolü yapılacak şekilde iletilir.
-Veri iletimine başlamadan önce bağlantıyı kurar (Three-Way Handshake). Bu, alıcı ile verici arasında güvenli bir kanal oluşturur.
-Verilerin doğru sırayla iletilmesini sağlar. Eğer veri kaybolursa ya da yanlış gelirse, verici bu veriyi tekrar gönderir.
-Veriler, alıcıya doğru şekilde iletilip iletilmediğini kontrol etmek için kontrol edilerek gönderilir. Her veri parçası, verici ve alıcı arasında doğrulama yapılır.
-Eğer ağda sıkışma oluşursa, TCP veri gönderme hızını otomatik olarak ayarlar.

örnek olarak:

1. İnternette bir web sayfasını ziyaret ettiğinizde, web tarayıcınız ile web sunucusu arasında veri iletimi TCP üzerinden yapılır. Buradaki veri, sayfanın içeriği, görselleri ve diğer bileşenleri doğru sırayla ve hatasız olarak iletilir.
2. E-posta sunucusu ile istemcisi arasında TCP kullanılarak e-posta mesajları güvenli bir şekilde iletilir.
3. FTP, dosya transferi yaparken TCP’yi kullanır. Dosyalar, kaybolan veya hatalı paketlerin tekrar gönderilmesini sağlayacak şekilde iletilir.

**Bağlantı Kurma Süreci (Three-Way Handshake):**

SYN: İstemci, sunucuya bir bağlantı isteği gönderir.
SYN-ACK: Sunucu, istemciye bağlantı talebini onaylayan bir yanıt gönderir.
ACK: İstemci, sunucuya bağlantı kurulduğunu bildiren bir yanıt gönderir.

![image](https://github.com/user-attachments/assets/d1c4a3c5-2db7-4e01-a7d9-02c8971c29bd)



### UDP (User Datagram Protocol)

UDP, bağlantı kurmayan, daha basit ve hızlı bir protokoldür. UDP’de veri gönderimi yapılırken, alıcı cihazın bağlantı durumu kontrol edilmez ve veri iletimi sırasında hata kontrolü yapılmaz. UDP, verinin en hızlı şekilde iletilmesini sağlar, ancak güvenlik ve sıralama garantisi sunmaz.
veri iletimi başlatılmadan önce herhangi bir bağlantı kurulmaz. Veriler doğrudan gönderilir.
verilerin doğru iletilip iletilmediğini kontrol etmez. Eğer veri kaybolursa, tekrar gönderilmez.
TCP’nin sunduğu güvenlik önlemleri ve sıralama kontrolü olmadığı için UDP, daha hızlı veri iletimi sağlar.
UDP, veri iletiminin düşük gecikme ile yapılmasını sağlar, bu nedenle gerçek zamanlı uygulamalarda tercih edilir.

örnek olarak:

1. Sesli ve görüntülü aramalar (örneğin, Skype veya Zoom) genellikle UDP kullanır. Bu tür uygulamalar, veri kaybını tolere edebilir ve gecikme süresinin düşük olmasını tercih eder.
2. Canlı video akışları ve video izleme servisleri (YouTube, Twitch gibi), veri paketlerinin hızlı bir şekilde iletilmesi için UDP kullanır. Burada önemli olan, verinin zamanında iletilmesidir, kaybolan veri paketleri pek de sorun oluşturmaz.
3. Gerçek zamanlı çevrimiçi oyunlarda, oyuncuların hareketleri ve komutları hızla iletilmelidir. Bu nedenle UDP, düşük gecikme süresi için tercih edilir.

![image](https://github.com/user-attachments/assets/b58d88c2-edd8-4940-ba04-4a18e5968a04)

![102](https://github.com/user-attachments/assets/341fe502-6fba-4a7f-8c18-79533948da52)

