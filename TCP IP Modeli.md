### TCP/IP: İnternetin Doğuşu

- Bugün kullandığımız internetin temelini oluşturan TCP/IP, aslında Amerika Savunma Bakanlığı’nın (DoD) 1960'ların sonunda ortaya çıkan bir ihtiyacını çözmek için tasarlandı. O dönemde Advanced Research Projects Agency (ARPA) isimli bir kuruluş, ABD'deki üniversiteler arasında hızlı ve kolay veri paylaşımı yapmak istiyordu. Amaç, farklı cihazların ve sistemlerin birbiriyle iletişim kurabilmesini sağlayacak bir dil, yani bir protokol geliştirmekti.

- Bu çalışmaların sonunda, ARPANET adı verilen bir ağ oluşturuldu. ARPANET, internet tarihindeki ilk "paket-anahtarlamalı" (packet-switching) ağdı. Başka bir deyişle, veriler bu ağ üzerinde küçük parçalara bölünerek gönderiliyor, alıcıda yeniden birleştiriliyordu. Bu teknoloji, bugünkü internetin altyapısını oluşturdu.

- 1969 yılının sonunda ARPANET, sadece dört bilgisayardan oluşuyordu. Ama bu küçük adım, internetin dev bir iletişim ağına dönüşmesinin başlangıcıydı. Kısacası, ARPANET sayesinde modern internetin ilk temeli atılmış oldu.


### TCP/IP Modelinde Veri İletimi Nasıl Çalışır?

- TCP/IP modelinde, gönderilen veriler birden fazla aşamadan geçerek karşı tarafa iletilir. Bu süreçte veriler, her katmanda kapsüllenerek (encapsulation) bir alt katmana aktarılır. Kapsülleme, veriye o katmana özgü bilgilerin eklenmesi anlamına gelir. Örneğin, bir e-posta gönderirken, e-postanızın başına ve sonuna o katmanın "nereye gideceği" ve "hangi yöntemle gönderileceği" gibi bilgilerin eklenmesi kapsülleme işlemidir.

- Alıcı tarafında ise bu veriler, her katmanda açılarak (decapsulation) bir üst katmana gönderilir. Açma işlemi, eklenen bilgilerin sırasıyla çıkarılması ve verinin orijinal haline döndürülmesi anlamına gelir. Bu yöntem sayesinde farklı marka ve modellerdeki cihazlar uyum içinde çalışabilir.

- Örneğin, bir bilgisayar Ethernet (kablolu internet) bağlantısı yerine Wi-Fi (kablosuz internet) kullansa bile bu durum, o bilgisayarın üzerinde farklı bir web tarayıcı (örneğin Chrome yerine Safari) kullanmasını gerektirmez. Çünkü TCP/IP modeli, ağ katmanlarını birbirinden bağımsız tutarak cihazların ve yazılımların birbiriyle sorunsuz bir şekilde çalışmasını sağlar.

- Kısacası, TCP/IP modeli, verilerin düzenli bir şekilde gönderilip alınmasını sağlayan, hem cihazları hem de yazılımları uyumlu hale getiren bir sistemdir. 

