
Kanadalı bir programcının Lisp compiler yapımını anlattığı
https://github.com/orangeduck/BuildYourOwnLisp
daki kodların Windows için derlenmiş versiyonu.

Windows'ta derleyebilmek için libedit kütüphanesi ve readline.h ve edithistory.h kurulmuş ve Makefile üzerinde gerekli değişiklikler yapıldı.

Ayrıca lispy.exe'nin kurulduğu klasöre gitmek zorunda kalmadan
lispy.exe'nin mevcut klasörden çalıştırılabilmesi için, Windows.h dahilindeki
GetModuleFileName ile main.c dosyası modifiye edildi.

Ortaya cıkan lispy.exe kurulum klasörü. Kurulum için klasörü Program Files içine açıp path Sistem Değişkeni sonuna ;C:\Program Files\lispy-1.0; ekleyin (restart gerektirebilir) CMD.exe veya PowerShell üzerinden çalıştırabilirsiniz.

https://yadi.sk/d/_sCzikr-xV-7vQ

Not: Sadece Windows 7'de derlenmiş ve denenmiştir.

Örnek bir fonksiyon  çalıştırma anı:

[image]!(https://i.ibb.co/pPD9QJk/lispy.png)
