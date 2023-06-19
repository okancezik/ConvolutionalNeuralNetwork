<h3>EVRİŞİMLİ SİNİR AĞLARI – CNN</h3>
<p>
  Evrişimli sinir ağları, yapay zekanın alt kolu olan derin öğrenme alanında yaygın olarak kullanılan bir yapay sinir ağı türüdür. 
  Derin öğrenme, yapay sinir ağlarından ve biyolojik sinir ağlarından ilham alan makine öğreniminin bir alt alanıdır. 
  Evrişimli sinir ağları da aynı oradaki gibi biyolojik sinir hücrelerinin çalışmasından esinlenerek geliştirilmiştir. 
  Yapay sinir ağlarına kıyasla evrişimli sinir ağları daha derin bir ağ yapısına sahiptir. Derin öğrenme dediğimiz kapsamda aynı bunu temsil eder. 
</p>
<p>
  Günümüzde birçok uygulamada CNN algoritması önemli yer alır. Görsel tanıma, görüntü sınıflandırma, nesne tespiti ve daha birçok uygulamada CNN algoritması başarılıdır. Özellikle görsel işlemede oldukça yaygın kullanılır.   
</p>
<p>
  Evrişimli sinir ağları algoritması derin bir yapıya sahiptir. Ağın içerisinde gerekirse çok sayıda katman olabilir. Bu katmanlar
  <ul>
    <li>Girdi katmanı</li>
    <li>Evrişimli katman (Convolutional layer)</li>
    <li>Aktivasyon katmanı (Activation layer)</li>
    <li>Havuzlama katmanı – Ortaklama (Pooling) katmanı</li>
    <li>Bağlı katman (Fully Connected layer) </li>
  </ul> 
</p>  
<p>
  Her katman birbiriyle etkileşim halindedir. Bu etkileşim her katmanda bulunan sinir hücrelerinin birbirleriyle ağırlıklı bağlantılara sahip olmasıyla gerçekleşir. 
</p>
<ul>
  <li>
    <h4>Girdi katmanı – Input layer</h4>
    <p>
      Girdi katmanı, ağımızın ilk katmanıdır. Ağa veriler bu katmandan verilmeye başlanır. Bu katmandan alınan veri sinir hücreleri aracılığıyla diğer katmana geçer. Buradaki önemli husus bu katmandaki nöron sayısı girdi bilgisindeki özellik sayısıdır. 
    </p>
  </li>
  <li>
    <h4>Evrişimli katman – Convolutional layer</h4>
    <p>
        Girdi katmanından gelen verinin üzerindeki özellikleri çıkarmak için kullanılan katmandır. Evrişim katmanında bu işlemi yapmak için filtreler-çekirdekler kullanılır. Filtreler veya çekirdekler genellikle 2x2,3x3,5x5,7x7.. şeklinde girdi verisinden daha küçük matrislerdir. Her filtre, girdi verisi üzerinde küçük bir pencereyi hareket ettirir ve giriş verisini bu pencere üzerinden geçirir. Yani filtre girdi üzerinde kaya kaya işlem gerçekleştirir. Bu işlem sonrasında ve bu katmanın çıktısı olarak özellik haritası elde edilir. 
    </p>
 </li>
   <li>
    <h4>Aktivasyon katmanı – Activation layer</h4>
    <p>
        Aktivasyon katmanında aktivasyon fonksiyonları kullanılır. Bir önceki katmandan gelen veri aktivasyon fonksiyonuna girer. Aktivasyon fonksiyonları ağa nonlineer özelliği kazandırır. Aynı zamanda aktivasyon katmanı ağın öğrenme kapasitesini arttırmayı amaçlar.
    </p>
 </li>
   <li>
    <h4>Havuzlama katmanı – Ortaklama (Pooling) katmanı</h4>
    <p>
      Bu katmanda boyut azaltma işlemleri gerçekleşir. Boyut azaltma ile hedeflenen şey hesaplandırmaları hızlandırmak ve aşırı öğrenmeyi engellemektir. Bu katmanda maksimum havuzlama yöntemi yaygın kullanılan bir yöntemdir. Bu yöntemde, her bir özellik haritası üzerinde bir kayan pencere geçirilir ve her bölgenin maksimum değeri alınarak yeni bir havuzlama haritası oluşturulur. Bu, özelliklerin konumundan bağımsız olarak en önemli özelliklerin korunmasına yardımcı olurken, hesaplama yükünü azaltır.
    </p>
 </li>
    <li>
    <h4>Bağlı katman – Fully connected layer</h4>
    <p>
        Bağlı katman CNN algoritmasının son katmanıdır. Havuzlama katmanından sonra gelen bağlı katmanda önceki katmanlardan alınan özellikler tam bağlantılarla birbirine bağlanır. Bağlı katmanda her bir özellik vektörü ilgili ağırlıklar ile çarpılır ardından aktivasyon fonksiyonu ile çıktı üretilir. Bu çıktılar sınıf veya kategoriye karşılık gelebilecek bir olasılık değeri olarak düşünebiliriz. Eğer sınıflandırma yapıyorsak ağın sın bağlı katmanında sınıf etiketi sayısı kadar sinir hücresi bulunur.
    </p>
 </li>
</ul>  
