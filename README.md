# Linux Syslog Yönetimi - Çift Yönlü Bağlı Liste Uygulaması

Bu proje, Linux işletim sisteminde üretilen sistem günlüklerinin (Syslog) dinamik bellek yönetimi kullanılarak, Çift Yönlü Bağlı Liste (Doubly Linked List) veri yapısı ile RAM üzerinde nasıl tutulabileceğini ve işlenebileceğini gösteren bir C uygulamasıdır.

## 📌 Kullanılan Veri Yapısı ve Nedeni
Bu projede **Çift Yönlü Bağlı Liste** kullanılmıştır. 
**Nedeni:** Sistem günlükleri dosyaya eskiden yeniye doğru (kronolojik) yazılır. Ancak sistem yöneticileri bir problemi analiz ederken (debugging) logları genellikle en yeniden eskiye doğru okumaya ihtiyaç duyarlar. Çift yönlü bağlı listenin `tail` ve `prev` işaretçileri sayesinde, en son oluşan logdan geçmişe doğru gezinmek algoritmik olarak karmaşıklığı düşürür (O(1) sondan başlama maliyeti).

## 🚀 Kurulum ve Çalıştırma
Projeyi kendi bilgisayarınızda çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1. Repoyu klonlayın:
   ```bash
   git clone [https://github.com/KULLANICI_ADIN/repo-adi.git](https://github.com/KULLANICI_ADIN/repo-adi.git)
