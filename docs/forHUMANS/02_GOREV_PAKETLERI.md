# 🧩 Görev paketleri — isimleri siz seçin

> **Bu belge:** Her paketin işini, sınırını ve teslimini tanımlar. Ufuk'un merge görevi ayrı; hiçbir oyun paketi bir kişiye atanmadı.

> [!IMPORTANT]
> Fikir bilinmeden saat eşitliği garanti edilemez. Puanlar göreli plan bütçesidir, saat değildir. Her paket 20 puanla başlar; ilk prototipten sonra kalan yük yeniden ölçülür.

## 🟦 A — Bölüm ve dengeleme; sınırlı AI

AI yalnız küçük kod desteği; üretim çoğunlukla insanın Unreal editöründeki çalışmasıdır.

| İş | Puan | Bitti sayılması |
|---|---:|---|
| Ana harita taslağı ve rota | 5 | Başlangıçtan sona izlenebilir rota |
| Hazır sistemlerin ana haritaya yerleşimi | 5 | Onaylı oyuncu/mekanik sürümleri birlikte çalışır |
| Işık, çevre yerleşimi ve çarpışmalar | 4 | Oyuncu takılmadan ilerler; hedef anlaşılır |
| Zorluk, süre ve başlangıç noktası ayarları | 3 | Sunulan editör değerleriyle dengelenir |
| Bölüm testi ve kendi düzeltmeleri | 3 | Bölüm baştan sona tamamlanabilir |

**Teslim:** Ana harita ve bölüm ayarları. **Dokunmaz:** B/C/D kodu, model reimport, proje genel ayarları. Başkalarının sistem hatalarını düzeltmek A'nın işi değildir.

## 🟩 B — Oyuncu ve karakter

| İş | Puan | Bitti sayılması |
|---|---:|---|
| C++ hareket, kamera, oyuncu girdileri | 6 | Test haritasında kontrol edilebilir |
| Etkileşim çağrısı | 3 | Ortak sözleşmeyle C nesnelerine ulaşır |
| Oyuncu modeli, iskelet, temel animasyon | 5 | Ölçek ve temel geçişler doğru |
| D için oyuncu olayları | 2 | Arayüz/ses bağlanabilir |
| Test, derleme, düzeltme | 4 | Kontrol kaybı ve temel hatalar giderilmiş |

**Teslim:** Oyuncu sistemi, karakter varlıkları, B test haritası. **Dokunmaz:** Ana harita, hedef/menü akışı, C mekanik kodu.

## 🟧 C — Mekanik ve çevre varlıkları

| İş | Puan | Bitti sayılması |
|---|---:|---|
| Tek ana mekanik ailesi | 6 | Başlangıç/başarı/başarısızlık denenmiş |
| Aynı mekanizmanın sınırlı varyasyonları | 3 | Ayarlarla çeşitlenir |
| Sınırlı çevre modelleri ve materyalleri | 5 | Pivot, ölçek, çarpışma, doku boyutu kontrol edilmiş |
| Yerleştirme ayarları ve olay bağlantıları | 2 | A kod değiştirmeden kullanabilir |
| Test, derleme, düzeltme | 4 | C test haritasında çalışır |

**Teslim:** Yerleştirilebilir mekanikler/çevre varlıkları. **Dokunmaz:** Oyuncu sınıfı, ana harita, HUD. Karmaşık düşman, envanter veya kayıt sistemi otomatik ek görev değildir.

## 🟪 D — Akış, sunum ve ortak teknik yapı

| İş | Puan | Bitti sayılması |
|---|---:|---|
| Küçük ortak arayüzler ve proje ayarları | 4 | B/C'nin kullanacağı bağlantılar belli |
| Başlatma, kazanma/kaybetme, yeniden başlatma | 5 | Oyun döngüsü tamam |
| Sade menü/HUD ve ses bağlantıları | 5 | İngilizce, okunabilir, olaylara doğru tepki |
| İlk ve son paketlemeyi yürütme | 3 | Paket başka bilgisayarda açılır |
| Test ve kendi düzeltmeleri | 3 | D test haritasında/pakette doğrulanmış |

**Teslim:** Akış/sunum ve paketleme kaydı. **Dokunmaz:** B/C uygulama kodu, ana harita yerleşimi. Paketleme hatasını ilgili sistem sahibi düzeltir; tüm hatalar D'ye yüklenmez.

## Dengeleme ve iş sırası

1. İlk oturumda kalan yükü karşılaştırın. Yeni içerik ancak bu bütçeyle değerlendirilir.
2. Ufuk'un merge zamanı da iş yüküdür: seçtiği paketin opsiyonel cilasını azaltın veya ayrı dosya sahibi devriyle destek verin.
3. Herkes kendi üretimini test eder. Herkes bir kez başka teslimi oynayarak geri bildirim verir; dosyasını değiştirmez.
4. Ağırlaşan pakette önce kapsamı azaltın. Yardım gerekiyorsa [sahipliği devredin](03_DOSYA_SAHIPLIGI.md); iki kişi aynı dosyaya yazmasın.
5. Jam başlayınca D küçük ortak sözleşmeyi, A bölüm planını, B oyuncuyu, C mekanik prototipini hazırlar.
6. İlk hedef tek küçük bölümde başlangıç → oynanış → sonuç. İlk paket başka bilgisayarda denenir; sonra cila gelir.
