# 🛠️ Ortak kurulum

> **Bu belge:** İlk kurulumda ve sürüm uyuşmazlığında kullanılır. Motor sürümünü tahmin etmez.

| Ayar | Durum |
|---|---|
| Unreal tam sürüm/build ve dağıtım | BEKLİYOR |
| C++ araçları ve Windows SDK | BEKLİYOR; motor gereksinimiyle eşleştirilecek |
| Proje/modül adı | BEKLİYOR |
| Proje konumu | Öneri: repo kökü; değişirse ignore/sahiplik yolları güncellenir |
| Ortak eklentiler ve sürümleri | BEKLİYOR |

1. GitHub Desktop'ta kendi hesabınla oturum aç.
2. `File > Clone repository > URL`: `https://github.com/Oxeen46/JAMciler`.
3. Disk yolları aynı olmak zorunda değil. Safa'nın gözlenen yolu `C:\Projects\JAMciler`.
4. `Current branch` bölümünden kendi isimli branch'ini seç; henüz yoksa Ufuk'la koordine et.
5. LFS kurulumunu doğrula: terminalde `git lfs version`; yerel kopyada `git lfs install`.
6. Proje geldiğinde `git lfs pull` ile gereken büyük dosyaları al. Dosyada yalnız `version https://git-lfs...` metni varsa gerçek varlık indirilmemiştir.
7. Tablodaki motor, araçlar ve eklentileri kur. Kişisel kararla sürüm yükseltme.
8. C++ proje dosyalarını üret; Editor hedefini uygun geliştirme yapılandırmasıyla derle; `.uproject` aç.
9. Test haritasında Play yap. Sorunu [açılış rehberi](06_UNREAL_SORUNLARI.md) ile incele.

> [!IMPORTANT]
> Dört bilgisayarda temiz clone + LFS indirme + derleme + açılış ayrı doğrulanır. GitHub'da dosyaları görmek bunun yerine geçmez.
