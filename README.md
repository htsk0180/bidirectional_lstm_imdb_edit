# bidirectional_lstm_imdb_edit

Merhabalar, Bu repo da IMDB data seti üzerinde yorumları sınıflandıracak basit bir ağ kurduk. Ve model paremetrelerini optimize ettik.
Ancak bu repo üzerinde bazı oynamalar yapacağız. 
2 farklı güncelleme yaparak sonuçları inceleyeceğimiz bir lab. ortamı kuracağız.
Softmax ve optimizasyon algoritmalarını şuana kadar kullanılmamış şekilde farklı fonksiyon ve algoritma ile değiştereceğiz.
Bu algoritmayı ve fonksiyonu biz yazacağız. Bakalım optimize edilmiş model mi yoksa bizim yazdığımız model mi dataset üzerinde daha iyi sonuç verecek ?

---

bidirectional_lstm_imdb_lion_opt. ipynb notebook'unda lion optimizer adı altında 2 ay önce makalesi yayımlanan optimizer'i mimarimize
dahil ettik.
Sonuçlar etkileyici. Adam optimizer'e göre daha hızlı ve daha yüksek doğruluk verdi. 

ADAM:

Epoch 1/2
782/782 [==============================] - 111s 126ms/step - loss: 0.3809 - accuracy: 0.8272 - val_loss: 0.3284 - val_accuracy: 0.8629
Epoch 2/2
782/782 [==============================] - 44s 57ms/step - loss: 0.1963 - accuracy: 0.9267 - val_loss: 0.3373 - val_accuracy: 0.8545

LION:

Epoch 1/2
782/782 [==============================] - 68s 79ms/step - loss: 0.4302 - accuracy: 0.7966 - val_loss: 0.3189 - val_accuracy: 0.8646
Epoch 2/2
782/782 [==============================] - 36s 46ms/step - loss: 0.1833 - accuracy: 0.9332 - val_loss: 0.3996 - val_accuracy: 0.8545



