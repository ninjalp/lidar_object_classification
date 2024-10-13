
lidar:lazer ışığı gönderip geri alır , tof ile çalışır , (ışık hızı *uçuş)/2 = buradan mesafe gelir .
360 derece döner ve o şekilde ışık gönderip alır .


lidardan açı ve mesafe verisi gelir .

açı ve mesafe bilgisinden nokta çıkartmak için :

r=mesafe

angle=açı


x= r * cos(angle)
y= r * sin(angle)

bu bize noktayı verir .

bu şekilde nokta bulutuna geçeriz .

makine öğrenmesi ile sınıflandırma yapacağımız için etiketli veriye ihtiyacımız var , 

o yüzden elde ettiğimiz noktaları bir uygulama penceresinde kare içine alarak etiketleyebiliriz.En azından ben öyle yaptım .

o noktalar hangi objeye aitse etiketledikten sonra , convex hull , dış bükey zarfını çıkartıp oradan sınıflandırmak mantıklı. CNN ile bu işi yapabiliriz.


