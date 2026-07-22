# 🇹🇷 Ağ Trafiği Kontrolü: Erişim Engelleme ve Bant Genişliği Sınırlandırma

Bu laboratuvar çalışmasında, Cisco Packet Tracer kullanılarak iki farklı alt ağ (192.168.1.0/24 ve 192.168.2.0/24) arasında yönlendirme yapılmış ve Router CLI ekranı üzerinden çeşitli ağ güvenliği ve trafik kontrol politikaları uygulanmıştır.

## 📌 Topoloji
![Ağ Topolojisi](images/ekranalıntısı.png)

## 🚀 Uygulanan Senaryo ve Konfigürasyonlar
Merkezi bir 1941 Router aracılığıyla bağlanan iki farklı yerel ağ üzerinde aşağıdaki işlemler gerçekleştirilmiştir:

* **Erişim Engelleme (Access Control List - ACL):** Cihazların (PC, Laptop veya Sunucu) birbirleriyle olan iletişimini kontrol altına almak için CLI üzerinden ACL kuralları yazılmıştır. Belirli IP adreslerinin ağlara veya sunuculara erişimi engellenmiştir (Deny/Permit kuralları).
* **Hız Düşürme (Traffic Shaping / Rate Limiting):** Ağ üzerindeki trafiği optimize etmek amacıyla GigabitEthernet arayüzleri üzerinde bant genişliği sınırlandırması yapılmış, paket iletim hızları düşürülmüştür.
* **Temel Yönlendirme:** Farklı bloklardaki (192.168.1.x ve 192.168.2.x) cihazların haberleşmesi için Router üzerinde Gateway yapılandırmaları tamamlanmıştır.

---

# 🇬🇧 Network Traffic Control: Access Deny and Bandwidth Limiting

In this lab practice, routing was established between two different subnets (192.168.1.0/24 and 192.168.2.0/24) using Cisco Packet Tracer, and various network security and traffic control policies were applied via the Router CLI.

## 📌 Topology
![Network Topology](images/ekranalıntısı.png)

## 🚀 Applied Scenario and Configurations
The following operations were performed on two different local networks connected via a central 1941 Router:

* **Access Control List (ACL):** ACL rules were written via CLI to control the communication between devices (PC, Laptop, or Server). Specific IP addresses were blocked from accessing networks or servers (Deny/Permit rules).
* **Traffic Shaping / Rate Limiting:** To optimize network traffic, bandwidth limitation was applied on GigabitEthernet interfaces, reducing packet transmission rates.
* **Basic Routing:** Gateway configurations were completed on the Router to allow communication between devices in different blocks (192.168.1.x and 192.168.2.x).
