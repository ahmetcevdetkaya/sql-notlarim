# sql-notlarim
## ***SQL NEDİR?***
-Sql,verileri depolayıp işlemeye yarayan yazılım dilidir.
### **SQL VERİ TİPLERİ*
-1.Metinsel Veri Tipleri
-2.Binary(İkilik) Veri Tipleri
-3.Sayısal Veri Tipleri
-4.Parasal Veri Tipleri
-5.Tarih-Zaman Veri Tipleri
-6.Diğer Veri Tipleri


-1.***Metinsel Veri Tipleri***
-**char:** Kapladıkları alanlar yönünden benzer olar için kullanılır maksimum 8000 karakteri destekler.Unicod desteklemez
-**nchar:** Char gibidir ama 4000 karatere kadar destekle  ve Unicod destekler 
-**varchar:** Charın aksine verinin boyutu kadar yer kaplar Unicod desteklemez
-**nvarchar:** Varcharın aksine Unicod destekler
-**text:** Belirtilenden az veride girilse boyutu kadar yer kaplar 2gb a kadar destekeler Unicodu desteklemez
-**ntext:** Textin aksine verinin boyutu kadar yer kaplar Unicodu Destekler
(Unicod:Her karakterin Rakamsal bir karşılığı olan yazılım dilidir)


-2.***Binary(İkilik) Veri Tipleri
-**binary:** 1 ve 0'ları temsil ettiği yazılım dilidir 8000byte a kadar destekler
-**varbinary:** Binary'in aksine verinin boyutu kadar yer kaplar
-**image:** Resim dosyalarını saklamak için kullanılır-genelde yerine varbinary kullanılır-


-3.***Sayısal Veri Tipleri***
-**bit:** Mantıksal verileri yani evet/hayır(0 ve 1) şeklinde bilgiyi tutmak için kullanılır
-**int:** 4 byte büyüklüğünde, -2 milyar /+2 milyar arasında değer tutabilen tam sayı veri tipidir.
-**bigint:** 8 byte büyüklüğünde -2⁶³ ve 2⁶³ arasında değer tutabilen tam sayı veri tipidir.
-**smallint:**  2 byte büyüklüğünde -32.768 ve 32.768 arası değer alabilen tam sayı veri tipidir.
-**tinyint:** 1 byte büyüklğüne sahip, 0–255 arası tam sayı veriler için kullanılan tam sayı veri tipidir.
-**decimal,numeric:** İkisinin de kullanımı aynıdır.Bu veri tipinde saklanacak sayının basamak sayısı tanımlanabilir.Veri tipi boyutu belirtilen basamak sayılarına göre değişkenlik gösterebilir.-38 ve +38 basamak arası verileri depolayabilir. -10³⁸ ,10³⁸ arası ondalık ve tam sayı türünde veri saklayabilir.
