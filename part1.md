# HTML Eğitim Serisi

Bu seri, HTML öğrenmeye yeni başlayanlar için hazırlanmıştır. Her derste önce konu kısaca anlatılır, sonra senin yazdığın kod aynen verilir ve en sonda kodda kullanılan önemli etiketler açıklanır.

---

# Ders 1: HTML Başlangıç

## Bu Derste Ne Öğreniyoruz?

Bu derste bir HTML sayfasının temel yapısını, başlık etiketlerini, paragraf yazmayı, satır boşluğu bırakmayı ve çizgi eklemeyi öğreniyoruz.

## Kod

```html
<!DOCTYPE html> <!--html 5 e uyumlu-->

<html> <!--html açılış etiketi-->
    <head> <!--web sitesi hakkında bilgiler-->
        <title> <!--sayfa başlığı-->
            Hoş Geldiniz
        </title>
    </head>
    <body> <!--web sitesinde gözükmesi istenenler-->
        merhaba
        <h1>merhaba</h1> <!--başlık etiketleri-->
        <br> <!--arada boşluk-->
        <h2>m</h2>
        <hr> <!--arada çizgili boşluk-->
        <h3>m</h3>
        <h4>m</h4>
        <h5>m</h5>
        <h6>m</h6>
        <p>Dümdüz Yazı</p> <!--Dümdüz yazı yazdırır-->
    </body>
</html> <!--html kapanış etiketi-->
```

## Kod Üzerinden Açıklama

`<!DOCTYPE html>` sayfanın HTML5’e uygun olduğunu belirtir.

`<html>` etiketi HTML sayfasının başladığını gösterir.

`<head>` bölümü kullanıcıya direkt görünmeyen, sayfa hakkında bilgilerin bulunduğu bölümdür.

`<title>` tarayıcı sekmesinde görünen sayfa başlığıdır.

`<body>` web sitesinde görünen yazıların ve içeriklerin bulunduğu bölümdür.

`<h1>` ile `<h6>` arasındaki etiketler başlık oluşturmak için kullanılır. `h1` en büyük, `h6` en küçük başlıktır.

`<br>` satır boşluğu bırakır.

`<hr>` sayfaya yatay çizgi ekler.

`<p>` paragraf yazmak için kullanılır.

---

# Ders 2: Hyperlink

## Bu Derste Ne Öğreniyoruz?

Bu derste HTML’de link vermeyi öğreniyoruz. Linkler sayesinde kullanıcıyı başka bir siteye veya sayfaya yönlendirebiliriz.

## Kod

```html
<!--! yazıp entera basarsak bütün lazım olan etiketler geliyor-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>hyperlink</title>
</head>
<body>
    <a href="https://www.youtube.com">youtube</a> <!--href parametresi gidilmesi gereken yeri yazmamız için-->     <!--a enter yapınca otomatik gelir-->
<br>
    <a href="https://www.youtube.com"
target="_blank"
title="Youtube'a gider">Youtube Yeni Sekme</a> <!--target parametresi yeni sekmeye gönderir title ise üstüne gelince yazı yazdırır-->

</body>
</html>
```

## Kod Üzerinden Açıklama

`<a>` etiketi link oluşturmak için kullanılır.

`href` parametresi linkin hangi adrese gideceğini belirtir.

`target="_blank"` linkin yeni sekmede açılmasını sağlar.

`title` kullanıcının linkin üzerine gelince göreceği küçük açıklamayı oluşturur.

Bu örnekte YouTube’a giden normal bir link ve yeni sekmede açılan bir link gösterilmiştir.

---

# Ders 3: Image

## Bu Derste Ne Öğreniyoruz?

Bu derste HTML sayfasına görsel eklemeyi öğreniyoruz. Görseller web sayfalarını daha anlaşılır ve görsel olarak daha güzel hale getirir.

## Kod

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image</title>
</head>
<body>
    <img src="foto/htmllogo.png" alt=""> <!--resim eklemek için img kullanılır src parametresi fotoğrafın kaynağını ister-->
    <br>
    <img src="foto/htmllogo.png" alt="" width="250px"> <!--widht parametresi fotoğrafın genişliğini belirler-->
    <br>
    <img src="foto/htmllogo.png" alt="" width="250px" height="10px"> <!-- height boyu belirler-->
    <br>
    <img src="foto/htmllogo.png" alt="HTML Fotosu" width="250px" height="250px"> <!-- alt foto hakkında bilgi verir okuyan kişinin inti o an yetmediyse alt çıkar-->
    <br>
    <img src="foto/htmllogo.png" title="HTML Fotoğrafı" width="250px" height="250px"> <!-- title fotoyu mouseun yanına götürünce pop up çıkmasını sağlar-->
