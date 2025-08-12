# Risk Analizi Projesi
Bu proje, kullanıcı giriş davranışlarını analiz ederek anomali tespiti ve risk değerlendirmesi yapmak için geliştirilmiştir. Proje, Python ve derin öğrenme teknikleri kullanılarak oluşturulmuş bir risk analizi sistemini içermektedir.

---

## Proje Açıklaması
Bu proje, bir şirketin iç sistemlerine yapılan kullanıcı girişlerini analiz ederek olağandışı davranışları tespit etmeyi ve risk skorları hesaplamayı amaçlamaktadır. Sistem, kullanıcıların alışkanlıklarını (IP adresi, giriş saati, kullanılan cihaz ve yazılımlar vb.) baz alarak her giriş için bir risk skoru üretir ve bu skora göre girişleri sınıflandırır.

---

### Özellikler
Mock Veri Üretimi: Gerçekçi kullanıcı giriş verileri oluşturulmuştur.

Risk Skorlama: Çeşitli risk faktörleri (IP değişikliği, MFA yöntemi, mesai saatleri dışı giriş vb.) kullanılarak her giriş için risk skoru hesaplanır.

Derin Öğrenme Modeli: LSTM tabanlı bir model ile risk skorlarının tahmin edilmesi sağlanır.

Anomali Tespiti: Kullanıcı davranışlarındaki anormallikler tespit edilir.

### Veri Seti
Projede kullanılan veri seti aşağıdaki özellikleri içermektedir:

personel_ID: Kullanıcı kimliği

MFAMethod: Çok faktörlü kimlik doğrulama yöntemi

CreatedAt: Giriş tarih ve saati

ClientIP: Kullanıcı IP adresi

Application: Erişilen uygulama

Browser: Kullanılan tarayıcı

OS: İşletim sistemi

Unit: Kullanıcının departmanı

Title: Kullanıcının unvanı

is_anamoly: Anomali olup olmadığı (1: Anomali, 0: Normal)

risk_score: Hesaplanan risk skoru

risk_level: Risk seviyesi (HIGH, MEDIUM, LOW, NORMAL)
