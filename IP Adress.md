### IP (Internet Protocol - İnternet Protokolü)

Bilgisayarlar, birbirleriyle doğru bir şekilde iletişim kurabilmek için aynı dili konuşmalıdır. IP adresi, bu dili temsil eder ve bilgisayarların birbirini tanıyıp doğru şekilde iletişim kurmasını sağlar. IP, İnternet Protokolü teriminin baş harflerinden oluşur ve bu protokol, internetteki cihazların birbirlerine nasıl bağlanacağını belirler. 

İletişimin düzgün bir şekilde kurulabilmesi için, ağa bağlanan tüm cihazların IP adreslerinin birbirinden farklı olması gerekir. Sistemde aynı IP adresine sahip birden fazla cihaz varsa iletişim kurulamaz ve çakışma meydana gelir.

### IPv4 (Internet Protocol Version 4)

IPv4, İnternet Protokolü'nün 4. versiyonudur. IP protokolünün bir sürümüdür ve şu anda internetin çoğunda yaygın olarak kullanılan adresleme yöntemidir. IPv4, günümüzde en yaygın olarak kullanılan IP adresleme türüdür. IPv4, 32 bitlik adresleme kullanır ve bu sayede 4.294.967.296 (2^32) farklı cihaz için IP adresi atanabilir. 

IPv4 adresi toplamda 32 bit'ten oluşur. Bu 32 bitlik adres, 4 parçaya (bölüme) ayrılır. Her bir parça, 8 bit uzunluğundadır ve bu 8 bitlik her bir bölüme oktet adı verilir.

Bir IPv4 adresi şu şekilde görünür:
192.168.1.1

Bu adres 4 bölümden oluşur ve her bir bölüm 0 ile 255 arasındaki bir sayı ile ifade edilir. IP adresleri ikilik (binary) düzende yazılır ancak kolay okumak ve yazmak için onluk düzene (decimal) çevrilir.  
Mesela 201.171.21.153

