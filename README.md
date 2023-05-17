# Tweet Emotion Recognition with Tensorflow
🙌Herkese merhaba. Notebook başlıkta ismi belirtilmiş olan Coursera'nın Guided Project'i takip edilerek oluşturulmuştur.Derivative of softmax function:) gibi merak ettiğim noktalar da dahil olmak üzere birçok noktayı proje sürecinde extra araştırmalarımla edindiğim için notebook içerisinde yine video, medium yazılarının yönlendirmeleri veya açıklamalar görebilirsiniz.

### Önemli Linkler
👀Kursu incelemek isterseniz https://www.coursera.org/learn/tweet-emotion-tensorflow adresini ziyaret edebilirsiniz.

📍Verisetini daha yakından incelemek için https://huggingface.co/datasets/dair-ai/emotion adresine göz atabilirsiniz.

### Neler Yaptım, Çıkarımım Ne?
✔Verisetimiz train, validation ve test olarak hali hazırda bölünmüş olup tweet içerikleri text, duygu değerleri ise label sütununda tutulmaktadır. 
0.88 accuracy_score ile [sadness,enjoy,fear,surprise,love,anger] 6 farklı duygunun sınıflandırılması Keras Sequantial modeli kullanılarak yapılmıştır.

🧐Aşağıda confusion_matrix çıktısından da görüleceği üzere gerçek değeri 'love' olmasına rağmen 'enjoy' olarak tahmin edilen 50 değer var. Bunun sebebi verisetindeki duygu dağılımı incelendiğinde anlaşılabilir.
Elimizde 'imbalance' bir veriseti var, model 'love' duygusunu yeterince öğrenememiş olabilir. Peki 'surprise' duygusunda neden durum böyle değil? Cevabını henüz ben de kestiremiyorum:)

![result_cm](https://github.com/msnunu/sentiment_analysis/assets/124269047/cc46daf8-f606-44e4-b269-da971b838e47)


### Notebook Bölümleri
Notebook dosyası 7 bölümden oluşmaktadır.
- 1.Introduction
- 2.Setup and Imports
- 3.Importing Data
- 4.Tokenizer
- 5.Padding and Truncating Sequences
- 6.Training The Model
- 7.Evaluating The Model
