# 🔄 Günlük GitHub Desktop

> **Bu belge:** Günlük alma/gönderme adımlarını gösterir. Menü adları uygulama dili/sürümüne göre küçük fark gösterebilir.

## 🟢 Başlangıç

1. Doğru repo ve kendi isimli branch'inde olduğunu kontrol et.
2. Önceki çalışmanı editörde kaydet, değişen dosyaları incele ve commit et. Bitmemiş işi main'e gönderme.
3. Unreal'ı ve dosya yazan ajanları kapat/durdur. Branch/varlık güncellerken editör açık kalmasın.
4. `Fetch origin`; kendi uzak branch'inde yeni kayıt varsa `Pull origin`.
5. Kendi branch'indeyken `Branch > Merge into current branch` ile güncel `origin/main`i seç. Listelenmiyorsa temiz çalışma durumunda main'e geç → Pull → kendi branch'ine dön → main'i birleştir.
6. Çakışma varsa dur, [sahibiyle çöz](05_PR_VE_MAIN.md). Sonra gerekliyse derle, Unreal'ı aç.

> [!IMPORTANT]
> Kişisel branch'te Pull, main'i otomatik getirmez. Adım 5 ayrıca gerekir. Kendi çalışmanı silmiyorsun; iki çizgiyi birleştiriyorsun.

## 🟢 Teslim

1. Kendi test haritanda dene; C++ değiştiyse derle.
2. Değişen dosyaları tek tek kontrol et. Görev dışı dosya varsa sebebini çözmeden gönderme.
3. Açıklayıcı commit: örneğin `Etkileşim mesafesi kontrolünü ekle`.
4. `Push origin` (ilkinde `Publish branch`).
5. Hazırsa [PR aç](05_PR_VE_MAIN.md). Hazır değilse kişisel branch'inde kalır.
6. Merge sonrasında yeni işe başlamadan ortak sürümü kendi branch'ine al.

## Tek görev listesi

GitHub Issues kullanılır: sahip, paket, izinli yollar, sonuç ve test. Önce aynı işin kartı var mı bak. Ajan Issue okuyamıyorsa görev metnini ona ver; ikinci görev listesi açma.
