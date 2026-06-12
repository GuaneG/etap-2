# Etap 2 — Linux & Bash: Otomatik CSV Arşivleyici

> Yol haritamın 2. etabı (Etap 1 ile paralel gidebilir). Linux komutları, bash scripting ve cron öğrenmek için yaptığım pekiştirme projesi.

Bir klasördeki CSV dosyalarını tarihe göre sıkıştırıp arşivleyen, her çalıştığında log tutan ve cron ile her gece otomatik çalışan bir bash scripti.

## Kullanılan araçlar
- **Bash**
- `tar` / `gzip` — sıkıştırma
- `date` — tarihli dosya adı
- `cron` — zamanlama

## Kaynaklar
- [MIT The Missing Semester](https://missing.csail.mit.edu/) (Ders 1, 2, 4)
- [OverTheWire Bandit](https://overthewire.org/wargames/bandit/) (hedef: Level 20)
- [crontab.guru](https://crontab.guru)

## Kurulum & çalıştırma
```bash
chmod +x arsivle.sh
./arsivle.sh /hedef/klasor

# Her gece 02:00'de otomatik çalıştırmak için (crontab -e):
0 2 * * * /tam/yol/arsivle.sh /hedef/klasor
```

## Notlar
<!-- TODO: grep/awk, pipe, exit kodu, cron syntax hakkında notlar -->

## ✅ Etap 2 Bitiş Kontrol Listesi
- [ ] grep/awk ile bir log dosyasından istediğim satır ve kolonu çekebiliyorum
- [ ] Pipe ile komutları zincirleyebiliyorum
- [ ] Argüman alan, hata kontrolü yapan bir bash scripti yazabiliyorum
- [ ] chmod ile dosya izinlerini ayarlayabiliyorum
- [ ] crontab syntax'ını okuyup yazabiliyorum
- [ ] Bandit'te Level 20'ye geldim
