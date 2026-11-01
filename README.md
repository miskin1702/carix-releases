# CARIX — Windows x64 yayınları

Bu depo yalnız CARIX kurulum dosyaları ve imzalı güncelleme metaverileri içindir. Uygulama kaynak kodu içermez.

## İndirme

[GitHub Releases](https://github.com/miskin1702/carix-releases/releases) sayfasından üretim sürümünü seçin:

- `CarixServerSetup-vX.Y.Z.exe`: sunucu kurulumu.
- `CARIX_X.Y.Z_x64-setup.exe`: masaüstü istemci kurulumu.
- `SHA256SUMS.txt`: dosya bütünlüğü özetleri.

**0.6.x yayınları eski deneme paketleridir; üretim sürümü olarak kullanılmamalıdır.** Üretim sürümleme zinciri0.7.0 ile başlar. Yayımlanmış dosyalar değiştirilmez; düzeltme yeni sürümdür.

## Güncelleme

Üretim uygulaması **stable** kanalını kullanır. Kullanıcı uygulamanın Güncellemeler ekranından manuel denetler ve yüklemeyi açıkça başlatır; GitHub hesabı gerekmez. Sunucu ve masaüstü paketleri ayrı güncellenir.

İmzalı kanal dosyaları `channels/stable.json` ve `channels/desktop-stable.json` içindedir. Güncelleyici yerel güvenilen Ed25519 anahtarı, paket boyutu ve SHA-256 özetiyle doğrulama yapar. Bilinmeyen anahtar/imza veya değişmiş paket kabul edilmez.

Ed25519 güncelleme imzası Windows Authenticode sertifikası değildir. Windows bilinmeyen yayıncı/SmartScreen uyarısı gösterebilir; güvenlik kontrollerini kapatmayın. İndirmeyi bu depodaki sürüm ve checksum ile karşılaştırın.

## Depo politikası

Git geçmişinde yalnız kanal JSON'ları, checksum'lar, sürüm notları ve bu açıklama bulunur. Kurucular/tar paketleri GitHub Release asset'leridir; kaynak, özel anahtar, kimlik bilgisi, veritabanı ve işletme yedeği yayımlanmaz.