![net8](https://github.com/user-attachments/assets/5d1a02bf-21a9-4208-ba07-c442d4e69af9)
![net9](https://github.com/user-attachments/assets/87b1f4a4-9c00-49e0-bc60-bc204b0f3723)


Örnek IP adresi: 201.171.21.153

Bu IP adresini ikilik (binary) düzene çevirelim:

201'in binary karşılığı:
201 = 11001001

171'in binary karşılığı:
171 = 10101011

21'in binary karşılığı:
21 = 00010101

153'ün binary karşılığı:
153 = 10011001

### IP Adresi Türleri

### 1. Class A:
**0.0.0.0 - 127.255.255.255**
- Class A, geniş bir ağ adresleme alanı sunar ve çok büyük ağlar için uygundur. Bu sınıf, internet servis sağlayıcıları veya çok büyük organizasyonlar tarafından kullanılır.
- 128 milyon IP adresi barındırır.

### 2. Class B:
**128.0.0.0 - 191.255.255.255**
- Class B, orta büyüklükteki ağlar için uygundur. Örneğin, büyük bir okul veya orta ölçekli bir şirket için kullanılabilir.
- yaklaşık 16 milyon IP adresi sunar.

### 3. Class C:
**192.0.0.0 - 223.255.255.255**
- Class C, daha küçük ağlar için uygundur. Genellikle küçük işletmeler veya ev ağlarında kullanılır.
- Yaklaşık 65.000 IP adresi sağlar.

### 4. Class D (Multicast):
**224.0.0.0 - 239.255.255.255**
- Bu sınıf, multicast (çoklu yayın) adresleri için ayrılmıştır. Grup adresleri kullanarak birden fazla cihaz aynı adresi dinleyebilir ve bu cihazlar üzerinden veri iletimi sağlanabilir.
- Genellikle televizyon yayınları veya sesli/görüntülü iletişim gibi hizmetlerde kullanılır.

### 5. Class E (Reserved):
**240.0.0.0 - 255.255.255.255**
- Bu IP adresleri, bilimsel araştırmalar ve deneysel kullanım için ayrılmıştır. İnternet ortamında kullanılmazlar ve genellikle ağ araştırmaları veya gelecekteki teknolojiler için ayrılır.

Bu classların içinde özelleşmiş IP blockları mevcuttur.

### Özel IP Adresleri (Private IP Addresses)
- Özel IP adresleri, internete doğrudan bağlanmayan cihazlarda, yani sadece yerel ağlar (evinizdeki Wi-Fi, bir okul ağı, iş yerinizin ağı gibi) üzerinde iletişim kuran cihazlarda kullanılır. Bu adresler, internete açık değillerdir ve sadece belirli ağlarda geçerlidir. Örneğin, evinizdeki bilgisayar veya telefon, kendi ağınız içinde iletişim kurarken, bu özel IP adreslerini kullanabilir.
-A,B ve C classlarında bulunurlar. Özel IP adres aralıkları aşağıda gösterilmiştir;

10.0.0.0 - 10.255.255.255
172.16.0.0 - 172.31.255.255
192.168.0.0 - 192.168.255.255

### Loopback IP Adresi
- Loopback adresi, bir cihazın kendi kendine bağlanması için kullanılan bir adres aralığıdır. 127.0.0.1 adresi, genellikle "localhost" olarak adlandırılır ve cihazın kendi servisini test etmek için kullanılır. Örneğin, bilgisayarınızda çalışan bir web servisini test etmek için tarayıcıya `http://127.0.0.1` yazabilirsiniz.

### Link-Local Adresleri
- Link-local adresler, cihazlar arasında sadece aynı ağda bulunan cihazların iletişim kurabilmesi için kullanılır. Eğer bir cihaz, DHCP (Dynamic Host Configuration Protocol) üzerinden IP adresi almazsa, bu adresler otomatik olarak atanır.
- Genellikle cihazlar birbirlerine doğrudan bağlandıklarında, bir DHCP sunucusu olmadan geçici bir IP alırlar. Bu, ağ içindeki cihazların iletişim kurabilmesi için gerekli adres aralığını sağlar.  Bu adresler, sadece cihazların yerel ağda birbirleriyle iletişim kurmalarını sağlar, internete erişimi sağlamaz.

Diyelim ki evinizde bir Wi-Fi ağı var ve yeni bir telefon almak istediniz. Telefonu Wi-Fi'ye bağladığınızda, telefonun internete bağlanabilmesi için bir IP adresine ihtiyacı vardır. Eğer evdeki modeminiz bir DHCP sunucusu olarak çalışıyorsa, telefon otomatik olarak bir IP adresi alır. Bu adres, telefonun internete bağlanabilmesi için gerekli olan bir genel IP adresi olacaktır.

Fakat eğer Wi-Fi modeminizde DHCP sunucusu kapalıysa ve telefon buna rağmen ağınıza bağlanmaya çalışıyorsa, telefonun IP adresi otomatik olarak 169.254.x.x aralığından seçilir ve bu telefon sadece yerel ağdaki cihazlarla iletişim kurabilir, internete bağlanamaz.

### Multicast IP Adresleri

- Multicast adresleri, bir grup cihazın aynı anda aynı veriyi almasını sağlamak için kullanılır. Bu adresleme türü, bir kaynaktan birden fazla hedefe veri gönderilmesine olanak tanır.
- Bu adresler, örneğin bir grup bilgisayara aynı anda video veya ses yayını yapılmasını sağlamak için kullanılır. Ayrıca bazı ağ uygulamaları, multicast ile veri iletimini gerçekleştirebilir.

Bir video konferans uygulaması düşünün. Bu uygulama, 224.0.0.1 adresi üzerinden toplantı video akışını yayar. Bu Multicast IP adresi üzerinden gönderilen veri, 224.0.0.1 adresini dinleyen tüm katılımcılara iletilir. Bu sayede her katılımcı aynı videoyu izleyebilir.

### Public IP Adresleri

- Yukarıdaki özel IP'ler dışında kullanılan bloklardır, internet ortamında kullanılır. Girdiğimiz çoğu siteye, internetten ulaştığımız her yere bu IP adresleri sayesinde ulaşırız. Bu IP adresleri uniq (tek kullanımlık) olarak kullanılmaktadır
- Dünyada toplamda 5 tane ana RIR bulunmaktadır. Türkiye ve çevresindeki bölgeden sorumlu olan RIR ise RIPE NCC (Réseaux IP Européens Network Coordination Centre)'dir. Bir şirket veya organizasyon, internete bağlı cihazları için kendi public IP aralığını almak istediğinde, RIPE ile iletişime geçmek zorundadır. Bu süreçte, şirketler belirli bir IP bloğu talep eder ve RIPE, bu başvuruya uygun bir IP adres aralığı tahsis eder.
- Public IP adreslerinin doğru bir şekilde yönetilmesi ve dağılması, internetin stabil ve güvenli bir şekilde çalışabilmesi için kritik öneme sahiptir. Bu dağıtım süreci, IP adreslerinin uluslararası koordinasyonu ve internetin büyümesiyle uyumlu olmasını sağlar.

![net11](https://github.com/user-attachments/assets/da7ee47f-3c46-4964-8674-f4b43fc9350a)



