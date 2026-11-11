# ✅ Test ve teslim

> **Amaç:** Yapılan işin denenmiş, kapsamı belli ve başka bilgisayara taşınabilir olmasını sağlamak.

1. Değişiklik öncesi/sonrası dosya listesini karşılaştır. Kendi alanı dışındaki beklenmeyen dosyaları sahibine bildir; körlemesine discard etme.
2. C++ değiştiyse derle. Live Coding sonucu tek başına temiz Editor build/paketleme başarısı değildir.
3. İlgili davranışı kendi test haritanda dene; başarı yanında anlamlı başarısızlık/yeniden başlatma durumunu kontrol et.
4. Başka sistemleri etkileyen ortak değişikliklerde entegre test gerekir.
5. `git diff --check`, LFS kapsamı ve filtreleri kontrol et. Gereksiz build, önbellek, API anahtarı veya lisanssız public dosya ekleme.
6. PR: görev, izinli alan, değişenler, denenen adımlar, yapılmayan kontroller ve bilinen sorunlar.
7. Test çalıştırılamadıysa nedenini açıkça yaz; başarılı gibi gösterme.
8. Oyunun ilk çalışır parçasında ve teslim öncesi başka bilgisayarda paket testi. Hataları ilgili paket sahibi düzeltir.
9. Son raporda yerel dosya / commit / push / PR / main / sunucu ayarı durumlarını ayrı belirt.
