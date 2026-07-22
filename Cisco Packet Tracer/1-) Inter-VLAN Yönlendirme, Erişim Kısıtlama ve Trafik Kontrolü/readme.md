# 🇹🇷 Ağ Güvenliği ve Trafik Optimizasyonu: Yönlendirme & Erişim Kontrolü

Bu laboratuvar senaryosunda, Cisco Packet Tracer üzerinde 1941 serisi bir Router kullanılarak iki farklı alt ağ (192.168.1.0/24 ve 192.168.2.0/24) arasında yapılandırma sağlanmış; aynı zamanda ağ güvenliğini artırmak ve trafiği optimize etmek amacıyla Router CLI üzerinden çeşitli "Network Hardening" ve QoS (Quality of Service) politikaları uygulanmıştır.

## 📌 Topoloji
![Ağ Topolojisi](../Ekran%20Alıntısı.PNG)

## 🚀 Uygulanan Senaryo ve Kritik Konfigürasyonlar
Merkezi yönlendirici üzerinden bağlanan yerel ağlarda aşağıdaki güvenlik ve optimizasyon işlemleri başarıyla test edilmiştir:

* **Hedefe Yönelik Erişim Engelleme (ACL):** Ağ içerisindeki cihazların yetkisiz erişimlerini kısıtlamak amacıyla Standart/Genişletilmiş Erişim Kontrol Listeleri (ACL) yapılandırıldı. CLI üzerinden yazılan kurallar ile **192.168.1.2** IP adresine sahip cihazın ağ üzerindeki erişimi tamamen engellendi (Deny).
* **Bant Genişliği ve Hız Optimizasyonu (Traffic Shaping):** Ağ performansını korumak ve darboğazları (bottleneck) önlemek için GigabitEthernet arayüzlerinde hız sınırlandırması (Rate Limiting) uygulandı. Bu kapsamda, **192.168.1.3** IP adresine sahip cihazın paket iletim hızı CLI üzerinden düşürülerek ağ trafiği optimize edildi.
* **Temel Yönlendirme ve Gateway Yapılandırması:** Farklı IP bloklarındaki uç noktaların (End Devices) kesintisiz haberleşebilmesi için Router üzerinde gerekli Gateway adreslemeleri ve arayüz konfigürasyonları tamamlandı.

---

# 🇬🇧 Network Security & Traffic Optimization: Routing & Access Control

In this laboratory scenario, communication between two different subnets (192.168.1.0/24 and 192.168.2.0/24) was established using a 1941 series Router on Cisco Packet Tracer. Additionally, various Network Hardening and QoS (Quality of Service) policies were implemented via the Router CLI to enhance network security and optimize traffic flow.

## 📌 Topology
![Network Topology](../Ekran%20Alıntısı.PNG)

## 🚀 Applied Scenario and Key Configurations
The following security and optimization operations were successfully tested on local networks connected via the central router:

* **Targeted Access Denial (ACL):** Standard/Extended Access Control Lists (ACLs) were configured to restrict unauthorized access by devices within the network. Through rules applied via the CLI, the device with the IP address **192.168.1.2** was strictly denied access to the network.
* **Bandwidth and Speed Optimization (Traffic Shaping):** Rate Limiting was applied to the GigabitEthernet interfaces to maintain network performance and prevent bottlenecks. Consequently, the packet transmission speed of the device with the IP address **192.168.1.3** was throttled via the CLI, ensuring optimized network traffic.
* **Basic Routing and Gateway Configuration:** Essential Gateway addressing and interface configurations were completed on the Router to allow seamless communication between end devices located in different IP blocks.
