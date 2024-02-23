BBC Basic Raytracer in 432 characters
=====================================

https://mastodon.me.uk/@bbcmicrobot/111762132859648345

```basic
REMĀĘĆĞ$Č*Ēĉ!ăě-ĕ'ď
MODE1:VDU5
FORN=8TO247:FORM=0TO319
X=0:Y=-.1:Z=3:U=(M-159.5)/160:V=(N-127.5)/160:W=1/SQR(U*U+V*V+1):U=U*W:V=V*W:I=SGNU:G=1
E=X-I:F=Y-I:P=U*E+V*F-W*Z:D=P*P-E*E-F*F-Z*Z+1:IFD>0T=-P-SQRD:IFT>0X=X+T*U:Y=Y+T*V:Z=Z-T*W:E=X-I:F=Y-I:G=Z:P=2*(U*E+V*F-W*G):U=U-P*E:V=V-P*F:W=W+P*G:I=-I:GOTO50
IFV<0P=(Y+2)/V:V=-V*((INT(X-U*P)+INT(Z-W*P)AND1)/2+.3)+.2
GCOL0,3-(48*SQRV+?(PAGE+5+M MOD4+N MOD4*4)/3)DIV16
PLOT69,4*M,4*N:NEXT,
```
* [ZX Spectrum Raytracer](https://gabrielgambetta.com/zx-raytracer.html)
    * Spectrum ractracer tutorial
    * Adds dithering (which is pretty narly with spectrum 8x8 color chunks)

https://bbcmic.ro/?t=9ctpk

https://bbcmic.ro/#%7B%22v%22:1,%22program%22:%22REM%C4%80%C4%98%C4%86%C4%9E$%C4%8C*%C4%92%C4%89!%C4%83%C4%9B-%C4%95'%C4%8F%5CnREM%20ordered%20dither%20pattern%20stored%20in%20REM%20statement%20above;%204x4%20grid%20of%20thresholds%5CnMODE1:REM%20set%20320x256,%204%20colour%20graphics%20mode%5CnVDU5:REM%20hide%20flashing%20text%20cursor%20by%20enabling%20draw-text-at-graphics-cursor%20mode%5CnX=0:Y=-.1:Z=3:REM%20camera%20position%5CnFOR%20N=8%20TO%20247:REM%20iterate%20over%20screen%20pixel%20rows%5CnFOR%20M=0%20TO%20319:REM%20iterate%20over%20screen%20pixel%20columns%5CnU=(M-159.5)/160:REM%20x%20component%20of%20ray%20vector%5CnV=(N-127.5)/160:REM%20y%20component%20of%20ray%20vector%5CnW=1/SQR(U*U+V*V+1):REM%20z%20component%20of%20ray%20vector%5CnU=U*W:V=V*W:REM%20normalise%20x%20and%20y%20components%5CnI=SGNU:REM%20is%20ray%20facing%20left%20or%20right?%20I%20becomes%20x%20and%20y%20coordinates%20for%20sphere%5CnC=FNray(X,Y,Z,U,V,W,I):REM%20fire%20ray%20from%20X,Y,Z%20along%20U,V,W%5CnGCOL0,3-(48*SQRC+?(PAGE+5+M%20MOD4+N%20MOD4*4)/3)DIV16:REM%20set%20draw%20colour%20using%20ordered%20dithering%5CnPLOT69,4*M,4*N:REM%20plot%20pixel%20(4x%20multiplier%20due%20to%20resolution-independent%20graphics%20coordinates%20-%201280x1024)%5CnNEXT%5CnNEXT%5Cn%5CnDEFFNray(X,Y,Z,U,V,W,I)%5CnE=X-I:F=Y-I:G=Z:REM%20vector%20from%20sphere%20centre%20to%20ray%20start%5CnP=U*E+V*F-W*G:REM%20dot%20product?%20Z%20seems%20to%20be%20flipped%5CnD=P*P-E*E-F*F-G*G+1%5CnIF%20D%3C=0%20=FNc(X,Y,Z,U,V,W):REM%20didn't%20hit%20anything;%20return%20colour%5CnT=-P-SQRD:IF%20T%3C=0%20=FNc(X,Y,Z,U,V,W):REM%20still%20didn't%20hit%20anything;%20return%20colour%20%20%20%20%5CnX=X+T*U:Y=Y+T*V:Z=Z-T*W:REM%20new%20ray%20start%20position%5CnE=X-I:F=Y-I:G=Z:REM%20vector%20from%20sphere%20centre%20to%20new%20ray%20start%5CnP=2*(U*E+V*F-W*G):REM%20dot%20product%20shenanigans?%5CnU=U-P*E:V=V-P*F:W=W+P*G:REM%20new%20ray%20direction%20vector%5CnI=-I:REM%20we'd%20hit%20one%20sphere,%20so%20flip%20x%20and%20y%20coordinates%20to%20give%20other%5Cn%5Cn=FNray(X,Y,Z,U,V,W,I):REM%20return%20colour%20from%20new%20ray%5Cn%5CnDEFFNc(X,Y,Z,U,V,W):REM%20generate%20pixel%20colour%5CnIF%20V%3E=0%20=V:REM%20facing%20up%20at%20all?%20return%20ray%20Y%20component%20for%20simple%20sky%20gradient%5CnP=(Y+2)/V:REM%20use%20height%20for%20overall%20checkerboard%20scale%20and%20y%20component%20of%20vector%20for%20perspective%5Cn=-V*((INT(X-U*P)+INT(Z-W*P)AND1)/2+.3)+.2:REM%20multiply%20simple%20gradient%20by%20checkerboard%5Cn%22%7D

