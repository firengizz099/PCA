# PCA

![App Screenshot](https://github.com/firengizz099/PCA/blob/main/pca.png?raw=true)

Bu Python kodu, bir veri kümesini kullanarak temel bileşen analizi (PCA) ile boyutsal azaltma uygulamak ve sonrasında PCA uygulanmış ve uygulanmamış veri kümeleri üzerinde lojistik regresyon sınıflandırma modelini eğitmek ve sonuçları karşılaştırmak. 
**Kodun ayrıntılı açıklaması:**

    1. Gerekli kütüphanelerin içe aktarılması:
        ◦ numpy, sayısal işlemler için.
        ◦ matplotlib, veri görselleştirme için.
        ◦ pandas, veri işleme için.
    2. Veri kümesinin 'Wine.csv' dosyasından yüklenmesi. Bu veri kümesi, şarapların kimyasal özelliklerini içerir.
    3. Bağımlı değişken (y) ve bağımsız değişkenlerin (X) ayırılması:
        ◦ X, veri kümesinin ilk 13 sütununu içerir.
        ◦ y, son sütunu (şarap sınıfı) içerir.
    4. Eğitim ve test verilerinin ayrılması:
        ◦ train_test_split fonksiyonu kullanılarak veriler %80 eğitim ve %20 test olarak ayrılır.
    5. Verilerin ölçeklendirilmesi:
        ◦ StandardScaler kullanılarak verilere ölçekleme uygulanır.
    6. Temel Bileşen Analizi (PCA) için PCA sınıfının kullanılması:
        ◦ n_components parametresi ile 2 bileşen kullanmayı belirtiyoruz.
    7. PCA dönüşümünün eğitim ve test verilerine uygulanması, verilerin daha düşük boyutlu bir uzaya dönüştürülmesi.
    8. PCA uygulanmamış veriler üzerinde lojistik regresyon sınıflandırma modelinin (classifier) oluşturulması ve eğitilmesi.
    9. PCA uygulanmış veriler üzerinde başka bir lojistik regresyon sınıflandırma modelinin (classifier2) oluşturulması ve eğitilmesi.
    10. Her iki model kullanılarak tahminlerin yapılması ve sonuçların y_pred ve y_pred2 içinde saklanması.
    11. Her iki tahmin için ayrı ayrı karmaşıklık matrislerinin (confusion_matrix) hesaplanması ve ekrana yazdırılması.
    12. PCA uygulanmış ve uygulanmamış veriler üzerindeki tahminlerin karşılaştırılması için bir karmaşıklık matrisinin (cm3) daha hesaplanması ve ekrana yazdırılması. Bu, PCA'nın veri boyutunu azaltmanın sınıflandırma performansına nasıl etki ettiğini gösterir.

Bu kod, veri boyutunu azaltmak için PCA'nın nasıl kullanılacağını ve PCA'nın sınıflandırma performansını nasıl etkileyebileceğini göstermek için kullanılıyor. Ayrıca, PCA uygulanmış ve uygulanmamış veriler arasındaki farkı incelemek için karmaşıklık matrisleri kullanıyor.
