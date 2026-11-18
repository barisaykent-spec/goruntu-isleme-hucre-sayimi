# Klasik Görüntü İşleme ile Mikroskobik Hücre Sayımı

Görüntü İşleme dersi yüksek lisans ara sınav projesi. Cell Tracking Challenge **Fluo-N2DH-GOWT1** veri setinde yalnızca klasik görüntü işleme yöntemleriyle (derin öğrenme yok) hücre segmentasyonu, sayımı ve zamansal sayım analizi.

## Veri seti
- Sayfa: https://celltrackingchallenge.net/2d-datasets/
- Eğitim arşivi: https://data.celltrackingchallenge.net/training-datasets/Fluo-N2DH-GOWT1.zip
- Notebook arşivi `data/` klasörüne otomatik indirir. Veri seti ve veri görüntüsü içeren şekiller bu repoya **yüklenmez**.

## Tekrarlanabilirlik
- Random seed: **31084** (öğrenci no son 5 hane 29058 + 2026)

## Çalıştırma
**Google Colab:** `main.ipynb`'yi Colab'da açın → *Runtime → Run all*.
**Yerel Jupyter:**
```bash
pip install -r requirements.txt
jupyter notebook main.ipynb
```

## Proje durumu
| Bölüm | Durum |
|---|---|
| 0–1. Kurulum ve veri inceleme | ✅ |
| 2. Veri seçimi (`selected_frames.csv`) | ✅ |
| 3. Referans sayımlar (geliştirme + doğrulama) | ✅ |
| 4. Baseline (dondu: Otsu + bağlı bileşen + min alan 30 px) | ✅ |
| 5–8. Deneyler (`experiments.csv`) | ⏳ |
| 9. Doğrulama (`validation_results.csv`) | ⏳ |
| 10. Kilit (`final_pipeline.json`, `test_predictions_locked.csv`) | ⏳ |
| 11. Test ve zamansal analiz (`test_results.csv`) | ⏳ |
