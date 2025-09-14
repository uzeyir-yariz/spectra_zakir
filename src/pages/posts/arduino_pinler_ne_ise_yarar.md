---
layout: ../../layouts/post.astro
title: "ARDUİNOYU ANLAMAK-1- BLOG -(5)-"
pubDate: 2025-9-13
description: "arduinodaki pinleri ve işlevlerini inceliyoruz..."
author: "Zakir"
excerpt: null
image:
  src:
  alt:
tags: ["pinler", "kodlama", "eğitim", "modüller", "programlama"]
---

### *Arduino Pin Rehberi: Bu Pinler Ne İşe Yarıyor?*

Merhaba Maker'lar! Arduino'ya yeni başladıysanız veya pinlerin neler yapabildiğini öğrenmek istiyorsanız doğru yerdesiniz. Arduino kartınızın üzerinde gördüğünüz o küçük metal çıkıntılar (pinler), onu gerçek dünyaya bağlayan sihirli köprülerdir. Gelin bu pinleri birlikte inceleyelim.

#### *1. Güç Pinleri (Power Pins)*

Bu pinler, kartınıza veya bileşenlerinize güç sağlamak için kullanılır.

- *Vin:* Kartı harici bir güç kaynağıyla (7-12V önerilir) beslemek için kullanılır. Pili doğrudan buraya bağlayabilirsiniz.
    
- *5V:* Kart üzerindeki regüle edilmiş 5 volt çıkışıdır. Breadboard'inızdaki sensörler veya modüllere güç sağlamak için kullanabilirsiniz.
    
- *3.3V:* Kart üzerindeki regüle edilmiş 3.3 volt çıkışıdır. 3.3V ile çalışan cihazlar (BLE modülleri, bazı sensörler) için idealdir.
    
- *GND (Toprak):* Elektrik devresini tamamlamak için gereken toprak (ground) bağlantısıdır. *Her devrede mutlaka bir GND bağlantınız olmalı!*
    
- *RESET:* Bu pini toprağa (GND) kısa süreliğine bağladığınızda, tıpkı karttaki reset butonuna basmış gibi Arduino'yu yeniden başlatır.
    

#### *2. Dijital Pinler (0-13)*

Bu pinler hem *giriş (input)* hem de *çıkış (output)* olarak kullanılabilir. Yani bir düğmeden sinyal okuyabilir veya bir LED yakabilirsiniz. Sadece iki değer alırlar: *HIGH (5V)* ve *LOW (0V)*.

- **~ İşaretli Pinler (3, 5, 6, 9, 10, 11):** Bu pinlerin özel bir yeteneği vardır: *PWM (Pulse Width Modulation - Darbe Genişlik Modülasyonu)*. PWM, dijital bir pini kullanarak analog bir sinyal taklidi yapmamızı sağlar. Bir LED'in parlaklığını ayarlamak veya bir servo motoru kontrol etmek için bu pinleri kullanırız.
    

#### *3. Analog Pinler (A0-A5)*

Bu pinler isimlerinden de anlaşılacağı gibi, *analog sinyalleri okuyabilen* giriş pinleridir. Dijital pinlerin aksine, sadece iki değer değil, 0 ile 5V arasındaki gerilimi ölçerler (1024 farklı seviyede, 0-1023). Potansiyometre, LDR (ışık sensörü), sıcaklık sensörü gibi bileşenlerden gelen değerleri okumak için kullanılırlar.

- *Önemli Not:* Bu pinler aynı zamanda *dijital giriş/çıkış pini* olarak da kullanılabilirler (A0, A1, A2, ... şeklinde).
    

#### *4. Özel Amaçlı Pinler*

Bazı pinlerin Arduino ile iletişim veya belirli bileşenleri sürme gibi özel görevleri vardır.

- *Serial Communication (Seri İletişim - 0 (RX) ve 1 (TX)):*
    
    - *RX (Receive):* Veri alım pini.
        
    - *TX (Transmit):* Veri gönderim pini.
        
    - Bilgisayarınızla seri monitör üzerinden haberleşmek veya Bluetooth modülü gibi cihazlarla iletişim kurmak için kullanılır. Bu pinlere devre takarken dikkatli olun, yanlış kullanım bilgisayarla iletişimi kesebilir.
        
- *External Interrupts (Harici Kesmeler - 2 ve 3):*
    
    - Bu pinler, ana program akışını anında durdurup özel bir fonksiyon çalıştırabilir. Örneğin, bir butona her basıldığında ana kodunuz ne yapıyor olursa olsun durur ve sizin tanımladığınız fonksiyonu çalıştırır. Çok hızlı tepki gerektiren işlemler için idealdir.
        
- *SPI Communication (10 - SS, 11 - MOSI, 12 - MISO, 13 - SCK):*
    
    - SPI protokolü, birden fazla cihazla hızlı veri alışverişi için kullanılır. SD kart modülleri veya RFID okuyucular genellikle SPI kullanır.
        
    - *MOSI:* Master'dan Slave'e veri gönderir.
        
    - *MISO:* Slave'den Master'a veri alır.
        
    - *SCK:* Senkronizasyon için saat sinyalidir.
        
    - *SS:* Hangi slave cihazla konuşulacağını seçer.
        
- *I²C Communication (A4 - SDA, A5 - SCL):*
    
    - I²C protokolü, sadece iki pinle (SDA ve SCL) birden fazla cihazı kontrol etmenizi sağlar. Sensör modülleri, LCD ekranlar gibi birçok cihaz I²C kullanır.
        
    - *SDA:* Veri iletişim hattı.
        
    - *SCL:* Senkronizasyon için saat hattı.
        

### *Sonuç*

Arduino pinleri, projelerinize hayat veren en temel unsurlardır. Hangisinin ne işe yaradığını öğrenmek, daha karmaşık ve yaratıcı projeler geliştirmenizin ilk adımıdır. Doğru pini doğru yerde kullanmak, hem devrenizin doğru çalışmasını sağlar hem de Arduino kartınızı olası hasarlardan korur.

Artık pinlerin dilinden anlıyorsunuz! Şimdi sıra, bu bilgileri kullanarak kendi devrelerinizi kurup kodlamaya geldi. Bol makerali projeler!