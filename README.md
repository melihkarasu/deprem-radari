# Canlı Deprem Haritası & Sismik Radar (Standalone Edition)

**VibeCodedApps** ekosistemi kapsamında geliştirilen, sıfır-backend (zero-backend) ve tamamen istemci taraflı çalışan canlı deprem izleme uygulaması.

## Özellikler
- **Canlı USGS Sismik Akışı:** Türkiye & Çevresi, Marmara, Ege, Doğu Anadolu, Akdeniz ve Küresel görünümlerle büyüklük (`M 1.0+` – `M 6.0+`) ve zaman aralığı (`24 saat`, `7 gün`, `30 gün`) filtreleme.
- **OpenStreetMap (Leaflet) Harita:** Büyüklük ve derinliğe göre renk kodlu sismik işaretçiler ve doğrudan USGS rapor bağlantıları.
- **İsteğe Bağlı Konum Odaklama:** Yalnızca kullanıcı "Yakınımda" butonuna tıkladığında 250 km yarıçapı tarar; konum verisi sunucuya gönderilmez.
- **Gizlilik ve Güvenlik:**
  - Yerel fontlar (`vendor/fonts/*.woff2`) ile sıfır Google Fonts CDN / IP aktarımı.
  - Takip edilen bölge filtreleri yalnızca tarayıcı `localStorage` üzerinde (`VibeRuntime`) saklanır ve tek tıkla silinebilir.
  - Harici Leaflet varlıkları SHA-384 Subresource Integrity (SRI) ile korunur.

## Kullanım
Herhangi bir statik sunucuda veya doğrudan `index.html` dosyasıyla çalıştırılabilir:
```bash
npx serve .
```
