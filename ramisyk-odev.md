# Github Lisansları 
Yazılımların kullanımı, dağıtımı gibi hakların sınır ve koşullarının detaylarını barındıran belgeler yazılım lisanslarıdır. 
## 1. MIT Lisansı
Özellikle açık kaynak dünyasında en çok kullanılan lisanslardan biridir. MIT Lisansı bir çok alanda geliştiricileri ve kullanıcıları özgür kılar. Yazılıma ait kaynak kodu veya derlenmiş yazılımı istenilen şekilde değiştirilmesinde, yayılmasında ve kullanılmasında hatta ticari bir şekilde kullanıma sunulmasında hiçbir sakınca bulunmamaktadır. Geliştirici tarafında ise, proje veya kod kapsamında herhangi bir sorun çıkması durumunda yükümlülükleri ortadan kaldırır. Yasal yükümlülüklerin yanı sıra MIT Lisanslı bir projenin kullanılması durumunda kaynak için referans belirtilmesi yani telif bulundurulması gerekmektedir. MIT Lisanslı projelerin kullanıldığı yeni projeler de lisanslanmalıdır. 

## 2. Apache Lisansı
MIT Lisansı ile aynı imkan ve özgürlükleri sunan Apache Lisansı farklı olarak, Apache ile lisanslanmış projelerin dağıtımında ürün lisanslarının da eklenmesi gerekmektedir. Bunların dışında Apache Lisanslı projeler üzerinde yapılan değişiklikler belirtilmeli ve bildirilmelidir.  
## 3. GNU Genel Kamu Lisansı
Açık kaynak kodlu projelerin kodlarına erişmede diğer lisanslardaki özgürlüklere sahip olan bu lisans, ürünlerin kullanımı için belirli kısıtlamalar bulunmaktadır. Öncelikle GNU lisansına sahip bir ürün kullanılıyorsa ve ürün dağıtılacaksa, bu ürünü kullanan yazılımın da GNU lisansına sahip olması gerekmektedir. Bu gereksinim yazılımın geri kalan kodlarının da açık kaynaklı olmasına neden oluyor aksi taktirde ticari satışlarda sorunlar yaratabiliyor.
## 4. Creative Commons
Fazla kullanılmayan, arka planda kalan lisans türleridir. Paylaşım ve değişim bakımından özgürlükler sunar ancak uygun referans vermek, lisansa bağlantı sağlamak ve değişiklik yapıldıysa bilgi vermek gerekmektedir [[1](https://medium.com/@mehmet.baran/yaz%C4%B1l%C4%B1m-lisans-tipleri-mit-apache-gnu-1397af4d1fbb) - [2](https://www.yusufaytas.com/acik-kaynak-lisanslari/)].

# Merge - Squash - Rebase Arasındaki Farklar
**Merge** işlemi uygulandığında, yeni bir *Merge commit* yaratıp iki branchin de yapılmış tüm değişikliklerini içerecektir. Master, diğer branch üzerinde yapılan tüm değişiklikleri alacak ve entegre edecektir ancak branch geçmişinde hiçbir değişiklik olmayacaktır.

**Squash** geçmişte atılan commit'leri yeniden düzenlemek, isimlendirmek veya birleştirmek için kullanıyoruz

Master üzerine yeni bir branch **rebase** edildiğinde, branch deki commitler tek tek alıp master ın sonuna ekleyecektir. Rebase sonucunda tek bir geçmiş oluşturulur çünkü tamamlanan işi bir branch ten diğerine aktarır. Bu süreçte istenmeyen geçmiş ortadan kalkar.

![https://miro.medium.com/max/875/1*g8ct_Pqa9Raakac0n-4v1A.png](https://miro.medium.com/max/875/1*g8ct_Pqa9Raakac0n-4v1A.png)

*Merge* tüm değişiklikleri sakladığı için, işlem sonunda tüm değişiklikler görüntülenmek isteniyorsa **merge kullanılmalıdır**.

Daha sade, anlaşılabilir ve lineer bir commit history görüntülenmek isteniyorsa **rebase** daha doğru bir kullanım olur [[3](https://medium.com/@halilibrahim_4325/git-merge-ve-rebasein-fark%C4%B1-nedir-1c6c81086fa9) - [4](https://qastack.info.tr/programming/2427238/in-git-what-is-the-difference-between-merge-squash-and-rebase)]. 
# Agile, Scrum ve Kanban
### Agile Nedir?
Değişime hızlı ve verimli bir şekilde uyum sağlamayı hedef alan bir proje yönetim metodolojisidir. Agile değişim sonucu olabilecek riskleri minimum zararla atlatmanın yanı sıra değişimin oluşturabileceği fırsatlardan da yararlanarak verimli bir çalışma planı oluşturur.

Agile metodolojisinde, talepler küçük parçalara ayrılarak planlamalar uzun süreçler için değil üzerinde hazırlanmak yerine bu parçalar üzerinde çalışılacak şekilde hazırlanıyor. Talep sahibinin parça çıktıları üzerinde sık sık görüşleri alınarak oluşabilecek yanlışlıkların önüne geçilebiliyor [[5](https://www.atlassian.com/agile)]. 
### Scrum Nedir?
Bir projede gelinen durumu düzenli olarak kontrol ederek, ortaya çıkan sorunları hızlı bir şekilde fark edip duruma göre proje ve ekibi uyarlama sistemi ile çalışmayı hedefler. Bu çalışma şekli, ile zaman, insan gücü ve gereken masraflar bakımından daha az maliyet ile daha kaliteli bir ürün ortaya koymayı amaçlar. 

Ürün sahibi, proje ekibi, scrum master kişilerinin etkilenişimi ile scrum süreci oluşur.

![https://www.orangescrum.com/blog/wp-content/uploads/2018/10/Agile-Project-Management-with-Scrum-Boards-Backlog-Sprints-in-OrangeScrum.png](https://www.orangescrum.com/blog/wp-content/uploads/2018/10/Agile-Project-Management-with-Scrum-Boards-Backlog-Sprints-in-OrangeScrum.png)

Ürün sahibi, istediği ürün için yapılması gereken her şeyi içeren bir iş listesi oluşturur ve bu listedeki işleri önem durumlarına uygun olarak ölçeklendirir. Ürün sahibinin proje ekibi ile sürekli iletişim halinde olduğundan istek veya gereksinim değişiklikleri söz konusu olduğunda hızlıca geri dönüş alınabildiğinden iş listesi sürekli olarak güncellenebilmektedir. 

Proje ekibi hızlı ilerlemesi gereken çalışmalar sergileyeceği için çok sayıda insan içermemelidir. 3 kişi ile 9 kişi arasında bir proje ekibi kurulması sürecin olumlu ilerleyebilmesi için daha uygun olduğu düşünülmüştür.  
#### Sprintler İle Ürünü Hazırlama
Ürün sahibi, proje ekibi ve scrum master'ın bir arada bulunduğu, belirlenen iş listesinin parçalara bölündüğü ilk toplantı **Sprint Planlama Toplantısı** olarak adlandırılır. Bu toplantıda bir aydan daha kısa bir süre sonra gerçekleşmesi gereken bir sonraki sprint toplantısına kadar yapılacak işler belirlenir.

Genellikle bir ya da iki hafta olarak belirlenen süreçlere **sprint** denir ve sprintler süresince herkes yapması gereken işleri yapmaya başlar. Her sprint sonunda (bir sonraki sprint toplantısında) yapılan işler değerlendirilir ve yeni yapılacak işler planlanarak süreç takibi yapılır.

Sprint süresince günlük olarak proje ekibi ve scrum master'ın bulunduğu 15 dakikayı geçmeyecek toplantılar düzenlenir. Toplantıların kısa olması hedeflendiği için genellikle ayakta gerçekleştirilir ve bu nedenle bu toplantılar**Günlük Stand-Up Toplantı (Daily Sand-Up Meeting)** olarak adlandırılır. Her gün yapılan bu toplantıların amacı ekibin birbirlerinden haberdar olması ve olası sorunlara hızlı çözümler bulunmasıdır.

Günlük Scrum toplantısının konuları şu sorular etrafında şekillenir:
- Dün ne yaptın?
- Bugün ne yapacaksın
- İşi yapmaya engel bir durum var mı?

Her sprit bitiminde yapılanları gözden geçirmek ve tamamlanan maddelerin değerlendirilmesi için herkese açık bir **Sprint Gözden Geçirme Toplantısı** yapılır. Bu toplantıdan sonra scrum ekibi ile sprint sürecinde yolunda giden ve gitmeyen işlerin değerlendirilmesi ve gelecek sprint'in daha verimli gerçekleşmesi için nelerin yapılacağının konuşulduğu bir **Sprint Geçmişini Değerlendirme Toplantısı** düzenlenir.

Üzerinden geçtiğimiz bu işlemler, süreçler ve toplantılar döngüler halinde iş listesindeki işler bitene kadar bütün sprintler için gerçekleşir ve ürünün ortaya çıkması ile scrum süreci sonlanır [[6](https://www.scrum.org/resources/what-is-scrum)].
### Kanban Nedir?
 İş yönetim ve organize yöntemidir. Yapılacak işlerin görselleştirilmesi ve bölünerek uygulama aşamasına geçilmesi amaç olarak belirlenmiştir. İnsanların yapacağı şeyleri bir alanda toplu görmesi onları ne yapacağı veya nereden başlayacağı karmaşasından kurtarmasına yardımcı olacağından bu teknik bir çok alanda süreç yönetimi için kullanılmaktadır.

Kanban için fiziksel ya da dijital bir tahta (tablo) hazırlanarak sütunlara bölünür. İşin gelişimine uygun olarak sütun sayıları ve isimleri farklılık gösterebilir. Sürecin yönetilebilir olması için her sütuna gelecek olan görev sayısı sınırlandırılmalıdır, yeni bir görev almak için bir tanesinin tamamlanması beklenmelidir.

![https://miro.medium.com/max/800/1*eG6NWCGRIuHheQIczqSYmA.png](https://miro.medium.com/max/800/1*eG6NWCGRIuHheQIczqSYmA.png)

Temelde kanban tahtası **Yapılacaklar, Yapılıyor Olanlar ve Yapılanlar (tamamlananlar)** sütunlarından oluşmaktadır. **Yapılacaklar** sütunu iş başlangıcında hazırlanır ve işi parçalara bölerek organize olmayı sağlarken sürekli ne yapacağını görmek işten zihinsel olarak uzaklaşmayı engeller. Yapılacak olanlar sütunundan daha önceden belirli sayıda iş **Yapılıyor Olanlar** sütununa kaydırılır ve işlemler gerçekleştirilmeye başlanır. Aynı anda birden çok işin yapılmaya çalışılması verimliliği düşüreceğinden bu alanın sınırlandırılması oldukça önemlidir. Son olarak da yapılıyor olan işlemlerden tamamlananlar **Yapılanlar** sütununa kaydırılarak işlem bitirilir. Bu alan için de insanın tamamladığı yani başarıya ulaştığı işlemleri de göz önünde bulundurmasının çalışma motivasyonunu arttırması nedeniyle verimlilik için önemli olduğunu söyleyebiliriz [[7](https://listelist.com/kanban-nedir/) - [8](https://kanbanize.com/kanban-resources/getting-started/what-is-kanban)].

# Github Flow'un Alternatifleri
## Git Flow
*master* ve *develop* olmak üzere iki ana branch'ten oluşur. *master* ürün kodlarını içerirken *develop* üründen önceki kodları içerir ve bütün kodlar *master* üzerinde merge olur.
### Avantajları:
- Projenin başlangıcından sonuna kadar olan süreçte branch'lerin sade bir şekilde kalmasını sağlar.
- İsimlendirme sistematik bir model olduğundan anlaşılırlığı arttırır.
- Git araç ve uzantılarına destek verir.
- Ürün için birden fazla versiyon olduğunda kullanımı kolaylaştırır.
### Dezavantajları:
- Git geçmişi okunamaz şekildedir.
- Tek versiyonlu ürünlerde desteklenmemektedir.
## GitLab Flow
### Avantajları:
- Sürekli Entegrasyon ve Teslimatın nasıl yapılacağını belirtir.
- Git geçmişi temiz tutulur, okunurluluğu arttırır.
- Üretimde tek versiyona ihtiyaç duyulduğunda idealdir
### Dezavantajları:
- GitHub Flow'a göre daha karmaşık bir yapıya sahiptir.
- Birden çok sürüme sahip uygulamalarda karmaşık bir hale gelir.
## One Flow
*develop* branch'i bulunmamaktadır. Her yeni release bir önceki release üzerine kurularak yapılır.
### Avantajları:
- Git geçmişi temiz tutulur, okunurluluğu arttırır.
- Takım kararlarına  uygun olacak şekilde esneklik gösterir.
- Üretimde tek versiyona ihtiyaç duyulduğunda idealdir
### Dezavantajları:
- Sürekli Entegrasyon ve Teslimat içeren projeler için kullanılması önerilmez.
- Özellik branch'leri Sürekli Entegrasyon işlemini zor hale getirir [[9](https://medium.com/@patrickporto/4-branching-workflows-for-git-30d0aaee7bf)].
# Gang of Four(GOF)
Nesne yönelimli programlamada, programlama dili fark etmeden, nesne olarak adlandırılan yapılar arasındaki ilişkilerin nasıl olması gerektiğini belirten kalıplar yazılım için tasarım kalıplarıdır. Gang of Four Erich Gamma, Richard Helm, Ralph Johnson and John Vlissides isimlerindeki 4 yazardır ve **Design Patterns — Elements of Reusable Object-Oriented Software** adlı kitabı yayınlamışlardır [[10](https://deryacakmak.medium.com/tasar%C4%B1m-kal%C4%B1plar%C4%B1-nelerdir-cd216ba47921)].
# Interface ve Abstract Sınıflar Arasındaki Farklar
## Interface Nedir?
Değişime uygun sürdürülebilir yazılım geliştirmenin temel elemanlarındandır ve ortak özellikler içerek sınıflar için bir temel sınıf oluşturmak için kullanılır. Temel sınıfta hangi metotların olacağı belirtilir ancak işlemlerin nasıl yapılacağının belirtilmesi gerekmemektedir. İç detayların bu interface ile üretilen sınıfların içerisinde yazılması gerekmektedir. 
## Abstract Sınıf Nedir?
Abstract sınıflar barındırdığı metodların iç detaylarını vermeden yazıldığı sınıflardır. Ortak özellikler içerek sınıflar için bir temel sınıf oluşturmak için kullanılır. Interface'ten farklı olarak metot detaylarını belirtmemiz mümkündür ve tüm sınıflar tekrar yazma gereksinimi duymaksızın kullanabilmektedir. 
## Farkları
- Interfacelerde metot içlerinin doldurulması gerekmezken abstract sınıflarda metotlar gövdeli ya da gövdesiz olabilir. 
- Abstract sınıflardan alınan metodların override şeklinde kullanılması gerekirken interfacelerdeki metodlar direkt kullanılabilir.
- Interfacelerde sadece default şekilde public olarak gelen erişim belirleyicisine sahipken abstract sınıflar keyword olarak diğer belirleyicilere sahip olabilir.
-  Bir sınıfın birden fazla interface ile extend edilmesi mümkünken (çoklu kalıtım özelliği) sadece bir abstract sınıftan extend edilebilir [[11](https://youtu.be/_xk7-jA07Q8) - [12](https://youtu.be/g8G6xjDKZhQ)]. 

# Kaynaklar
1. İnternet: Yazılım Lisans Tipleri (MIT, Apache, GNU) </br>
https://medium.com/@mehmet.baran/yaz%C4%B1l%C4%B1m-lisans-tipleri-mit-apache-gnu-1397af4d1fbb
2. İnternet: Açık Kaynak Lisansları - Yusuf Aytas </br>
https://www.yusufaytas.com/acik-kaynak-lisanslari/
3. İnternet: Git Merge ve Rebase’in Farkı Nedir ? </br>
https://medium.com/@halilibrahim_4325/git-merge-ve-rebasein-fark%C4%B1-nedir-1c6c81086fa9
4. İnternet: Git'te merge --squash ve rebase arasındaki fark nedir? </br>
https://qastack.info.tr/programming/2427238/in-git-what-is-the-difference-between-merge-squash-and-rebase 
5. İnternet: What is Agile? | Atlassian </br>
https://www.atlassian.com/agile
6. İnternet: What is Scrum? </br>
https://www.scrum.org/resources/what-is-scrum
7. İnternet: 5 Soruda Kanban Nedir? Ne Değildir?  </br>
https://listelist.com/kanban-nedir/ 
8. İnternet: Kanban Explained in 10 Minutes | Kanbanize </br>
https://kanbanize.com/kanban-resources/getting-started/what-is-kanban
9. İnternet: Tasarım Kalıpları Nedir?  </br>
https://deryacakmak.medium.com/tasar%C4%B1m-kal%C4%B1plar%C4%B1-nelerdir-cd216ba47921 
10. İnternet: 4 branching workflows for Git.  </br>
https://medium.com/@patrickporto/4-branching-workflows-for-git-30d0aaee7bf 
11. İnternet: Java Programlama Dersleri 33 - Interfaceler  </br>
https://youtu.be/_xk7-jA07Q8
12. İnternet: Java Programlama Dersleri 35 - Abstract Classlar  </br>
https://youtu.be/g8G6xjDKZhQ
