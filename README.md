# sql-notlarim
## ***SQL NEDİR?***
-Sql,verileri depolayıp işlemeye yarayan yazılım dilidir.
### **SQL VERİ TİPLERİ*
- 1.Metinsel Veri Tipleri
- 2.Binary(İkilik) Veri Tipleri
- 3.Sayısal Veri Tipleri
- 4.Parasal Veri Tipleri
- 5.Tarih-Zaman Veri Tipleri
- 6.Diğer Veri Tipleri


- 1.***Metinsel Veri Tipleri***
- **char:** Kapladıkları alanlar yönünden benzer olar için kullanılır maksimum 8000 karakteri destekler.Unicod desteklemez
- **nchar:** Char gibidir ama 4000 karatere kadar destekle  ve Unicod destekler 
- **varchar:** Charın aksine verinin boyutu kadar yer kaplar Unicod desteklemez
- **nvarchar:** Varcharın aksine Unicod destekler
- **text:** Belirtilenden az veride girilse boyutu kadar yer kaplar 2gb a kadar destekeler Unicodu desteklemez
- **ntext:** Textin aksine verinin boyutu kadar yer kaplar Unicodu Destekler
(Unicod:Her karakterin Rakamsal bir karşılığı olan yazılım dilidir)


- 2.***Binary(İkilik) Veri Tipleri
- **binary:** 1 ve 0'ları temsil ettiği yazılım dilidir 8000byte a kadar destekler
- **varbinary:** Binary'in aksine verinin boyutu kadar yer kaplar
- **image:** Resim dosyalarını saklamak için kullanılır-genelde yerine varbinary kullanılır-


- 3.***Sayısal Veri Tipleri***
- **bit:** Mantıksal verileri yani evet/hayır(0 ve 1) şeklinde bilgiyi tutmak için kullanılır
- **int:** 4 byte büyüklüğünde, -2 milyar /+2 milyar arasında değer tutabilen tam sayı veri tipidir.
- **bigint:** 8 byte büyüklüğünde -2⁶³ ve 2⁶³ arasında değer tutabilen tam sayı veri tipidir.
- **smallint:**  2 byte büyüklüğünde -32.768 ve 32.768 arası değer alabilen tam sayı veri tipidir.
- **tinyint:** 1 byte büyüklğüne sahip, 0–255 arası tam sayı veriler için kullanılan tam sayı veri tipidir.
- **decimal,numeric:** İkisinin de kullanımı aynıdır.Bu veri tipinde saklanacak sayının basamak sayısı tanımlanabilir.Veri tipi boyutu belirtilen basamak sayılarına göre değişkenlik gösterebilir.-38 ve +38 basamak arası verileri depolayabilir. -10³⁸ ,10³⁸ arası ondalık ve tam sayı türünde veri saklayabilir.


- 4.***Parasal Veri Tipleri***
- **money:** 8 byte boyutunda, yaklaşı -2⁶⁴ ile 2⁶⁴ arasında parasal değerleri tutmak için kullanılır. 4 basamağa kadar duyarlı ondalık tipli verileri saklar.
- **smallmoney** 4 byte uzunluğunda yaklaşık -214.000 ile 214.000 arası parasal değerleri tutmak için kullanılır.Money tipinde olduğu gibi 4 basamağa kadar duyarlı ondalık tipli verileri saklarken kullanılır.


- 5.***Tarih-Zaman Veri Tipleri*** 
- **date:** Tarihleri YYYY-AA-GG şeklinde saklamayı sağlar 4byte kadar destekler
- **smalldatetime:** Tarih ve zaman verilerini yıl-ay-gün ve saat-dakika-saniye-salise şeklide saklar.Date gibi 4byte kadar destekler
- **datetime:**: YYYY-AA-GG şeklinde tarih ve zaman verilerini tutar ve 8byta kadar destekler
- **datetime2:** Datetime göre salise hassasiyeti daha yüksetir 6-8byte kadar destekelr
- **time:** Sadece saat verilerini saat-dakika-saniye-salise saklamaya yarar
- **datetimeoffset:**  Ülkelere göre değişen zaman farkını hesaplayıp tutarken kullanılır.


