# 🧱 C++ ve MCP standartları

> **Amaç:** Sistemlerin birbirini bozmadan bağlanmasını ve üretim araçlarının görev sınırında kalmasını sağlamak. Motor sürümü henüz belirlenmedi.

1. Oynanış mantığı C++ olur. Blueprint graph ile alternatif oynanış sistemi kurma. Asset ayarı/animasyon/UMG için motorun ihtiyaç duyduğu içerik türleri ayrıca kararlaştırılır; kullanıcı C++ dedi diye bunları habersiz yasaklama veya ekleme.
2. Tek dev karakter/GameMode sınıfına tüm ekip kodunu doldurma. Küçük sorumluluklar ve olaylar/aralıklar tanımla.
3. D ortak sözleşmeleri sahiplenir; B oyuncu girdisini, C nesne davranışını, D sonuç/HUD akışını uygular. Ortak imza değişikliği bağımlı sahiplerle koordine edilir.
4. A'nın düzenleyeceği değerleri uygun editör özellikleri/veri varlıkları üzerinden sun; yalnız uygun alanlar düzenlenebilir olsun. A kodu veya B/C varlıklarını yeniden kaydetmek zorunda kalmasın.
5. Gizli yerel mutlak disk yollarını kaynaklara yazma; taşınabilir proje-relative yollar kullan.
6. MCP işlemi öncesi bağlı proje/sahne kimliğini doğrula. Rastgele açık Unreal/Blender projesine yazma.
7. Üretilen model: lisans, ölçek, pivot, topoloji, doku boyutu, çarpışma ve gerekli animasyonları kontrol et. Önce kendi test haritana import et.
8. Araç hatasını kapsam dışı tüm proje ayarlarını değiştirerek çözme; kanıtı raporla.
9. API maliyeti doğuracak yeni ücretli aşım/abonelik etkinleştirme. Kampanya kodlarını repoya koyma.
