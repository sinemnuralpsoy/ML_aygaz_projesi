# ML_aygaz_projesi
https://www.kaggle.com/code/sinemnuralpsoy/ml-aygaz-bootcamp
Bu proje, Disneyland parklarının ziyaretçi yorumlarından tatmin seviyelerini tahmin etmeyi amaçlamaktadır. Veri kümesi,  Disneyland'in Paris, California, ve Hong Kong şubelerine ait 42,000 ziyaretçi yorumunu içermektedir. Tahmin edilmek istenen temel özellik, ziyaretçi yorumlarındaki "Rating" (puan) değeridir.
Kullanılan Modeller ve Performans Sonuçları:

Linear Regression (Doğrusal Regresyon):

Test R-Kare Skoru: 0.39662
Mean Absolute Error (MAE): 0.63193
Mean Squared Error (MSE): 0.67364
Mean Absolute Percentage Error (MAPE): 0.21628
Yorum: Doğrusal regresyon modelinin R-Kare skoru, modelin tahminlerinin hedef değişkenle ne kadar uyumlu olduğunu gösterir. Skor 0.39662 olarak hesaplandı, bu da modelin tahminlerinin, gerçek puanların yaklaşık %40'ını açıkladığını belirtir. MAE ve MSE değerleri, modelin tahmin hatalarının ortalama büyüklüğünü yansıtır.

Logistic Regression (Lojistik Regresyon):

Test Accuracy: 0.61724
Test Precision: 0.57702
Test Recall: 0.61724
Test F1 Score: 0.58539
Yorum: Lojistik regresyon modeli, sınıflandırma görevinde kullanılan bir yöntemdir. Accuracy, modelin doğruluğunu ifade ederken, Precision ve Recall, sınıflandırma sonuçlarının kalitesini ölçer. F1 skoru, precision ve recall arasındaki dengeyi temsil eder. Modelin sonuçları, genel olarak orta seviyede bir performansı göstermektedir.

Decision Tree (Karar Ağaçları):

Test Accuracy: 0.48057
Test Precision: 0.47772
Test Recall: 0.48057
Test F1 Score: 0.47889
Cross-Validation Accuracy: 0.47776
Karar ağaçları modeli, sınıflandırma için kullanılan başka bir yöntemdir. Modelin performansı, doğruluk, precision, recall ve F1 skoru açısından düşüktür. Cross-validation sonuçları da benzer şekilde düşük bir doğruluk göstermektedir, bu da modelin genelleme kapasitesinin sınırlı olduğunu gösterir.

K-Nearest Neighbors (KNN):

Test Accuracy: 0.53904
Test Precision: 0.45124
Test Recall: 0.53904
Test F1 Score: 0.46681
Cross-Validation Accuracy: 0.53411
KNN modelinin sonuçları, diğer sınıflandırma modellerine kıyasla orta seviyede performans göstermektedir. Precision ve recall değerleri modelin doğruluğunu ve kapsayıcılığını temsil eder. Cross-validation sonuçları, modelin genel olarak tutarlı bir performans sergilediğini göstermektedir.

Ridge Regression (Ridge Regresyonu):

En İyi Alpha: 100.0
En İyi Skor: 0.67765
Eğitim Verisinde MSE: 0.61198
Cross-Validation MSE: 0.67823
Test Verisinde MSE: 0.68974
Test Verisinde RMSE: 0.83051
Yorum: Ridge regresyonu, hiperparametre optimizasyonu ile en iyi performansını elde etmiştir. MSE ve RMSE değerleri, modelin tahmin hata büyüklüğünü belirtir. En iyi alpha değeri 100.0 olarak belirlenmiştir.

Gözetimsiz Öğrenme Algoritmaları:

k-Means:
Silhouette Score: 0.50238
Silhouette Score (n=2): 0.45940
 K-means algoritması, kümeleme performansını ölçmek için kullanılan Silhouette skorunu göstermektedir. Skor 0.50238 olarak hesaplandı, bu da kümelerin birbirinden ne kadar iyi ayrıldığını ve iç içe geçmediğini ifade eder. n=2 için hesaplanan skor ise biraz daha düşük olup, kümelerin iç içe geçme oranının arttığını gösterir.

Apriori:
Frequent Itemsets: (Item1, Item2, Item3)
Association Rules: Boş
 Apriori algoritması, sık kullanılan itemsetleri bulmada başarılı olmuş ancak association rules oluşturulmamıştır. Bu, verinin belirlenen eşiklerin uygun olmadığını gösterebilir.
 Farklı model ve algoritmaların performansı çeşitli sonuçlar vermiştir. Linear Regression ve Ridge Regression, tahminler açısından daha başarılı olurken, sınıflandırma algoritmaları (Logistic Regression, Decision Tree, KNN) orta seviyede performans sergilemiştir. K-means kümeleme iyi bir silhouette skoru göstermiştir, ancak hiperparametre ayarları model performansını etkileyebilir. Apriori algoritması ise beklenen association rules'ları oluşturamamıştır. Bu sonuçlar, model ve algoritmaların performansını optimize etmek için daha fazla inceleme ve ayar gerektirdiğini göstermektedir.