-6.***Diğer Veri Tipleri***
- **sql_variant:** Sayı,metin, binary gibi farklı veri tiplerini depolamak için kullanılır
- **xml:**XML türünde veri saklamak için kullanılır. Kapasitesi 2 GB’dır
- **geometry:** Öklid koordinat sistemine ait verileri tutmak için kullanılır.
- **timestamp:**: Tabloya kayıt eklendiğinde , güncellendiğinde binary türünde özel değer alan veri tipidir.
- **uniqueidentifier:** 16 byte uzunluğunda benzersiz GUID tipinde veri tutar.İki GUID birbirinden tamamen farklıdır eşit olamazlar.
- **hierarchyid:** Ağaç veri modeli ve ya hiyerarşik olarak sınflandırılmış verileri saklamak için kullanılır.
- **geography:**  Coğrafi koordinat ve GPS verilerini tutmak için kullanılır.










**SQL SORGU KOMUTLARI NELERDİR?**
- Öncelikle neden SQL sorusuna cevap verelim,düşünün çalıştığınız şirketteki verileri düzenlemelisiniz ama belkide binlerce satır veri var elinizde manuel bir şekilde düzenlemek ne kadar kolay olurdu bir düşünün?İşte SQL burda devreye giriyor ve bizlere yardım ediyor.

- Peki SQL bize bu yardımı nasıl sunuyor sizi fazla yoramdan cevabı vereyim "SQl SORGU KOMUTLARI" yardımı ile peki SQL sorgu komutları nelerdir?

- **Sql select:** Basitçe istedğiniz veri tipindeki verileri size sunar
- Örnek olarak:
- Select ad,soyad, FROM müşteri
- Bu kodu yazdığınız zaman müşteri tablosundaki ad soyad verileri karşınıza çıkar

- **Sql select dıstınct:** Sql select size hem satır hem sütun olacak şekilde verileri gösterirken sql dıstınct size sütun olarak gösterir
- Örnek olarak:
- SELECT DISTINCT sehir FROM musteri;
- Bu kodu yazmanız halinde size yukarıdan-aşağıya doğru şehir isimlerini gösterecekdir

-**Sql where:** Sql select size bütün verileri gösterirken Sql where istedğiniz konumdaki verileri gösterir yani İstanbuldaki Müşteriler gibi
- Örnek olarak:
- SELECT * FROM musteri WHERE sehir='istanbul'
- Bu kodu yazmanız halinde size istanbuldaki müşterileri gösterir

-*Where komudu ile kullanabileğiniz operatörler*
- "=" = Eşit.
- "<>" = Eşit değil. Note:Bazı versiyonlarda "!=" kullanılabilir
- ">" = Büyüktür.
- "<" = Küçüktür.
- ">=" = Büyük Eşit.
- "<=" = Küçük Eşit.
- BETWEEN = Arasında.
- LIKE = Örüntü arama.
- IN = Bir sutün içindeki birden fazla olasığı belirlemek için

- _SQL AND-OR kullanımı_

- _SQl AND_
- 1.koşul ve 2.koşulun doğru olduğu durumlarda kullanılır
- Örneğin musteri tablosunda  Cinsiyeti “E” ve Şehri “İstanbul” olanları listelemek için;
- SELECT * FROM musteri WHERE sehir='İstanbul' AND cinsiyet='E' kodunu yazmanız gerekir

- _SQL OR_
- Aynı "And" komudu gibi 1.koşul ve 2. koşulun doğru olduğu durumlarda kullanılır
- Örneğin musteri tablosunda şehri İstanbul yada Samsun olanları listelemek için;
- SELECT * FROM musteri WHERE sehir='İstanbul'OR sehir='Samsun' kodunu yazmanız gerekir

- _SQL AND VE OR'U AYNI ANDA KULLANMA_
- Örnek olarak musteri tablosunda cinsiyeti ‘K’ olan ve Şehri “Konya” yada “Manisa” olanları listelemek için; 
- SELECT * FROM musteri WHERE cinsiyet='K' AND (City='Konya' OR City='Manisa') kodunu yazmak gerekir

- **Sql order by:**
![WhatsAppUIClone](https://user-images.githubusercontent.com/48753655/123524344-37a57a80-d6d2-11eb-9523-ba2f7a49a10b.PNG)

  

    

  


  




