# 🛡️ Siber Güvenlik Araç Kutusu

Tarayıcıda çalışan, sunucu gerektirmeyen küçük bir siber güvenlik araç seti.

## Özellikler

- **Parola analizi:** Uzunluk, karakter çeşitliliği ve yaygın kalıplara göre güç tahmini ve kırılma süresi
- **Hash üretici:** SHA-256, SHA-512 ve SHA-1 (Web Crypto API)
- **Base64:** Kodlama ve çözme (UTF-8 destekli)

Girilen veriler hiçbir yere gönderilmez, tüm işlemler tarayıcıda yapılır.

## Kullanım

Dosyayı indirip `index.html` dosyasını tarayıcıda aç. Kurulum veya bağımlılık yok.

## GitHub Pages ile yayınlama

1. Repo ayarlarında **Settings → Pages** bölümüne git
2. Source olarak `main` branch ve `/ (root)` seç
3. Birkaç dakika sonra site `https://kullanici-adin.github.io/repo-adi/` adresinde yayında olur

## Neler öğrendim

- Parola gücü uzunluk ve rastgelelikle artar, "karmaşık görünmek" yetmez
- Hash tek yönlüdür, Base64 ise şifreleme değil sadece kodlamadır
- Parolalar saklanırken hızlı hash yerine bcrypt, scrypt veya Argon2 kullanılmalıdır

## Geliştirme fikirleri

- [ ] Parola üretici
- [ ] JWT çözücü
- [ ] Caesar / Vigenère şifreleme aracı
- [ ] Have I Been Pwned (k-anonymity) entegrasyonu

## Uyarı

Bu proje yalnızca eğitim ve savunma amaçlıdır.

## Lisans

MIT
