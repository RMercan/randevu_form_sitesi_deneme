# CLAUDE.md

## Proje
Bu bir tanıtım sayfası projesi.

## Ne satıyor
Kadıköy'deki Moda İskelesi Vapur Kafe'yi tanıtan tek sayfalık bir tanıtım sitesi. Sayfada tanıtım, menü bağlantısı ve iletişim formu var. Menü PDF olarak şu linkte:

https://files.sehirhatlari.istanbul/menu-tr.pdf

## Kim görecek
Kadıköy'de yaşayan insanlar.

## Kurallar
- Tek dosya: `index.html`. CSS ve JS dosyanın içinde.
- Dışarıdan kütüphane çekme: CDN, framework, font servisi, Tailwind, placeholder görsel servisi yok.
- İçi boş pazarlama cümlesi yok.
- Uydurma referans yok: sahte yorum, sahte isim, sahte puan yazma. Bilmediğin bilgiyi (fiyat, saat, adres) uydurma, boş bırak veya kullanıcıya sor.
- İçerik Türkçe.
- Kod İngilizce: sınıf, id, değişken, fonksiyon ve kod yorumları İngilizce yazılır. Sayfada görünen metinler Türkçe kalır.
- Mobile-first, responsive.

## Her Zaman Önce
- Frontend kodu yazmadan önce `frontend-design` skill'ini çağır.

## Referans Görsel
- Referans görsel verilirse: yerleşim, boşluk, tipografi ve renkleri birebir eşle. Tasarımı "iyileştirme", referansta olmayan bölüm veya özellik ekleme.
- Referans yoksa: aşağıdaki kurallarla özenle sıfırdan tasarla.

## Yerel Sunucu ve Ekran Görüntüsü
- `file:///` adresinden ekran görüntüsü alma; sayfayı localhost üzerinden sun.
- Sunucu zaten çalışıyorsa ikincisini başlatma.
- Ekran görüntüsünü al, tasarımla karşılaştır, farkları düzelt. En az 2 tur yap.
- Karşılaştırırken somut ol: "başlık 32px ama 24px olmalı" gibi.
- Kontrol et: boşluklar, font boyutu/ağırlığı/satır yüksekliği, renkler (tam hex), hizalama, border-radius, gölge, görsel boyutları.

## Marka Varlıkları
- Tasarımdan önce `brand_assets/` klasörüne bak (logo, renk rehberi, görseller olabilir).
- Orada varlık varsa kullan, yerine placeholder koyma. Renk paleti tanımlıysa tam değerlerini kullan, marka rengi uydurma.

## Jenerik Görünümden Kaçınma
- **Renkler:** Varsayılan mavi/indigo yok. Özel bir ana renk seç, diğerlerini ondan türet.
- **Gölgeler:** Düz tek katmanlı gölge yok. Düşük opaklıkta, renk tonlu, katmanlı gölge kullan.
- **Tipografi:** Başlık ve gövde aynı font olmasın. Harici font yüklemeden sistem fontlarıyla (serif başlık + sans gövde gibi) eşleştir. Büyük başlıklarda dar harf aralığı (`-0.03em`), gövdede geniş satır yüksekliği (`1.7`).
- **Gradyanlar:** Birden çok radial gradient katmanla. Gerekirse satır içi SVG noise filtresiyle doku ekle.
- **Animasyon:** Sadece `transform` ve `opacity` animasyonu. `transition: all` yok.
- **Etkileşim durumları:** Tıklanabilir her öğede hover, focus-visible ve active durumu olsun.
- **Görseller:** Harici görsel çekme. Görsel gerekiyorsa satır içi SVG ya da CSS ile üret; üzerine gradyan katmanı ekleyebilirsin.
- **Boşluk:** Rastgele değil, tutarlı boşluk değerleri kullan.
- **Derinlik:** Yüzeyler katmanlı olsun (zemin → yükseltilmiş → yüzen).

## Sert Kurallar
- Kullanıcının vermediği içerik ekleme.
- Tek ekran görüntüsü turuyla bırakma.
- `transition: all` kullanma.
- Varsayılan mavi/indigo ana renk kullanma.
