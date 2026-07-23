# Timsah Türü Sınıflandırma

Bu proje, timsahlara ait fiziksel ve biyolojik özelliklerden yararlanarak bilimsel
tür etiketlerini tahmin eden çok sınıflı bir makine öğrenmesi çalışmasıdır.

[Notebook'u nbviewer ile aç](https://nbviewer.org/github/sametcsk/Predicting-Crocodile-Scientific-Names-with-ML/blob/main/crocodile-species-classification.ipynb)

## Yöntem

- Veri temizleme ve keşifsel veri analizi
- Kategorik ve sayısal özelliklerin hazırlanması
- Dokuz farklı sınıflandırma algoritmasının karşılaştırılması
- Test kümesi ve çapraz doğrulama sonuçlarının birlikte incelenmesi

## Sonuçlar

| Model | Test doğruluğu | Çapraz doğrulama doğruluğu |
| --- | ---: | ---: |
| Naive Bayes | %98,86 | %97,39 |
| Gradient Boosting | %98,30 | %97,16 |
| XGBoost | %96,02 | %96,82 |
| Random Forest | %94,32 | %94,32 |

Bazı türlerde örnek sayısı oldukça düşüktür. Bu nedenle yüksek genel doğruluk,
tüm türlerde aynı güvenilirliğin sağlandığı anlamına gelmez.

## Kullanılan Araçlar

`Python` • `Pandas` • `scikit-learn` • `XGBoost` • `LightGBM` • `Matplotlib`

## Çalıştırma

```bash
git clone https://github.com/sametcsk/Predicting-Crocodile-Scientific-Names-with-ML.git
cd Predicting-Crocodile-Scientific-Names-with-ML
jupyter notebook crocodile-species-classification.ipynb
```
