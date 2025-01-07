### Address Resolution Protocol (ARP)

- Bir cihazın, bir hedef IP adresine veri gönderebilmesi için o IP adresine karşılık gelen MAC adresini bilmesi gerekir. Ancak başlangıçta, cihaz bu MAC adresini bilmez. İşte burada ARP devreye girer.

- ARP, bir cihazın ağda başka bir cihazın MAC adresini öğrenmek için kullandığı bir protokoldür. Cihaz, hedef IP adresini öğrenmek için tüm ağdaki cihazlara bir ARP isteği gönderir. Bu istek, ağda bulunan her cihazın bu IP adresi hakkında bir bilgi verip vermediğini kontrol eder. Eğer ağdaki bir cihaz bu IP adresine sahipse, o cihaz, MAC adresini içeren bir ARP cevabı gönderir. Bu sayede veri gönderen cihaz, hedef bilgisayarın MAC adresini öğrenir ve veriyi doğru cihaza yönlendirebilir.

- Bir cihaz, tüm ağdaki cihazlara veri göndermek istediğinde, bu tür iletimi broadcast olarak adlandırırız. Broadcast paketleri, ağdaki tüm cihazlara aynı anda gönderilir. Bu, bir cihazın mesajının ağdaki diğer her cihazla paylaşılması anlamına gelir. Ancak, bu tür paketlerin gönderilmesi gereksiz band genişliği kullanımı yaratır çünkü ağdaki her cihaz bu mesajı almak zorunda kalır. Bu yüzden broadcast kullanımı bazen verimsiz olabilir.


![1689335143683](https://github.com/user-attachments/assets/2837ae1a-b8dd-41b9-a365-120ff38e4fb4)


- Bir örnek vermek gerekirse, eğer bir bilgisayarın ARP isteği tüm ağa gönderiliyorsa, bu bir **broadcast** mesajıdır çünkü mesaj tüm cihazlara ulaşacaktır.

- **Unicast**, bir cihazın veriyi tek bir cihaz ile paylaştığı iletişim türüdür. Yani, bir bilgisayarın başka bir bilgisayara sadece ona özel olarak veri göndermesi unicast'tır. Bu tür iletimde, veri yalnızca hedef cihaz tarafından alınır ve diğer cihazlar bu veriyi almaz.
Örneğin, A bilgisayarı B bilgisayarına direkt olarak veri gönderdiğinde, bu bir unicast iletişimi olur. Yalnızca A ve B arasında gerçekleşir.

- **Multicast**, bir cihazın belirli bir gruptaki cihazlara veri göndermesi anlamına gelir. Yani, veriyi sadece tek bir cihaz veya tüm ağ yerine, belirli bir grup cihaz alır. Bu sayede, band genişliği daha verimli kullanılır çünkü yalnızca ilgilenen cihazlar mesajı alır.
Örneğin, bir video yayını düşünün. Bu video yayını sadece belirli bir kullanıcı grubuna gönderilmek isteniyorsa, multicast kullanılır. Böylece yalnızca bu grup üyeleri bu yayını izler, diğer cihazlar bu veriyi almaz.


![Unicast-vs-Multicast-vs-Broadcast-1-scaled](https://github.com/user-attachments/assets/a22880cb-4d8a-41f5-979f-7820278f5fc8)

