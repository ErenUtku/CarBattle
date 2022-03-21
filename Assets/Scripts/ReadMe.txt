18 Mayis

GUNLUK

*Oyunu kafamdan gecirdim ve hemen iki arabanin karsilikli gelebilecegi bir zemin hazirladim. Ilk basta araba icin bir 
hareket mekanizmasi yapip bunu hem player icin hem de hazirlayacagim AI icin kullanacagim.

*Oyuncunun satin alabilecegi 3 tane etmen olmasi gerektigine karar kildim. biri arabanin agirligi digeri hizi bir digeri ise itis(vites) gucu

*Muhtemelen agirlik ve hiz degiskenlerini satin almak cok kolay olacaktir direk arabanin icersindeki tanimlanmis degerlerin uzerine eklenerek devam edilecektir.

*Vites icin 2 adet buton dusunuyorum bir tanesi arabaya gaz verip bir digeri belirtilen araliga gelindiginde vites atmasini yani arabaya itis gucu saglamasi hedeflendi

*Su an AI icin bir sey dusunmedim ama oyuna player icin alacagim upgradelerin en azindan bir kaci AI ya uygulanmassa oyun cok kolay olur.

*AI icin 3 saniyede bir atabilecegi bir itis kuvveti ayarlayacagim ama bunun kesinlikle belli bir degerin uzerinde olmasi disinda bir randomize eklemek istiyorum
boylece bot surekli ayni itme gucunu almayip karsisinda gercekten bir player varmis hissiyati verebilirim.

YAPTIKLARIM

- Araba ekledim ve bu arabanin gidebilmesi icin 4 ceker bir araba sistemi tasarladim, motor ve agirlik gucuyle calisan bu sistemi abstract class ile yazip
Ai uzerinede ekledim. Denemek icin ai uzerine 3 saniyede bir gelen bir itis gucu verdim. playerin ustune tiklanildiginda ise ona itis gucu veren bir mekanizma hazirladim

- UI hazirladim, Bu UI uzerinde engine body ve gear adi altinda 3 adet satin alinabilir icerik koydum, Win condisyonunda 1000 
lose condisyonunda da 1000=? ancak kendini tekrar eden lose condisyonlarinda atanilan intiger deger kadar bu sayi bolumme ugrayacaktir.

-Su an mouseinput ile gecis yaptigim oyun ekranina Time scale kullanarak arabalari durdurdum. Time scale in daha saglikli olabilecegini dusundum, Bunu 
Awake metoduna yazarak olasi buglardan sakindim.(arabanin saniyelik hareket etmesi gibi). Bunu ilerde degistirebilirim.

-Level Manager ekledim, icine normalde 2 tane condisyon koyacaktim ama su an sadece aracin statlarini kontrol etmek icin kaybetme collideri koydum. Bu oyunun time scale
ini 0 layip scenin restartlamasini sagliyor.

DUSUNCELERIM

-Simdilik arabaya gaz ve vites icin birer tus atayacagim ve bunu player classi icerisinde tanimlayacagim.

-AI icin playerin statlarina oranla artip azalan bir sistem yapabilecegimi dusunuyorum , ornegin eger arabamiza agirlik satin alirsak ai'in motor hizi
10 arttirilabilir.


/*------------------------------------------------------------------------*/

19 Mayis

*Bugun arabanin satin alim sirasinda yasadigi problemi cozdum, Artik hem satin aldiginda hem de satin almadiginda elindeki valueyle yani player prefle oynayabiliyor.

*Bir slider ekledim bu slider mouse tusuna basildiginda doluyor biraktiginda azaliyor, space tusuna basildiginda belli bir miktar geri gidiyor. Saridaysa 0 a yesildeyse biraz ortaya kirmizida bastiysa 
0 a yakin bir degerden gaza basmaya basliyor.

*Slider ve araba iliskisi cozuldu, Artik problemsiz bir sekilde arabaya vites atabiliyoruz. Araba kirmizi cizgiye 2,5 saniye boyunca durursa arac bozuluyor oyuncu kontrolu kaybediyor,
muhtemelen ai da itecegi icin bir sure sonra oyunu kazaniyor.

/*------------------------------------------------------------------------*/
 
20 Mayis 

*Dun playerla ilgili her seyi tamamladim, sadece AI in nasil bir davranis yapacagini cozmem lazim.



