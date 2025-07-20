# Trafik Kazaları Analizi: İngiltere (2000–2016)

Bu proje, İngiltere'de 2000–2016 yılları arasında meydana gelen trafik kazalarını analiz etmek amacıyla hazırlanmıştır. Çalışma kapsamında 
kazaların zaman içindeki değişimi, mevsimsel etkiler, kırsal ve kentsel farklılıklar gibi faktörler incelenmiştir.

## Kullanılan Veri Setleri
- **Accidents**: `accidents_2005_to_2007.csv`, `accidents_2009_to_2011.csv`, `accidents_2012_to_2014.csv`
- **Traffic Flow**: `ukTrafficAADF.csv`
- Kaynak: [Kaggle – UK Traffic Accidents & Flow](https://www.kaggle.com/datasets/daveianhickey/2000-16-traffic-flow-england-scotland-wales)

## Analiz Soruları
1. Zaman içinde kaza oranlarını tahmin edebilir miyiz?
2. Mevsimsel değişkenlik var mı?
3. Kırsal ve kentsel alanlar nasıl farklılaşıyor?
4. Hangi çevresel ve zamansal faktörler kaza riskini artırıyor?

## Kullanılan Yöntemler
- Veri ön işleme ve temizleme (`pandas`)
- Zaman serisi analizi (line plot, linear regression)
- Gruplama ve özetleme (`groupby()`)
- Görselleştirme (`seaborn`, `matplotlib`)

## Öne Çıkan Bulgular
- **Yıllara göre** kaza sayılarında düşüş eğilimi gözlenmiştir (2000 → 160.000, 2016 → 118.000).
- **Yaz ve sonbahar aylarında** kaza sayısı artmaktadır (özellikle Temmuz ve Kasım).
- **Kentsel alanlar** daha fazla kazaya sahne olurken, **kırsal alanlar** daha ölümcül kazalara neden olmaktadır.
- **Tek yönlü çift şeritli yollar**, açık hava koşulları ve iş saatlerinde kazalar daha fazladır.

## Sonuç
Trafik kazalarının oluşumu yalnızca sürücü hatalarıyla değil, çevresel ve yapısal faktörlerle de yakından ilişkilidir. Bu analiz, karar vericilere daha etkili trafik yönetimi ve önleyici stratejiler geliştirme konusunda veri temelli bir bakış açısı sunmaktadır.

## 📂 Proje Yapısı

```
├── data/
│   ├── accidents_2005_to_2007.csv
│   ├── accidents_2009_to_2011.csv
│   ├── accidents_2012_to_2014.csv
│   └── ukTrafficAADF.csv
├── notebooks/
│   └── traffic_accidents_analysis.ipynb
├── visuals/
│   └── *.png
└── README.md
```

## Gereksinimler
- Python 3.8+
- pandas
- matplotlib
- seaborn
- scikit-learn (regresyon için)

## Gelecek Geliştirmeler
- Trafik yoğunluğu ile kazaların eşleştirilmesi
- Hava durumu verileri ile entegre analiz
- Machine Learning ile öngörü modeli

---
