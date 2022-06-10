---
title: 'Aspose Alıcı B&#252;ltenin, Aralik 2007'
date: Tue, 04 Dec 2007 13:38:00 +0000
draft: false
url: /2007/12/04/aspose-al-c-b-ltenin-aralik-2007/
author: Salman Sarfraz
summary: ''
tags: ['Aspose Turkey']
---

**In This Issue**

*   **Hoşgeldiniz!**
*   **Ürün Vitrini – [Aspose.Pdf][1]**
*   **Aspose.BarCode çıkış yapıyor**
*   **Daha optimize bir Aspose.Slides for Java**
*   **Excel 2007 XLSX dosyalarını Aspose.Cells for Java ile alıp verin**
*   **Aspose.Words for .NET 4.4.2.0 Çıktı**
*   **Teknik Ipucu - Yeni tablo motoruyla son Aspose.Slides'a çabuk geçiş**
*   **Aspose.Total for Reporting Services Ürün Paketi**

**Hoşgeldiniz**

Aspose Bülten'in Aralık 2007 sayısına hoşgeldiniz. Bu ayki bültenimizde vitrin ürünü Aspose.Pdf hakkında bilgilendirme yapacağız. Ayrıca .Total for Reporting Services, Aspose.Words, Aspose.Cells, Aspose.Slides ve Aspose.BarCode ürünlerimizin son sürümlerindeki yeni ve heyecan verici özelliklere göz atacağız. Aspose'dan son haberleri alırken bir yandan da aylık Teknik İpucu sayesinde yeni tablo motoru sayesinde Aspose.Slides'a nasıl çabucak geçebileceğinizi göstereceğiz.

**Ürün Vitrini**

[**Apose.Pdf**][2] .NET veya Java uygulamalarının Adobe Acrobat kullanmadan PDF dokümanları yaratmasını sağlayan bir PDF dokümanı raporlama bileşenidir. Aspose.Pdf uygun fiyatlıdır ve pek çok kuvvetli özellik içerir: sıkıştırma, tablolar, grafikler, resimler, linkler, güvenlik, özel fontlar gibi. Aspose.Pdf API, XML şablonu ve XSL-FO dosyalarından PDF dosyası yaratılmasını destekler. Aspose.Pdf kullanımı çok kolaydır ve 14 adet hem C# hem de Visual Basic'te yazılmış demo içerir. Lütfen ücretsiz deneme sürümünü [**indirip**][3] Aspose.Pdf'in sizin ihtiyaçlarınızı nasıl karşılayacağını görün.

**Aspose.BarCode çıkış yapıyor**

[**Aspose.BarCode**][4] ürünlerinde oldukça çok ilerleme kaydedildi. Aspose.BarCode dokümantasyonu yeni baştan yazıldı. Detaylar için lütfen **resmi sayfayı** ziyaret edin. Aspose.BarCode for .NET için yeni bir de sürüm çıktı (**detaylar**) [**Buradan**][5] downlaod edebilirsiniz. [**Aspose.BarCode for Reporting Services**][6] için de bir takım zenginleştirmeler yapıldı ve v1.2.0.0 (**detaylar**) çıktı. [**Buradan**][7] download edebilirsiniz.

**Daha optimize bir Aspose.Slides for Java**

[**Aspose.Slides**][8] for Java'nın yeni sürümü 1.8.0.0 çıktı. Bu yeni sürüm yeni ve optimize edilmiş tablo motoru ve PPT dosyası okuyup yazmak için önemli hafıza ve hız optimizasyonları içeriyor. Pek çok yeni özellik arasında OLE1 nesnelerinin dosya isimlerini okuma ve gelişmiş metin gerçekleyicisi var. Pek çok hata da giderildi. Son sürüm [**buradan**][9] indirilebilir. Daha fazla detay için lütfen **resmi sayfayı** ziyaret ediniz.  

**Excel 2007 XLSX dosyalarını Aspose.Cells for Java ile alıp verin**

[**Aspose.Cells**][10] for Java v1.9.1 artık Excel 2007 XLSX dosyalarını alıp vermeyi destekliyor. Ayrıca bu sürümde PHP ile kullanabilme ve verileri değer aralığında sıralama özelliklerini destekliyor. Pek çok hata giderildi ve geliştirme yapıldı. Son sürüm [**buradan**][11] indirilebilir. Daha fazla bilgi için lütfen **resmi sayfayı** ziyaret edin.

**Aspose.Words for .NET 4.4.2.0 Çıktı**

[**Aspose.Words**][12] for .NET v4.4.2.0 çıktı. Bu Aspose.Words için bir bakım sürümü ve başta DOCX alma geliştirmeleri ve düzeltmeleri olmak üzere pek çok geliştirme ve düzeltme içeriyor. Lütfen son sürümü [**buradan**][13] indirin. Daha fazla bilgi için lütfen **resmi sayfayı** ziyaret edin.  

**Teknik İpucu –  
    Yeni tablo motoruyla son Aspose.Slides'a çabuk geçiş**