![1](https://github.com/user-attachments/assets/13fa43b2-8fda-40eb-a9ec-cf1e0ad4ad73)

### KATMANLAR

**1. Uygulama Katmanı (Application Layer)**
Bu katman, aslında kullandığımız uygulamaların ve bu uygulamaların veri gönderirken kullandığı dosya türlerinin bulunduğu yer. Daha basit bir ifadeyle, internetteki bir web sayfasını açarken ya da bir dosya gönderirken bu katman devrede olur.

Örneğin: “Turkcell ana sayfasını, HTTP protokolü üzerinden HTML formatında bir web tarayıcısında açıyorsunuz.”
Buradaki:

- HTTP, web sayfalarının iletişim kurmasını sağlayan bir protokol (bir çeşit iletişim dili),
- HTML ise o sayfanın yazıldığı dosya formatıdır.

Bu katman ayrıca, OSI modelinde (TCP/IP’den farklı bir model) ayrı olan sunum (veriyi okuma biçimi) ve oturum (iki cihaz arasındaki iletişimin yönetimi) katmanlarını da içinde barındırır.

Bu katmanda sık kullanılan protokoller:

- SMTP: E-posta göndermek için kullanılır.
- FTP: Dosya transferi yapmak için kullanılır.

**2. Taşıma Katmanı (Transport Layer)**
Bu katman, gönderilen verinin karşı tarafa nasıl gönderileceğini belirler. İşte veri gönderirken yaşanan şu konular burada çözülür:

- Hata kontrolü (error control): Veri kaybı yaşandı mı?
- Akış kontrolü (flow control): Çok fazla veri aynı anda mı gidiyor, hız dengeleniyor mu?
- Güvenilirlik (reliable): Veriler doğru sırayla mı iletildi, eksik veri var mı?

Bu katmanda iki ana protokol kullanılır:

1. TCP (Transmission Control Protocol):
Bağlantı tabanlıdır (connection-oriented). Yani veri gönderilmeden önce iki cihaz arasında bir anlaşma yapılır. Bu, iki kişinin telefon konuşmasına başlamadan önce “Alo” demesine benzer.
Güvenilirdir. Yani veri, sıralı bir şekilde, kayıpsız olarak iletilir.

2. UDP (User Datagram Protocol): 
Bağlantısızdır (connectionless). Yani veri direkt gönderilir, önceden anlaşma yapılmaz.
Daha hızlıdır, ancak gönderilen verinin ulaşacağı garanti edilmez. Bu, bir kişinin mektubu posta kutusuna bırakıp teslim edilip edilmediğini kontrol etmemesine benzer.

Örnek: Video oyunları gibi hızlı ama çok hassas olmayan veri iletimi gerektiren yerlerde UDP kullanılırken, bir e-posta gönderiminde güvenilirlik önemli olduğu için TCP tercih edilir.

**3. İnternet Katmanı (Network Layer)**
Bu katmana bazen IP Katmanı da denir. Burada, gönderilen veriye bir adres etiketi eklenir. Bu etiket, verinin hangi cihazdan geldiğini ve hangi cihaza gitmesi gerektiğini gösteren bir IP adresidir.

Aynı zamanda bu katman, verinin en iyi yol üzerinden hedefe ulaşmasını sağlar. Yani bu katman, veriyi adresine en hızlı ve doğru şekilde ulaştırmanın yollarını arar. Bu işlemi yönlendirme cihazları olan router (yönlendirici) yardımıyla yapar.

Bu katmanda kullanılan protokoller:

- IP (Internet Protocol): Verilere kaynak ve hedef adresleri ekler.
- ICMP: Hata raporlarını ve ağ durumunu bildirir.

**4. Ağ Arayüzü Katmanı (Network Interface / Data Link Layer)**
Bu katman, veriyi fiziksel olarak gönderip alan cihazlar arasında bir köprü görevi görür. Gönderilen veri burada donanım diline çevrilir. Mesela, bir veriyi internet kablosuyla mı, kablosuz bağlantıyla mı göndereceğiniz bu katmanda belirlenir.

- Hata bildirimi,
- Ağ düzeni (topolojisi),
- Veri akışı kontrolü gibi işler de bu katmanda yapılır.
Bu katmanda MAC adresi adı verilen bir donanım adresi kullanılır. MAC adresi, bir cihazın ağ üzerindeki kimliği gibidir.

Örnek: İki bilgisayar aynı ağda iletişim kuruyorsa, bu katman cihazların MAC adreslerini kullanarak veriyi doğru yere ulaştırır.

Bu katmanda kullanılan cihazlar: Switchler (veriyi ağ üzerindeki doğru cihaza iletir).

**5. Fiziksel Katman (Physical Layer)**
Bu katman, verilerin fiziksel olarak nasıl iletileceğiyle ilgilenir. Örneğin:

- Birler ve sıfırlar (yani dijital veri), elektrik sinyallerine, ışık sinyallerine ya da radyo dalgalarına nasıl dönüştürülecek?
- Bu sinyaller kablo, fiber optik ya da kablosuz olarak nasıl gönderilecek?

Burada işler tamamen fiziksel düzeyde gerçekleşir, yani veriler kablolar, sinyaller ve cihazlar arasında taşınır.

Bu katmanda kullanılan cihazlar:

- HUB: Bir ağdaki cihazlar arasındaki fiziksel bağlantıyı sağlar.
Örnek: Bir USB kablosunun bilgisayara veri aktarırken kullandığı elektrik sinyalleri bu katmanda işlenir.
