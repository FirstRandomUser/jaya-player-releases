# Jaya Player — kullanım kılavuzu

Jaya Player, Android TV, TV kutuları ve akıllı telefonlar için bir IPTV oynatıcıdır.
Uygulama **TV kanalı veya içerik sağlamaz**: yalnızca kullanıcının eklediği oynatma listelerini oynatır.

---

## 1. Kurulum

1. Uygulamayı indirin: **https://github.com/FirstRandomUser/jaya-player-releases/releases/latest/download/jaya-player.apk** (her zaman en son sürüm) veya [Releases](https://github.com/FirstRandomUser/jaya-player-releases/releases/latest) sayfasından.
2. TV kutusunda **Downloader** uygulaması veya USB bellek kullanmak pratiktir.
3. İlk kurulumda Android bu kaynaktan yüklemeye izin vermenizi ister — izin verin.
4. Android 6.0 veya üzeri gerekir.

Sonraki güncellemeleri uygulama **kendisi** indirir ve kurar (bkz. bölüm 10).

---

## 2. İlk açılış ve oynatma listesi

İlk açılışta **Ayarlar** açılır.

1. **Oynatma listeleri → Ekle**'ye basın.
2. Türü seçin:
   - **M3U bağlantısı** — sağlayıcınızın verdiği liste adresi;
   - **Xtream Codes** — sunucu adresi, kullanıcı adı ve şifre;
   - **dosya** — cihazdaki veya USB bellekteki `.m3u` listesi.
3. **EPG** (yayın akışı) — XMLTV adresi. Genellikle sağlayıcının listesinde zaten bulunur, alan boş bırakılabilir. Yayın akışı görünmüyorsa EPG adresini sağlayıcınızdan öğrenip buraya yazın.
4. **Her … saatte güncelle** — liste ve yayın akışının ne sıklıkla güncelleneceği.
5. **Kaydet**'e basın. Yükleme arka planda sürer — hemen izlemeye dönebilirsiniz.

Birden fazla liste ekleyebilirsiniz. Güncelleme hatayla biterse (örneğin internet yoksa), uygulama bir sonraki açılışta kendiliğinden tekrar dener.

---

## 3. Uzaktan kumanda

| Tuş | İşlem |
|---|---|
| ▲ ▼ | önceki / sonraki kanal |
| ◀ | kanal listesi |
| ◀ ◀ (daha sola) | grup listesi |
| ▶ | Favoriler |
| ▶ ▶ (hızlı iki kez) | yayın istatistikleri (aç/kapat) |
| OK | bilgi paneli |
| OK tekrar | duraklat |
| duraklatmada OK | devam et |
| uzun OK | işlem menüsü (ses, altyazı, görüntü oranı, ayarlar) |
| rakamlar | numaraya göre kanala git |
| 0 | önceki kanal |
| iki kez Geri | çıkış |

**Kanal listesinde:**
- ▶ — seçili kanalın yayın akışı;
- uzun OK — işaretleme modu: ◀ Favorilere ekle/çıkar, ▶ kanalı sil (silinenler "Silinenler" grubundan geri alınabilir).

**Akıllı telefonda:** dokunma — duraklatma ve bilgi paneli; yukarı kaydırma — bilgi paneli, aşağı — gizle; sol yarıda sağa kaydırma — kanal listesi; sağ yarıda sola kaydırma — Favoriler; uzun dokunma — ayarlar.

---

## 4. Yayın akışı ve arşiv

- Yayın akışı **24 saat geriye ve 36 saat ileriye** saklanır.
- Kanal listesinde ▶'ye basın — yayın akışı açılır. Sağlayıcınız destekliyorsa geçmiş programlar **arşivden** izlenebilir.
- Arşivde: **OK** — ilerleme çubuğu, ◀ ▶ — adım (basılı tutunca hızlanır), **Geri** — canlı yayına dönüş.

---

## 5. Canlı yayını duraklatma (Timeshift)

**Ayarlar → Oynatma → Kayıtlı canlı duraklatma.**

- **Kapalı:** duraklatma görüntüyü durdurur; devam edince canlı yayına dönülür.
- **Açık:** duraklatmadan sonra izleme **aynı andan** devam eder. Canlıdan gecikme altta görünür; **Geri** — canlı yayına dönüş.

**Duraklatma kaydı depolaması:**
- **Dahili bellek** — kayıt duraklatma anında başlar ve kanal değiştirilince silinir.
- **Harici disk (USB)** — kanalı izlediğiniz sürece kayıt sürekli yapılır, bu yüzden **duraklatmada ◀ ▶ geri sarar** (yer yettiği kadar). Uygulama diskte `Timeshift` klasörü oluşturur ve boş alanın en fazla %80'ini kullanır; eski kayıtlar otomatik silinir.

