\# 🎓 Öğrenme Yönetim Sistemi (LMS) Seçimi İçin Bütünleşik AHP ve TOPSIS Karar Destek Modeli


[https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white]
\
\[https://img.shields.io/badge/Docker-Ready-2496ED?logo=docker&logoColor=white]
\[https://img.shields.io/badge/Yöntem-AHP%20%26%20TOPSIS-blue]
\[https://img.shields.io/badge/Alan-Endüstri%20Mühendisliği-brightgreen]
\[https://img.shields.io/badge/Lisans-MIT-orange]



> Bir yükseköğretim kurumunun uzaktan ve hibrit eğitim altyapısını optimize etmek amacıyla; \*\*SWOT, Pareto ve Balık Kılçığı\*\* kök neden analizleriyle tanımlanan kriterleri \*\*Analitik Hiyerarşi Prosesi (AHP)\*\* ve \*\*TOPSIS\*\* çok kriterli karar verme teknikleriyle modelleyen, Python ve Docker tabanlı karar destek sistemi.



\---



\## 📑 İçindekiler

1\. \[Proje Özeti ve Çözülen Problem](#-proje-özeti-ve-çözülen-problem)

2\. \[Temel Sorular ve Katma Değer](#-temel-sorular-ve-katma-değer)

3\. \[Karar Verme Metodolojisi](#-karar-verme-metodolojisi)

&#x20;  - \[Problem Teşhisi ve Kök Neden Analizi](#1-problem-teşhisi-ve-kök-neden-analizleri)

&#x20;  - \[AHP ile Kriter Ağırlıklandırma](#2-analitik-hiyerarşi-prosesi-ahp-ile-kriter-ağırlıklandırma)

&#x20;  - \[TOPSIS ile Alternatiflerin Sıralanması](#3-topsis-ile-alternatiflerin-sıralanması)

4\. \[Analiz Sonuçları ve Sıralama](#-analiz-sonuçları-ve-sıralama)

5\. \[3 Boyutlu Duyarlılık ve Kararlılık Analizi](#-3-boyutlu-duyarlılık-ve-kararlılık-analizi)

6\. \[Yönetsel Çıkarım: Matematiksel Model vs. Saha Gerçekliği](#-yönetsel-çıkarım-matematiksel-model-vs-saha-gerçekliği)

7\. \[Depo Yapısı ve Çalıştırma](#-depo-yapısı-ve-çalıştırma)



\---



\## 🎯 Proje Özeti ve Çözülen Problem

Yükseköğretim kurumlarında LMS seçimi yalnızca teknik bir yazılım satın alması değil; \*\*kullanıcı deneyimi, ders yönetimi, Öğrenci Bilgi Sistemi (OBS) entegrasyonu, veri güvenliği (KVKK) ve toplam sahip olma maliyetini\*\* eş zamanlı optimize etmeyi gerektiren çok boyutlu bir karar problemidir.



Bu çalışma; sezgisel ve sübjektif kararların önüne geçmek amacıyla, nitel ve nicel kriterleri bilimsel bir karar modeli içinde birleştirerek kurumun operasyonel ve stratejik hedeflerine en uygun LMS platformunu belirlemek üzere tasarlanmıştır.



\---



\## 💡 Temel Sorular ve Katma Değer



\* \*\*Ne İşe Yarıyor?\*\* Yükseköğretimde uzaktan eğitim altyapısı için en uygun LMS platformunu, sübjektif değerlendirmelerden arındırarak 6 temel kriter ve 6 alternatif üzerinden analitik olarak seçer.

\* \*\*Neleri Kapsıyor?\*\* SWOT, Pareto (%81,5 kuralı) ve Balık Kılçığı kök neden analizlerini; 5 uzmanın değerlendirmelerine dayalı AHP ağırlıklandırmasını ($CR < 0{,}10$); TOPSIS ideal çözüme yakınlık modelini; 6 senaryolu ve eşik tabanlı duyarlılık analizlerini kapsar.

\* \*\*Neleri İçeriyor?\*\* Tüm matematiksel adımları koşan Python analiz motoru (`lms\_mcdm\_analysis.py`), 4 adet analitik grafik, temiz CSV veri setleri, Docker altyapısı ve 4 sekmeli profesyonel bir Excel raporu içerir.

\* \*\*Neye Kolaylık Sağladı?\*\*

&#x20; 1. \*\*Entegrasyon ve Ders Yönetiminin Belirleyiciliği Kanıtlandı:\*\* Karar sürecinde maliyetin (%3,18) değil; Ders Yönetimi (%34,65) ve OBS Entegrasyonunun (%31,27) toplam ağırlığın üçte ikisini oluşturduğu matematiksel olarak kanıtlandı.

&#x20; 2. \*\*Yüksek Kararlılık Doğrulandı:\*\* VEDUBOX'ın baz senaryoda ($C\_i = 0{,}8346$) birinci çıkmasının yanı sıra, 6 farklı öncelik senaryosunun tamamında liderliğini koruduğu ispatlandı.

&#x20; 3. \*\*Yönetsel Riskler Hesaba Katıldı:\*\* Matematiksel olarak birinci çıkan alternatif ile mevcut altyapının sağladığı maliyet avantajı dengelenerek doğrudan geçiş yerine kontrollü bir pilot geçiş yol haritası önerildi.



\---



\## 🔬 Karar Verme Metodolojisi



```text

\[1. Problem Teşhisi]       \[2. AHP Ağırlıklandırma]         \[3. TOPSIS Sıralama]       \[4. Doğrulama]

SWOT + Pareto + Ishikawa ──> 5 Uzman Matrisi (Geom. Ort.) ──> Vektör Normalizasyonu ──> 6 Senaryo + Eşik

Öncelikli Sorun Tespiti      Tutarlılık Oranı (CR < 0.10)   İdeal Çözümlere Uzaklık    Duyarlılık Analizi

