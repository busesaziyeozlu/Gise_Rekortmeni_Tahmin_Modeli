<img width="1663" height="1079" alt="image" src="https://github.com/user-attachments/assets/e4ecdaf1-24d4-4e30-a512-b142b400a784" />
Veri Bilimi ile Gişe Rekortmeni Filmlerin Şifresini Çözmek: Bir Uçtan Uca Analiz Projesi
Sinema dünyasında bir filmin "Hit" olması tesadüf mü, yoksa verilerle öngörülebilir bir matematik mi? 
Son projemde, TMDB 5000 veri setini kullanarak film endüstrisinin finansal ve sosyal dinamiklerini analiz eden kapsamlı bir makine öğrenmesi hattı kurdum. İşte projenin teknik yolculuğu ve elde ettiğim çarpıcı bulgular:
Veri Mühendisliği ve Hazırlık
Enflasyon Normalizasyonu: Farklı yıllara ait bütçe ve hasılat verilerini adil kıyaslayabilmek için CPI (Tüketici Fiyat Endeksi) kullanarak tüm finansal değerleri günümüze modernize ettim. 

Feature Engineering: Sektörel içgörüleri modele yansıtmak adına; oyuncuların piyasa değerini ölçen Cast Score, yönetmenlerin başarı oranını simgeleyen Director Score ve stüdyo gücünü yansıtan Production Company Score gibi yeni metrikler türettim. 

Ağırlıklı Puanlama: Ham puanlar yerine, oy sayısını da hesaba katan Weighted Rating sistemi ile daha güvenilir bir "kalite" metriği oluşturdum. 

Temel Analiz Bulguları (EDA)
Bütçe vs. Kâr: Enflasyon düzeltmesi yapıldığında bütçe ile hasılat arasındaki korelasyonun zayıfladığı görüldü. Bu, yüksek bütçenin tek başına başarıyı garantilemediğini, risk yönetiminin kritik olduğunu kanıtlıyor. 

Türlerin Gücü: Aksiyon, Macera ve Animasyon türleri ticari olarak en yüksek ortalama geliri üretirken; "Hit" filmlerin büyük çoğunluğu geniş kitlelere hitap eden bu türlerde yoğunlaşıyor. 

Mevsimsellik: Gişe gelirlerinin Mayıs-Haziran (Yaz dönemi) ve Kasım-Aralık (Tatil dönemi) aylarında zirve yaptığı mevsimsel bir örüntü tespit edildi. 

Modelleme ve Performans
Bir filmin "Hit" olup olmayacağını tahmin etmek için dört farklı algoritmayı karşılaştırdım:
Random Forest Classifier (Şampiyon model 🏆)
XGBoost
LightGBM
MLP (Yapay Sinir Ağları)
Sonuç: Random Forest, hem %92.58'lik doğruluk oranı hem de 0.85'lik F1-Skoru ile en dengeli ve başarılı performansı sergiledi. Kurduğum "Tahmin Motoru" sayesinde yeni projelerin gişe potansiyeli artık verilerle analiz edilebiliyor. 

Veri bilimi, sanatın yaratıcılığını öldürmez; aksine stratejik kararlar alabilmek için görünmez örüntüleri gün ışığına çıkarır. 
