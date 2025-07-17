# HayvanatBahcesiSimulasyonu-SelamiCetin-Python
🦁 Hayvan Ekosistemi Simülasyonu Projesi
Bu proje, Python kullanarak bir ekosistemdeki hayvan popülasyonlarının davranışlarını, üremelerini ve av-avcı ilişkilerini simüle eden bir simülasyon sistemidir.

🌟 Öne Çıkan Özellikler
Gerçekçi hayvan davranışları: 7 farklı hayvan türü ve avcı

Dinamik üreme mekaniği: Cinsiyet temelli çiftleşme ve yavru oluşumu

Av-avcı ilişkileri: Türe özgü avlanma mesafeleri ve stratejileri

Rastgele hareket: Her türün kendine özgü hareket mesafesi

İstatistiksel çıktılar: Simülasyon sonunda popülasyon raporu

🛠️ Kurulum ve Çalıştırma
Gereksinimler:

bash
pip install numpy matplotlib
Kodu çalıştırma:

bash
python main.py
📊 Örnek Çıktı
text
📊 1000 Adım Sonunda Hayvan Popülasyonu:
Sheep    : 42
Cow      : 18
Chicken  : 35
Rooster  : 28
Wolf     : 9
Lion     : 7
Hunter   : 1

⏱️ Simülasyon Süresi: 1.24 saniye
Toplam Hayvan Sayısı: 140
📂 Dosya Yapısı
Dosya Adı	Açıklama
animal.py	Hayvan sınıfı ve temel davranışlar
simulation.py	Simülasyon motoru ve iş mantığı
main.py	Program giriş noktası ve sonuç raporlama
🧠 Simülasyon Mantığı
Başlangıç Popülasyonu:

30 koyun, 10 inek, 20 tavuk/horoz

10 kurt, 8 aslan ve 1 avcı

Her Adımda:

Tüm hayvanlar rastgele hareket eder

Yakın hayvanlar çiftleşir ve yavru doğurur

Avcılar belirli mesafedeki avları yakalar

Üreme Kuralları:

Erkek-dişi çiftleri 3 birim mesafede çiftleşir

Tavuk/horoz aynı tür olarak kabul edilir

Yavrular ebeveynlerin ortasında doğar

🌍 Ekosistem Kuralları
Avcı	Av Hedefleri	Mesafe
Kurt	Koyun, Tavuk, Horoz	4 birim
Aslan	İnek, Koyun	5 birim
Avcı	Tüm hayvanlar (kendi türü hariç)	8 birim
📈 Olası Geliştirmeler
Gerçek zamanlı görselleştirme

Çevresel faktörler (su kaynakları, bitki örtüsü)

Genetik özellik aktarımı

Mevsimsel değişiklikler

Popülasyon grafiklerinin kaydedilmesi

Bu proje, ekosistem dinamiklerini anlamak için harika bir başlangıç noktası oluşturmakta ve biyolojik çeşitliliğin korunmasına yönelik çalışmalara ilham verebilmektedir.


graph TD
    A[Simülasyon Başlat] --> B[Popülasyonu İlkile]
    B --> C{Adım Sayısı 1000 mi?}
    C -->|Hayır| D[Tüm Hayvanları Hareket Ettir]
    D --> E[Üreme Kontrolü]
    E --> F[Avlanma Kontrolü]
    F --> C
    C -->|Evet| G[Popülasyon Raporu Oluştur]
    G --> H[Sonuçları Göster]
