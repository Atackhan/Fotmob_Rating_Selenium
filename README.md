

````markdown
# Premier League Oyuncu Rating Verisi Toplama

Bu proje, 2023–2024 Premier League sezonuna ait maçlardan oyuncuların performans (rating) verilerini otomatik olarak çekmek için geliştirilmiştir. Veriler, analiz ve modelleme süreçlerinde kullanılmak üzere Excel dosyasına kaydedilir.

## Hedef

Futbol analiz projemizde eksik olan oyuncu rating verilerini tamamlamak amacıyla, FotMob platformundan veri toplama işlemi gerçekleştirilmiştir.

## Özellikler

- Selenium ile FotMob sayfaları üzerinde otomatik gezinme
- Her maç için:
  - Ev sahibi ve deplasman takımı isimleri
  - Maç tarihi
  - Oyuncu isimleri
  - Oyuncu performans puanı (rating)
- Verilerin `fotmob_data.xlsx` adlı Excel dosyasına yazılması
- Kesintilere karşı güvenli veri kaydı (script durdurulsa bile veri kaybı yaşanmaz)

## Kullanılan Teknolojiler

- Python 3.x
- Selenium
- openpyxl
- ChromeDriver

## Kurulum

1. Gerekli Python paketlerini yükleyin:

```bash
pip install selenium openpyxl
``


## Kullanım

1. `fotmob_scraper.py` dosyasını çalıştırın:

```bash
python fotmob_scraper.py
```

2. Script çalıştıktan sonra veriler `fotmob_data.xlsx` dosyasına kaydedilir.

## Örnek Çıktı (Excel)

| Maç Tarihi | Ev Sahibi       | Deplasman        | Oyuncu Adı      | Oyuncu Rating |
| ---------- | --------------- | ---------------- | --------------- | ------------- |
| 20.08.2023 | Manchester City | Newcastle United | Kevin De Bruyne | 8.3           |
| 20.08.2023 | Manchester City | Newcastle United | Erling Haaland  | 7.9           |
| ...        | ...             | ...              | ...             | ...           |

## Notlar

* FotMob dinamik içerik yüklediği için bazı bekleme süreleri (`time.sleep`) kullanılmıştır.
* Web scraping işlemlerinde ilgili sitelerin kullanım koşullarına dikkat edilmelidir.
* Proje yalnızca eğitim ve kişisel analiz amaçlıdır.

## Lisans

Bu proje açık kaynaklıdır ve MIT lisansı ile lisanslanmıştır. Ayrıntılar için `LICENSE` dosyasına bakabilirsiniz.

```

---

##  Bu README ile Ne Elde Edersin?

- Kodun amacını net anlatır
- Teknik detayları açıklar (kullanım, çıktı, kurulum)
- GitHub'da düzgün görünen bir format sağlar
- Projenin profesyonel durmasını sağlar

---
