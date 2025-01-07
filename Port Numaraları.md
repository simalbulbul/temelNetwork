### Port Numaraları

- Sunucular eriştiği hedefteki hangi programdan hizmet alacağını port numaraları belirler.
- Port numaraları, bilgisayarlar ve ağlar arasında yapılan iletişimin düzenli ve güvenli bir şekilde gerçekleşmesini sağlayan önemli bir bileşendir. Portlar, sunucular ve istemciler arasındaki veri iletiminde belirli bir uygulamaya veya servise yönlendirilen paketleri tanımlar. Bu sayede bir bilgisayarda birden fazla program aynı anda çalışabilir ve her biri farklı portlardan hizmet verebilir.
- Ağ üzerindeki herhangi bir sunucu programa bağlanmak istenildiğinde, programın çalıştığı bilgisayarın adresinin yanında istekleri kabul ettiği 'port' numarasını da vermek gerekir.

**Well-known Portlar** (1024 ve Altındaki Portlar): Bu portlar, dünya çapında yaygın olarak kullanılan uygulamalar ve servisler için ayrılmıştır. 0 ile 1023 arasındaki port numaraları, belirli bir uygulama için dünya çapında kabul görmüş ve genellikle sabit olan port numaralarıdır. 

- Diyelim ki bir internet sitesine girmek istiyorsunuz. Önce port 53 üzerinden DNS sorgusu yapılır, çünkü DNS (Domain Name System), alan adı ile IP adresi arasında bir çeviri yaparak doğru siteye yönlendirilmenizi sağlar. Ardından, DNS cevabı ile belirlenen IP adresi üzerinden, HTTP (port 80) veya HTTPS (port 443) protokollerine bağlı olarak web sitesine erişirsiniz.
- Bir başka örnek vermek gerekirse, e-posta göndermek için port 25 üzerinden SMTP protokolü kullanılır. Bu port, e-posta sunucusunun gelen mesajları alması için belirlenmiştir.

Ağ yöneticileri, belirli bir portun açık olup olmadığını kontrol etmek için çeşitli araçlar kullanır. Telnet gibi araçlarla, belirli bir portun açık olup olmadığını anlamak mümkündür. Eğer bağlantı başarıyla gerçekleşirse, o port üzerinden hizmetin verildiği anlaşılır.

Örneğin, bir web sunucusunun çalışıp çalışmadığını kontrol etmek için:

`telnet www.google.com 80`

komutu kullanılarak port 80’in açık olup olmadığı test edilebilir.

`netstat -an ` komutu, bilgisayarınızdaki ağ bağlantılarını ve açık portları listelemenizi sağlayan bir ağ aracıdır. Bu komut, özellikle ağ durumu hakkında hızlı bilgi almak için kullanılır ve şu bilgileri sağlar:

1. Aktif bağlantılar: Hangi istemciler ve sunucular arasında veri iletimi yapıldığını gösterir.
2. Açık portlar: Bilgisayarınızdaki hangi portların dinlendiğini (listening) ve bağlantı taleplerini kabul ettiğini belirtir.
3. Bağlantı durumu: Bağlantıların mevcut durumu hakkında bilgi verir. Örneğin, "ESTABLISHED" (kurulmuş bağlantı), "LISTENING" (dinleme durumunda) veya "TIME_WAIT" (bağlantı sonlanmak üzere) gibi.

![netstat-1024x683](https://github.com/user-attachments/assets/86d86038-ba83-471b-895d-a268c2677cba)



