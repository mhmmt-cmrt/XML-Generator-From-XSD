# Xml-Class-Generator-From-Xsd

Bu Proje e dönüşüm uygulamaları kapsamında e belgelerde kullanılan xml belgesini üretmek amacıyla gerçekleştirilmiştir. 
 
Proje kapsamında ilk olarak e fatura uygulaması için xml oluşturulacaktır. Öncelikle aşağıdaki kütüphanenin kurulumu yapılır.

Install all dependencies.
>pip install xsdata[cli,lxml,soap].

Daha sonra ilgili modüle xml sınıflarının oluşturulacağı xsd dosyası ve sınıfların kaydedileceği paket ismi verilir.

Generate models.
>xsdata Files/xsdrt/maindoc/UBL-Invoice-2.1.xsd --generated.

Bu işlemden sonra elde edilen sınıflar kullanılarak xsd şemasında belirtilen formatlarda e fatura xml belgesi elde edilir.
E Müstahsil uygulaması içinde yine terminalde aşağıdaki kod koşularak ilgili xml sınıfları elde edilir ve bu sınıflar yardımıyla da e belge oluşturulur.

Generate models.
>xsdata Files/xsdrt/maindoc/UBL-CreditNote-2.1.xsd --generated
Proje kapsamında kullanılan xsd belgeleri Gelir İdare Başkanlığı tarafından yayınlar UBL-TR formatına uygun standart belgelerdir.
