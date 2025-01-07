### OSI Modeli

 OSI (Open Systems Interconnection) modeli, bilgisayarlar ve ağ cihazları arasındaki iletişim sürecini 7 farklı katmanda ele alan bir ağ modelidir. TCP/IP modeli ise iletişimi daha sadeleştirilmiş bir şekilde 4 katmanda gösterir. Her iki model de cihazların birbiriyle iletişim kurabilmesi için standart bir yapı sunar.
  
![1_322lRmlTQQDJR4DBWbYAZg](https://github.com/user-attachments/assets/b0e34dcd-c483-48a2-aecc-880297fc4818)

### Encapsulation ve Decapsulation Nedir?

**1. Encapsulation (Kapsülleme):**

- Veri, bir cihazdan çıkıp diğerine gönderilirken, her katmandan geçtiğinde üzerine o katmana özgü bir header (başlık) eklenir. Bu başlık, veriyi yönlendirmek ve işlemek için gereken bilgileri taşır.

Örneğin: Gönderici cihazda, veri uygulama katmanından başlar ve fiziksel katmana kadar her aşamada yeni bir başlık eklenir.

**2. Decapsulation (Kapsülün Çözülmesi):**

- Alıcı cihaz, fiziksel katmandan başlayarak veriyi alır ve her katmanda bir önceki katmanın eklediği başlığı çıkarır. Bu işlem her katmanda tekrar eder ve sonunda alıcı cihaz verinin saf haline, yani asıl içeriğine ulaşır.

**Encapsulation:** Bir paketi kargoya verirken, önce kutuya koyar, sonra üzerine adres bilgilerini ekler ve gönderirsiniz. Her işlem, paketin üstüne bir bilgi eklemek gibidir.

**Decapsulation:** Alıcı paketi teslim aldığında, önce kargo kutusunu açar, ardından paketi çıkarır ve son olarak içindeki ürüne ulaşır.
Bu süreçte OSI modelindeki her katman, bir gönderici ile bir alıcı arasında gerçekleştirilen işlemleri temsil eder.
