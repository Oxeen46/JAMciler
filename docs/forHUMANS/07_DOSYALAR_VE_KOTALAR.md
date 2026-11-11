# 💾 Yükleme ve GitHub Free kotaları

> **Bu belge:** İlk Unreal yüklemesinden önce ve büyük varlık gönderirken kullanılır. Resmî sınırlar 12 Kasım 2026'da kontrol edildi; hesabın mevcut tüketimi ayrıca kontrol edilmelidir.

## Ne yüklenir?

| Alan | Karar |
|---|---|
| `.uproject`, `Source/`, `Config/` | Evet; proje, C++ ve ortak ayarlar |
| `Content/` | Kullanılan varlıklar, haritalar ve bağımlılıkları; LFS |
| `Build/` | Gerekli ikon/platform/paketleme kaynakları evet; topluca dışlanmaz |
| `Plugins/` | Gerekli ve paylaşılabilir içerik; binary gereksinimleri tek tek incelenir |
| `SourceArt/` | Gerekli düzenlenebilir kaynaklar; lisans kontrolüyle LFS |
| Belgeler, Git ayarları | Evet |
| Proje `Binaries/`, `Intermediate/`, `Saved/`, `DerivedDataCache/` | Hayır; yerel üretilen dosyalar |
| IDE geçici dosyaları, üretilmiş solution | Hayır |
| Unreal motor kurulumu | Hayır; herkes motoru kurar |
| Paketlenmiş oyun/ZIP/video çıktıları | Kaynak Git geçmişine hayır; yerel `Artifacts/` veya teslim alanı |
| Anahtar/kupon/özel hesap bilgisi | Hayır |

> [!WARNING]
> Kaynağı olmayan eklentinin Binaries dosyaları gerekli olabilir. Tüm DLL/LIB dosyalarını dışlamak projeyi bozabilir. Public yeniden dağıtım lisansı olmayan varlığı repoya koymayın; yetkili ayrı kurulum gerekir.

## Sınırlar

| Limit | Free |
|---|---|
| Normal Git dosyası | 50 MiB üstünde uyarı; 100 MiB üstü engel |
| Tek Git push | 2 GiB; toplam repo kotası değildir |
| LFS tek dosya | 2 GB |
| Ücretsiz LFS depolama | 10 GiB; eski LFS sürümleri de sayılır |
| Ücretsiz LFS indirme | Dönem başına 10 GiB; repo sahibinin hesabından |

## Kotayı koruma

1. Git filtreleri büyük dosyaların ilk commit'inden önce hazır olsun.
2. LFS sıkıştırma değildir. Değişen dosyanın yeni tam sürümü depolama kullanır.
3. Örnek: 2 GiB LFS verisini üç arkadaş indirirse yaklaşık 6 GiB indirme tüketir. Sonraki yeni sürümler de tüketimdir.
4. Her Pull her dosyayı tekrar indirmez; gereksiz yeniden clone/toplu reimport yapmayın.
5. Büyük asset paketinin tamamı yerine gereken varlıkları bağımlılıklarıyla taşıyın. Gereksiz demo haritalarını/8K dokuları yüklemeyin.
6. Public olmak LFS'yi sınırsız yapmaz; dışarıdan indirme de kota etkileyebilir.
7. Repo sahibi kullanım/bütçe ekranını başlangıçta ve günlük kontrol eder. Ücretli aşım otomatik açılmaz. $0 bütçe maliyeti engeller fakat kota biterse LFS durabilir.
8. Dosyayı main'den silmek eski LFS sürümlerini otomatik temizlemez; geçmiş temizleme ayrı işlemdir.
9. `.gitignore`, önceden takip edilen dosyaları kendiliğinden takip dışına çıkarmaz.

## İlk aktarım kontrolü

- [ ] Her bilgisayarda LFS hazır.
- [ ] `git lfs ls-files` beklenen ikilileri gösteriyor.
- [ ] `git status` önbellek/anahtar/derleme çıktısı içermiyor.
- [ ] Eklenti ve varlık lisansları public paylaşım için uygun.
- [ ] Başka bilgisayarda clone + LFS + derleme + oyun testi geçti.

Kaynaklar:
- https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github
- https://docs.github.com/en/get-started/using-git/troubleshooting-the-2-gb-push-limit
- https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage
- https://docs.github.com/en/billing/concepts/product-billing/git-lfs
- https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-directory-structure
