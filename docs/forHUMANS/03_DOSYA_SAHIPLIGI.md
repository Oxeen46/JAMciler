# 📂 Dosya sahipliği

> **Bu belge:** İnsanlar ve ajanlar için tek sahiplik kaynağıdır. Yollar, proje açılınca uygulanacak tasarımdır; mevcut dosya iddiası değildir.

| Kişi | Branch | Paket | Ek rol |
|---|---|---|---|
| Ufuk | `Ufuk` | SEÇİLMEDİ | main merge sorumlusu |
| Safa | `Safa` | SEÇİLMEDİ | — |
| Canberk | `Canberk` | SEÇİLMEDİ | — |
| Mustafa | `Mustafa` | SEÇİLMEDİ | — |

**Ufuk'un GitHub hesabı ve yedek merge sorumlusu:** BEKLİYOR. İsimlerden hesap adı türetilmez.

| Sahip | Düzenlediği yollar |
|---|---|
| A | `Content/JAM/Maps/Main/`, `Content/JAM/LevelData/` |
| B | `Source/<Modul>/Player/`, `Content/JAM/Characters/`, `Content/JAM/Input/`, `Content/JAM/Tests/B/`, `SourceArt/Characters/` |
| C | `Source/<Modul>/Mechanics/`, `Content/JAM/Mechanics/`, `Content/JAM/Environment/`, `Content/JAM/Tests/C/`, `SourceArt/Environment/` |
| D | `Source/<Modul>/Flow/`, `Source/<Modul>/UI/`, `Source/<Modul>/Shared/`, `Content/JAM/UI/`, `Content/JAM/Audio/`, `Content/JAM/Tests/D/`, `SourceArt/Presentation/` |
| D, koordine ederek | `.uproject`, `Config/`, `Build/`, `Plugins/`, modül başlangıcı, `*.Build.cs`, `*.Target.cs` |
| Ufuk, ekip kararıyla | Repo ayarları, `.github/`, Git filtreleri ve ortak belgelerde kabul edilen değişiklikler |

1. Başkasının alanını okumak/oynayarak test etmek serbest; görev dışı kaydetmek ve göndermek değil.
2. Ana haritayı yalnız A kaydeder. Diğerleri kendi test haritalarını kullanır.
3. Model kaynağı ve Unreal varlığı aynı sahipte kalır. A yerleştirir, reimport etmez.
4. Haritaya bağlı external actor/object ve built-data da aynı sahibindir. OFPA/World Partition seçilirse ilgili yollar çalışma başlamadan tabloya eklenir.
5. Ortak materyalin tek sahibi olur. Geniş taşıma/rename, reimport ve redirector düzeltmesi koordine edilen ayrı görevdir.
6. Devir: kartta eski/yeni sahip → eski sahibi commit/push → yeni sahibi güncel main'i alır → tablo güncellenir → çalışma başlar.

> [!WARNING]
> Belge veya branch adı teknik kilit değildir. PR'da yollar incelenir. Hesap/paket eşleşmesi yapılmadan otomatik alan kontrolü etkin sayılmaz.
