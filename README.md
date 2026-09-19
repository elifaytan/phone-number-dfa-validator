# Phone Number DFA Validator

Python kullanılarak geliştirilmiş, telefon numarası formatlarını Deterministik Sonlu Otomat (DFA) mantığı ile doğrulayan bir projedir.

Proje, Biçimsel Diller ve Otomatlar dersi kapsamında DFA yapısının gerçek bir problem üzerinde uygulanmasını göstermek amacıyla geliştirilmiştir.

## Projenin Amacı

Bu projede belirlenen telefon numarası formatına uygun girişlerin kabul edilmesi, hatalı formatların ise reddedilmesi amaçlanmıştır.

Telefon numarası:

0XXX XXX XX XX

biçimine uygun olacak şekilde kontrol edilmektedir.

Girilen karakterler DFA tarafından sırayla işlenir ve her karakter için mevcut durumdan bir sonraki duruma geçilir.

Giriş tamamlandığında DFA kabul durumundaysa telefon numarası geçerli, aksi durumda geçersiz kabul edilir.

## Kullanılan Yöntem

Projede Deterministik Sonlu Otomat (DFA) kullanılmaktadır.

Bir DFA temel olarak aşağıdaki bileşenlerden oluşur:

- Durumlar
- Giriş alfabesi
- Başlangıç durumu
- Geçiş fonksiyonu
- Kabul durumu

Her giriş karakteri için yalnızca bir sonraki durum bulunmaktadır. Bu nedenle sistem deterministik olarak çalışmaktadır.

## Çalışma Mantığı

Program kullanıcıdan bir telefon numarası alır.

Girilen telefon numarasındaki karakterler sırasıyla DFA tarafından kontrol edilir.

Her rakam veya boşluk karakteri için uygun durum geçişi gerçekleştirilir.

Beklenmeyen bir karakter veya yanlış format ile karşılaşıldığında giriş reddedilir.

Tüm karakterler başarıyla işlendiğinde ve DFA kabul durumuna ulaştığında telefon numarası geçerli kabul edilir.

## Kontrol Edilen Format

Program aşağıdaki yapıya uygun telefon numaralarını kontrol etmektedir:

    0XXX XXX XX XX

Örnek geçerli format:

    0532 123 45 67

Format içerisinde:

- İlk karakter `0` olmalıdır.
- Rakam grupları belirlenen uzunlukta olmalıdır.
- Gruplar arasındaki boşluklar doğru konumlarda bulunmalıdır.
- Fazladan veya eksik karakter bulunmamalıdır.

## DFA Yaklaşımı

Telefon numarasındaki her karakter için ayrı durum geçişleri kullanılmaktadır.

Örneğin:

    q0 -> q1 -> q2 -> q3 -> ... -> qAccept

Başlangıç durumu `q0` olarak düşünülebilir.

Her doğru karakter DFA'yı bir sonraki duruma geçirir.

Yanlış bir karakter veya format hatası ile karşılaşıldığında giriş kabul edilmez.

Son karakterden sonra kabul durumuna ulaşılması durumunda telefon numarası geçerlidir.

## Kullanılan Teknolojiler

- Python
- Jupyter Notebook
- Deterministic Finite Automaton (DFA)
- Finite State Machines
- Formal Languages
- Automata Theory

## Proje Dosyaları

- `Biçimsel_Proje_Kodu.ipynb` — DFA tabanlı telefon numarası doğrulama kodunun bulunduğu Jupyter Notebook
- `README.md` — Proje hakkında açıklamalar

## Çalıştırma

Projeyi çalıştırmak için Jupyter Notebook kullanılabilir.

`Biçimsel_Proje_Kodu.ipynb` dosyasını açın ve hücreleri sırasıyla çalıştırın.

Program tarafından istenen telefon numarasını belirlenen formatta girin.

Örnek:

    0532 123 45 67

DFA giriş karakterlerini sırayla kontrol ederek telefon numarasının formata uygun olup olmadığını belirler.

## Öğrenilen Kavramlar

Bu proje kapsamında aşağıdaki konular uygulamalı olarak kullanılmıştır:

- Deterministik Sonlu Otomat
- Durumlar
- Durum geçişleri
- Başlangıç durumu
- Kabul durumu
- Giriş alfabesi
- Geçiş fonksiyonu
- Biçimsel dil tanımlama
- Girdi doğrulama

## Projenin Amacı

Bu çalışma ile teorik olarak öğrenilen DFA kavramının gerçek bir doğrulama problemi üzerinde uygulanması amaçlanmıştır.

Telefon numarası formatının durumlar ve geçiş kuralları kullanılarak modellenmesi sayesinde sonlu otomatların metin ve format doğrulama problemlerinde nasıl kullanılabileceği gösterilmiştir.

## Proje Notu

Bu proje Biçimsel Diller ve Otomatlar dersi kapsamında geliştirilmiş akademik bir çalışmadır.
