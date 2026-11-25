# Rangers Instant

Dijital fotoğrafları Instax / Polaroid tarzı instant film karesine çeviren, tarayıcıda çalışan tek dosyalık uygulama. Fotoğraflar cihazdan dışarı çıkmaz; tüm işlem tarayıcıda yapılır.

A single-file browser app that turns digital photos into Instax / Polaroid style instant film frames and lays them out on photo paper for printing. Everything runs locally in the browser.

`index.html` is generated from `src/rangers-instant.html` in the main project by `publish.sh`.

## Sürümler / Releases

### v1.5
- Baskı sayfalarında kareler tam piksele oturuyor ve 1:1 kopyalanıyor; önceden yarım piksel kayma ve %0,02 ölçek farkı yüzünden tüm kare yeniden örnekleniyor, hafif yumuşuyordu.
- Baskı keskinleştirmesi artık yalnızca baskı dosyasına uygulanıyor (telafi gibi); önizlemede görmek için "Telafi ve keskinleştirmeyi önizlemede de göster".
- Marka okunur boyutta: yazılar 300 dpi baskıda yaklaşık 5 punto, şerit ve logo büyüdü.
- Marka daha net basılıyor: logo, kask ve dart tam piksel boyutunda önceden hazırlanıp hafifçe keskinleştiriliyor; yazılar, çizgiler ve ikonlar tam piksele oturuyor. Belirginlik varsayılanı %100.
- Kenar gölgesi varsayılanı 80.
- Bilgisayarda sayfayı ilk kaydırınca başlık küçülürken panelin zıplaması giderildi.
- Baskı JPEG kalitesi %95'ten %98'e çıktı.
- Yeni kâğıt boyutu: 15 × 21 cm.

### v1.4
- Marka (yeni 6. bölüm), çerçevenin kalın kenarına, notun altına basılır. İki seçenek var:
  - "Köşe imzası": küçük logo ve "made by RANGERS INSTANT" yazısı.
  - "Şerit": logonun renklerinde ince bir bant. Üzerinde dik kask, dart, fotoğraf karesi ve aynı yazı tekrar eder; bant kart kenarlarında kesilir.
  - "Şeffaf şerit": aynı şerit, krem zemin ve siyah çizgiler olmadan; yalnızca renkli çizgiler kalır.
- Belirginlik ayarlanabilir ve seçim hatırlanır. Marka önizlemede, indirilen karede ve baskıda görünür.

### v1.3
- İndirilen PNG ve baskı JPEG'lerine 300 dpi bilgisi yazılıyor; yazdırma uygulamaları gerçek boyutu (ör. 54 × 86 mm) doğru alıyor.
- Kart köşe yarıçapı küçültüldü (Instax 1,5 mm, Polaroid 1 mm).

### v1.2
- Kâğıt fotoğraf çerçevenin altında duruyor gibi: çok hafif yuvarlatılmış fotoğraf penceresi ve çerçevenin fotoğrafa düşen iç gölgesi (Çerçeve panelinde "Kenar gölgesi" ayarı).
- Tek kare indirme kendi bölümünde; siyah kenar ve baskı telafisi varsayılan olarak kapalı, telafi açıklaması netleştirildi.
- Fotoğraf görünümünde yalnızca kesikli çizgi ipucu; format ve indirme ikonlarındaki kaymalar düzeltildi.
- Bilgisayarda aşağı kaydırınca önizleme ve Fotoğraf/Kare seçici artık başlığın altında kalmıyor.

### v1.1
- Tek kare indirme: yuvarlak köşe (varsayılan, köşe dışı şeffaf) veya köşeli; isteğe bağlı siyah kenar.
- Marker yazı tipine Türkçe karakterler: Ş ş Ğ ğ İ ı ve noktalı i.
- Telefonda iki satırlık, düzenli ipucu kutusu.
- Bilgisayarda sabit başlık ve sekmeler, değişen değerlerde "sıfırla" ipucu, baskı listesinde not öncelikli isimler.

### v1.0
- İlk sürüm: Stüdyo (kenar/eğim düzeltme, film görünümleri, notlar) ve Baskı (çoklu kare yerleşimi).