USB bellek: FAT32 veya exFAT (cihazınız destekliyorsa NTFS).
DASH, şifreli akışlar ve ayrı ses kanallı akışlar desteklenmez — bunlarda duraklatma normal şekilde çalışır.

---

## 6. Gizli gruplar (ebeveyn denetimi)

1. Grup listesini açın (◀ ◀), bir grup seçin ve **OK'yi basılı tutun** — grup seçimi açılır.
2. Grupları OK ile işaretleyin ve **Geri**'ye basın.
3. Şifreyi oklarla girip OK'ye basın. Varsayılan şifre **▶ ▶ ▶ ▶**.
4. İlk gizlemeden sonra uygulama oklardan kendi şifrenizi oluşturmanızı önerir (örneğin ▲ ▲ ◀ ▶) — unutmayın.

Gizli grupları yeniden göstermek için grup listesinde **◀'ye hızlıca üç kez basın** ve şifreyi girin. Uygulama simge durumuna küçültülünce gruplar tekrar gizlenir.

---

## 7. Resim içinde resim ve arka plan (akıllı telefon)

- **Resim içinde resim:** ana ekrana geçince video küçük pencerede devam eder.
- **Arka planda ses:** ekran kilitlenince ses devam eder; kontrol bildirim panelinden yapılır.

---

## 8. Ayarlar

- **Ekran:** otomatik kare hızı, 120 Hz, bilgi paneli süresi, liste kaydırma, **OLED ekran** (yanma koruması: öğelerin kaydırılması, saatin gizlenmesi, duraklatmada ekran koruyucu, menülerin karartılması).
- **Saat:** ekrandaki konumu.
- **Oynatma:** resim içinde resim, arka planda ses, ses seviyesi dengeleme, istatistikler, canlı duraklatma, komşu kanalların ön yüklemesi, arabellek, User-Agent.
- **Temalar** (ayarlarda ayrı "Temalar" düğmesi): hazır temalar (Klasik, OLED siyah, Okyanus, Sıcak, Cam) veya panellerin, seçimin, metnin, bilgi panelinin, saatin kendi renkleri ve saydamlık.
- **Yönetim:** şifre ve ayar öğelerinin kilitlenmesi (kilitli öğeler gizlenir).

**User-Agent**, oynatıcının sağlayıcı sunucusuna kendini nasıl "tanıttığıdır". Liste yüklendi ama kanallar açılmıyorsa **VLC**'yi deneyin.

---

## 9. Yedekleme

**Ayarlar → Uygulama hakkında → Dışa aktar** listeleri, Favorileri, gizli grupları ve ayarları dosyaya kaydeder. **İçe aktar** bunları geri yükler — örneğin yeni bir cihazda.

---

## 10. Güncellemeler

- Uygulama güncellemeleri kendisi denetler, indirir ve kurar (**Uygulama hakkında**'dan kapatılabilir).
- Kurulumdan önce imza doğrulanır — güncelleme taklit edilemez.
- Uygulama **90 gün** boyunca güncelleme denetleyemezse kısıtlı mod açılır (yayın akışı ve arşiv yok, Favorilerde 5 kanal). İnternete bağlanmanız yeterli — her şey geri gelir.

---

## 11. Pro sürüm

Şu anda tüm özellikler **ücretsizdir**. Pro çıktığında herkes **3 ay** daha tam erişime sahip olacak.

| | Ücretsiz | Pro |
|---|---|---|
| Kalite | 1080p'ye kadar (4K/HDR — 3 dakika) | 4K, HDR |
| Favoriler | 20 kanal | sınırsız |
| Gizli gruplar | 1 | sınırsız |
| Arşiv | son 3 saat | sağlayıcının verdiği kadar |
| Ses dengeleme, otomatik kare hızı, 120 Hz, alıcıya AC3/DTS | — | ✓ |
| Kayıtlı canlı duraklatma, temalar | — | ✓ |
| Resim içinde resim ve arka planda ses (telefon) | — | ✓ |

---

## 12. Sorun giderme

- **Kanal açılmıyor** — User-Agent'ı değiştirin (VLC); listeyi başka bir cihazda deneyin.
- **Yayın akışı yok** — listedeki EPG adresini kontrol edin; **Oynatma listeleri**'ni açın — yükleme hatası orada görünür.
- **Telefonda ses dengelemeyle ses cızırdıyor** — dengelemeyi kapatın.
- **Zayıf TV kutusunda 4K takılıyor** — "Büyük" arabelleği seçin veya HD izleyin.

---

© 2026 Ruslan G. Tüm hakları saklıdır.