</body>
</html>
```

## Kod Üzerinden Açıklama

`<img>` etiketi sayfaya resim eklemek için kullanılır.

`src` fotoğrafın dosya yolunu belirtir.

`width` fotoğrafın genişliğini ayarlar.

`height` fotoğrafın yüksekliğini ayarlar.

`alt` fotoğraf yüklenmediğinde görünen açıklama yazısıdır.

`title` fotoğrafın üzerine gelince çıkan küçük açıklamadır.

Bu derste aynı görselin farklı özelliklerle nasıl gösterilebileceği anlatılmıştır.

---

# Ders 4: Audio

## Bu Derste Ne Öğreniyoruz?

Bu derste HTML sayfasına ses dosyası eklemeyi öğreniyoruz. Ses dosyaları müzik, konuşma veya efekt olarak kullanılabilir.

## Kod

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <audio src="müzik/mj.mp3" controls></audio> <!--srcye müziğin kaynağını ister controls sitede gözükmesi içindir-->
  <br>
    <audio src="müzik/mj.mp3" controls autoplay muted></audio> <!--site açılınca sesin oynaması için autoplay girilir muted ise sesi kapalı çaldırır.-->
  <br>
    <audio src="müzik/mj.mp3" controls loop></audio> <!--loop ses bittikçe tekrar çalar.-->
</body>
</html>
```

## Kod Üzerinden Açıklama

`<audio>` etiketi sayfaya ses eklemek için kullanılır.

`src` ses dosyasının kaynağını belirtir.

`controls` ses oynatma kontrollerini gösterir.

`autoplay` sayfa açılınca sesin otomatik başlamasını sağlar.

`muted` sesi kapalı başlatır.

`loop` ses bittikten sonra tekrar çalmasını sağlar.

Bu derste aynı ses dosyasının normal, otomatik başlayan ve tekrar eden kullanımları gösterilmiştir.

---

# Ders 5: Video

## Bu Derste Ne Öğreniyoruz?

Bu derste HTML sayfasına video eklemeyi öğreniyoruz. Video etiketi sayesinde site içinde video oynatabiliriz.

## Kod

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <video src="video/sf.mp4" width="500px" controls></video> <!--src kaynak width genişlik controls oynatmak için gerekli-->
    <br>
    <video src="video/sf.mp4" width="500px" controls autoplay muted loop></video> <!--autoplay site açılınca otomatik videoyu başlatır muted videonun sesini kısık başlatır loop ise video bittikçe başa döndürür-->
</body>
</html>
```

## Kod Üzerinden Açıklama

`<video>` etiketi sayfaya video eklemek için kullanılır.

`src` videonun dosya yolunu belirtir.

`width` videonun genişliğini ayarlar.

`controls` video oynatma kontrollerini gösterir.

`autoplay` sayfa açılınca videonun otomatik başlamasını sağlar.

`muted` videoyu sessiz başlatır.

`loop` video bitince tekrar başa döndürür.

Bu derste normal video kullanımı ve otomatik başlayıp tekrar eden video kullanımı gösterilmiştir.

---

# Ders 7: Metin Biçimlendirme

## Bu Derste Ne Öğreniyoruz?

Bu derste HTML’de yazıların görünümünü değiştirmeyi öğreniyoruz. Yazıları kalın, italik, küçük, büyük, alt simge, üst simge, altı çizili, üstü çizili ve fosforlu gösterebiliriz.

## Kod

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <p>Normal Yazı</p>
    <p><b>Kalın</b> Yazı</p> <!--b etiketi kalınlaştırır-->
    <p><i>İtalik</i> Yazı</p><!--i etiketi italik yapar-->
    <p> <big>Büyük </big> Yazı</p> <!--big etiketi büyütür-->
    <p> <small>Küçük </small> Yazı</p> <!--small etiketi küçültür-->
    <p><sub>alt</sub> sembol</p> <!--sub yazıyı alta alır-->
    <p><sup>üst</sup> sembol</p> <!--sup yazıyı üste alır-->
    <p><ins>Altı</ins> Çizili Yazı</p> <!--ins yazının altını çizer-->
    <p><del>Üstü</del> Çizili Yazı</p> <!--del yazının üstünü çizer-->
    <p><mark>Fosforlu</mark> Yazı</p> <!--mark yazıyı fosforlar-->
</body>
</html>
```

## Kod Üzerinden Açıklama

`<p>` paragraf yazmak için kullanılır.

`<b>` yazıyı kalınlaştırır.

`<i>` yazıyı italik yapar.

`<big>` yazıyı büyütür.

`<small>` yazıyı küçültür.

`<sub>` yazıyı alta alır.

`<sup>` yazıyı üste alır.

`<ins>` yazının altını çizer.

`<del>` yazının üstünü çizer.

`<mark>` yazıyı fosforlu gösterir.

Bu derste metinlerin HTML etiketleriyle nasıl biçimlendirileceği gösterilmiştir.

---

# Seri Özeti

Bu eğitim serisinde HTML’in temel konuları işlendi:

1. HTML başlangıç yapısı
2. Hyperlink kullanımı
3. Görsel ekleme
4. Ses ekleme
5. Video ekleme
7. Metin biçimlendirme

Her derste kodlar korunarak, kodun ne işe yaradığı açıklanmıştır.

