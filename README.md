Web tasarımı dersi projesi için modern tasarımlı, kullanıcı hareketlerine duyarlı bir web sayfası tasarlanmamız istendi. Bu kapsamda "Nova Sigorta" ismiyle modern web sayfalarına benzer ve işlevsel bir web sitesi geliştirildi.

# II.Proje Gereksinimlerinin Analizi

Projeyi geliştirmeye başlamadan önce sektörde ileri gelen şirketlerin(Allianz\[1\], Axa\[2\], Anadolu Sigorta\[3\],Türkiye Sigorta\[3\], HDI Sigorta\[4\]) web sayfaları incelendi. Bu sayfalarda yer alan özellikler incelenerek proje için bir şablon seçildi. Şablonun teması güveni ve sakinliği simgelemek amaçlı Mavi ve Beyaz renklerden oluşuyor.  

Proje için gereken temel özellikler:  

*   Menü kısmında Hakkımızda, Misyon-Vizyon, Hizmetler, Birimler, İletişim, İstatistikler sayfaları bulunmalı.
    
*   Kullanıcı hizmetleri ve birimleri inceledikten sonra teklif almak için karşı tarafa ulaşabilmeli.
    
*   Sayfaya yönetici tarafından yeni duyuru eklenebilmeli.
    
*   Kullanıcı arayüzü kullanımı basit ve kolay erişilebilir olmalı.
    
*   Site ekran boyutu farketmeksizin akıcı çalışmalı.
    
*   Anasayfada şirket ve hizmetler hakkında detaylı bilgilere ulaşılabilmeli, burada ayrıca müşteri yorumları, SSS bölümü vb. bulunmalı.
    

# III.Sistemin Mimarisi

Proje iki temel yapıdan (Admin paneli ve Kullanıcı arayüzü) oluşmakta.

Projede kullanıcılara gösterilecek bir duyuru ekleme yapısı ve kullanıcıdan form alma yapısı olması istendiği için bunların gerçekleştirileceği bir Admin paneli yapısı oluşturuldu. Burada admin tarafından duyuru girişi yapılabiliyor ve kullanıcının gönderdiği mesaj görüntülenebiliyor.

Kullanıcı arayüzünde ise kullanıcının rahatça gezinebildiği, sayfalara erişimi kolay bir yapı oluşturuldu.

# IV.karşılaşılan zorluklar ve çözümler  

### 1)Bazı resimlerin görüntülenememesi:

Sayfalara resim eklendikten sonra çalıştırıldığında bazı resimler görüntülenemiyordu. Bu durumu çözmek için FileReader API kullanarak resimleri URL’ye dönüştürüp metin olarak tarayıcı hafızasında saklayan bir yapı oluşturuldu.  

### 2)Açılır pencere yapısı:

Menü kısmında istenen hizmetler ve birimler butonlarının açılır pencere halinde olması yapısını oluşturmak için diğer butonlardan farklı olarak bir dropdown yapısı eklendi.  

### 3)İletişim sayfası:

Kullanıcının bilgilerini girerek şirkete email gönderdiği bir yapı bulunması istendiği için, bunu sunucu tarafında yapmayan fakat web sayfasının olanaklarını kullanarak bir object yapısı oluşturuldu ve bu sayede mesajların yönetici tarafında görüntülendiği prototip bir yapı hazırlandı.  

### 4)Eklenen duyuruların anasayfada görünüp duyurular sayfasında görünmemesi:

 Bunu çözmek için daha önceden duyurular sayfasına özel hazırlanan duyuru ekleme modal yapısı yerine iki sayfada da aynı modal yapısını kullanarak sayfalar senkronize hale getirildi.  

### 5)Header ve Footer yapısı:
 Site içeriğindeki her sayfada header ve footer kısımlarının güncel haliyle bulunması gerekliliği karşılandı.
