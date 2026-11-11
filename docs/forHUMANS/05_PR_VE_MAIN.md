# 📥 PR ve main

> **Bu belge:** Teslim yapan kişi ve Ufuk için birleştirme adımlarını açıklar.

## Teslim yapan kişi

1. Güncel main'i kendi branch'ine al; tekrar derle/test et.
2. GitHub `Pull requests > New pull request`: base `main`, compare kendi ismin.
3. Değişen dosyaları incele; şablonu doldur.
4. Ufuk'u incelemeye çağır; hesabı henüz eşleşmemişse ekip kanalında bildir.

## Ufuk

1. Doğru branch, görev kapsamı, sahiplik ve test sonucunu kontrol et.
2. Ortak sistem değişikliklerinde entegre davranışı yerelde dene.
3. Hata varsa sahibine ver. Herkesin işini yeniden yazmak zorunda değilsin.
4. Hazır PR'ı normal **merge commit** ile birleştir. Sürekli isimli branch'lerde şimdilik squash/rebase yok.
5. Kişisel branch'i silme; main güncellemesini ekibe bildir.
6. Kendi PR'ını başka ekip üyesi incelesin; onaydan sonra sen birleştirebilirsin.

## Çakışma

1. Metin dosyasında iki değişikliğin amacı anlaşılmadan taraf seçmeyin; sahibi çözer ve test eder.
2. `.uasset/.umap/.blend` metin gibi birleştirilmez. Hangi sürüm korunacak sahibi belirler; diğer iş gerekiyorsa yeniden uygulanır.
3. Genel `ours/theirs`, discard/reset veya force-push çözümü kullanmayın.

## GitHub ayarı — henüz uygulanmadı

- Public main için PR, en az bir başka kişinin onayı, görüşmelerin çözülmesi; force-push/silme kapalı önerilir.
- Ufuk günlük merge sorumlusu; yedek seçilecek.
- Hesap türü/ayar desteği görülmeden yalnız Ufuk'un teknik merge yetkisi olduğu iddia edilmez. CODEOWNERS tek başına yazma kilidi değildir.
- Başlangıçta bulut Unreal derleme otomasyonu yok; yerel test/paketleme gerekir.