[**Aspose.Slides**][14] for .NET 2.7.0 (ve for Java 1.8.0) yeni tablo motoru ve açık API getirdi ve bu eski sürümlerle tam uyumlu değil. En önemli değişiklik hücre sınırlarının işlenmesi. Eskiden sınır stilini değiştirmek için bu tarz bir şey yazılırdı:  
  
  
\[C#\]  
  
// Accessing the cell in first row and first column  
Cell cell = table.GetCell(0,0);  
// Accessing the top border of the cell  
CellBorder border = cell.TopBorder;  
// Setting the color of the top border  
border.LineFormat.ForeColor = Color.Red;  
// Setting the width of the top border  
border.LineFormat.Width = 3;  
  
\[VB\]  
  
' Accessing the cell in first row and first column  
Dim cell As Cell =  table.GetCell(0,0)  
' Accessing the top border of the cell  
Dim border As CellBorder =  cell.TopBorder  
' Setting the color of the top border  
border.LineFormat.ForeColor = Color.Red  
' Setting the width of the top border  
border.LineFormat.Width = 3  
  
\[Java\]  
  
// Accessing the cell in first row and first column  
Cell cell = table.getCell(0,0);  
// Accessing the top border of the cell  
CellBorder border = cell.getTopBorder();  
// Setting the color of the top border  
border.getLineFormat().setForeColor(Color.RED);  
// Setting the width of the top border  
border.getLineFormat().setWidth(3);  
  
Birleştirilmiş hücrelerin sınırları işlenemeyen bazı satırlara sahipti. Yeni tablo motoru bunun için çok basit bir mekanizma sunuyor. Her hücre sınırının satırlara döngüsü var. Yani yeni sürümlere geçmek için kodu bu şekilde yazmanız lazım:  
  
\[C#\]  
  
// Accessing the cell in first row and first column  
Cell cell = table.GetCell(0,0);  
// Accessing the top border of the cell  
CellBorder border = cell.TopBorder;  
// Accessing the iterator of the lines in top border of the cell  
IEnumerator iter = border.GetEnumerator();  
// Loop through all the lines  
while (iter.MoveNext())  
{  
    Line line = (Line) iter.Current;  
    // Setting the color of the top border  
    line.LineFormat.ForeColor = Color.Red;  
    // Setting the width of the top border  
    line.LineFormat.Width = 3;  
}  
  
\[VB\]  
  
' Accessing the cell in first row and first column  
Dim cell As Cell =  table.GetCell(0,0)  
' Accessing the top border of the cell  
Dim border As CellBorder =  cell.TopBorder  
' Accessing the iterator of the lines in top border of the cell  
Dim iter As IEnumerator =  border.GetEnumerator()  
' Loop through all the lines  
While iter.MoveNext()  
    Dim line As Line = CType(iter.Current, Line)  
    ' Setting the color of the top border  
    line.LineFormat.ForeColor = Color.Red  
    ' Setting the width of the top border  
    line.LineFormat.Width = 3  
End While  
  
\[Java\]  
  
// Accessing the cell in first row and first column  
Cell cell = table.getCell(0,0);  
// Accessing the top border of the cell  
CellBorder border = cell.getTopBorder();  
// Accessing the iterator of the lines in top border of the cell  
Iterator iter = border.iterator();  
// Loop through all the lines  
while (iter.hasNext())  
{  
    Line line = (Line) iter.next();  
    // Setting the color of the top border  
    line.getLineFormat().setForeColor(Color.RED);  
    // Setting the width of the top border  
    line.getLineFormat().setWidth(3);  
}  

**Aspose.Total for Reporting Services Ürün Paketi**

Aspose olarak üçüncü büyük ürün paketimiz olan [**Aspose.Total for Reporting Services**][15]’ı piyasaya sürmekten çok mutluyuz. Aspose.Total for Reporting Services paketi SQL raporlamayı geliştiren, değişik formatlarda rapor yaratılmasını sağlayan beş değişik gerçekleme uzantısı içeriyor. Kurulduğu 2002’den beri Aspose’un odak noktası dosya yönetimi olmuştur. Bu yeni ürün yelpazesi de bu eforun devamı olarak veritabanı uzmanlarının ihtiyacı olan araçları sağlamayı hedefliyor. Paketin deneme sürümü [**buradan**][16] indirilebilir. Daha fazla bilgi için lütfen **resmi ürün sitesini** ziyaret edin.




[1]: http://www.aspose.com/Products/Aspose.Pdf/Default.aspx
[2]: http://www.aspose.com/Products/Aspose.Pdf/Default.aspx
[3]: http://www.aspose.com/Community/Files/51/aspose.pdf/default.aspx
[4]: http://www.aspose.com/Products/Aspose.Barcode/
[5]: http://www.aspose.com/Community/Files/53/aspose.barcode/category1082.aspx
[6]: http://www.aspose.com/Products/Aspose.BarCode.Reporting.Services/
[7]: http://www.aspose.com/Community/Files/52/aspose.barcode.reporting.services/category1217.aspx
[8]: http://www.aspose.com/Products/Aspose.Slides/
[9]: http://www.aspose.com/Community/Files/51/aspose.slides/category1199.aspx
[10]: http://www.aspose.com/Products/Aspose.Cells/
[11]: http://www.aspose.com/Community/Files/51/aspose.cells/entry102877.aspx
[12]: http://www.aspose.com/Products/Aspose.Words/
[13]: http://www.aspose.com/Community/Files/51/aspose.words/entry103596.aspx
[14]: http://www.aspose.com/Products/Aspose.Slides/
[15]: http://www.aspose.com/Products/Aspose.Total/
[16]: http://www.aspose.com/Community/Files/50/aspose.total.for.reporting.services/default.aspx



