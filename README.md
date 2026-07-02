# Oyun Sənayesi Analizi (Power BI & SQL Layihəsi)

Bu layihədə oyun sənayesindəki qlobal satış trendləri, platformaların bazar payı, janrların populyarlığı və oyun sənayesinin illər üzrə inkişaf dinamikası analiz edilmişdir. Layihə həm SQL verilənlər bazası sorğularını, həm də vizual hesabatlılığı əhatə edir.

## 🛠️ İstifadə Olunan Texnologiyalar
* **SQL:** Verilənlərin təmizlənməsi (Data Cleaning), aqreqasiya olunması və analiz sorğularının yazılması.
* **Power BI Desktop:** Məlumat modelləşdirilməsi, DAX ölçülərinin (Measures) yazılması və interaktiv idarəetmə panelinin (Dashboard) qurulması.

---

## 💾 SQL mərhələsində görülən işlər (Data Preparation)
Verilənlər bazası (Database) üzərində hesabatın təməli üçün aşağıdakı SQL əməliyyatları icra olunmuşdur:
1. **Məlumatların Təmizlənməsi:** Buraxılmış (null) dəyərlər, təkrarlanan sətirlər və yanlış formatda olan məlumatlar təmizləndi.
2. **Aqreqasiya Sorğuları:** Regionlar üzrə (Şimali Amerika, Avropa, Yaponiya və digər) ümumi satış məbləğlərini hesablamaq üçün `SUM()`, `GROUP BY` və `JOIN` əməliyyatlarından istifadə olundu.
3. **Performans Optimizasiyası:** Power BI-a yüklənən məlumat həcmini optimallaşdırmaq məqsədilə yalnız lazımi sütunlar SQL `VIEW`-ları vasitəsilə süzüldü.

---

## 📊 Power BI mərhələsində görülən işlər (Data Visualization)
Hesabat panelində vizuallıq və interaktivlik ön plana çıxarılmışdır:
* **Məlumat Modelinin Qurulması (Data Modeling):** Fakt və Dimensiya cədvəlləri arasında "Ulduz sxemi" (Star Schema) əlaqələri yaradıldı.
* **DAX Analitikası:** Ümumi Satış (Total Sales), Ümumi Oyun Sayı (Game Count) və Orta Satış (Avg Sales) kimi dinamik KPI göstəriciləri DAX metrikaları ilə hesablandı.
* **İnteraktiv Dashboard Dizaynı:** 
  * İstifadəçilərə Tarix, Platforma və Janr üzrə dinamik filtrləmə (Slicers) imkanı verildi.
  * Platformaların satış payı bar qrafiki ilə, janrların payı isə dairəvi qrafiklə vizuallaşdırıldı.
  * Zaman oxu üzrə oyun sənayesinin trendi xətti qrafiklə əks etdirildi.

---

## 📈 Əsas Sahələr (Görüntülər)

### Oyun Kəşf Paneli
![Vizual Səhifə 1](Ekran%20şəkli%202026-07-01%20113815.png)
![Vizual Səhifə 2](Ekran%20şəkli%202026-07-01%20113859.png)
![Vizual Səhifə 3](Ekran%20şəkli%202026-07-01%20113933.png)
