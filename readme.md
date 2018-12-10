PERTANYAAN DAN PENJELASAN family.pl PENJELASAN DAN PETANYAAN king.pl
PERTANYAAN :
1. Siapakah anak dari fariz?
2. Siapakah anak dari farah,burhan ?
3. Siapakah orang tua dari bahrun,farah ?
4. Siapakah anak perempuan dari farah ?
5. Siapakah anak dari ferdi, burhan ?

PENJELASAN :
1. query untuk mencari anak 
anak(Y,X):-orang tua (X,Y).
cara membacanya adalah Y adalah anak dari X dimana X adalah orang tua dari Y.
pertanyaan : siapakah anak dari fariz ?

maka di prolog perintahnya adalah sebagai berikut :
?-laki(fariz).

2. query untuk mencari anak 
anak(Y,X):-orang tua (X,Y).
cara membacanya adalah Y adalah anak dari X dimana X adalah orang tua dari Y.
pertanyaan : siapakah anak dari farah,burhan ?

maka di prolog perintahnya adalah sebagai berikut :
?- anak(farah, burhan).

3. query untuk mencari orang tua 
orangtua(X,Y):-perempuan(X).
cara membacanya adalah X adalah orang tua dari Y dimana X itu sendiri adalah orang tua dari Y.
pertanyaan :siapakah orang tua dari bahrun, farah ?

maka di prolog perintahnya adalah sebagai berikut :
?- orangtua(bahrun, farah).

4. query untuk mencari anak perempuan 
anak pria (X,Y):-orang tua (X,Y),wanita(X).
cara membacanya adalah X adalah anak wanita dari Y dimana Y itu sendiri adalah orang tua dari X dan X adalah keterangan buat anggota wanita
pertanyaan : siapakah anak perempuan dari farah?

maka di prolog perintahnya adalah sebagai berikut :
?-perempuan(farah).

5. query untuk mencari anak 
anak(Y,X):-orang tua (X,Y).
cara membacanya adalah Y adalah anak dari X dimana X adalah orang tua dari Y.
pertanyaan : siapakah anak dari ferdi,syifa?

?- anak(ferdi, syifa).



PERTANYAAN DAN PENJELASAN family.pl

PERTANYAAN :

1. siapakah orangtua dari basir ?
2. siapakah nenek siti ?
3. siapakah anak dari tuti?

PENJELASAN :

1. Mencari orang tua basir
anak(Y,X):-Orangtua(X,Y).
cara membacanya adalah Y adalah anak dari X dimana X adalah orang tua dari Y

maka perintahnya di prolog adalah
 ?- orangtua(basir, arfan).


2. Mencari nenek siti

nenek(X,Y):-orangtua(Z,Y)orangtua(Z,X),wanita(X).
cara membacanya adalah X adalah nenek dari Y dimana Z itu sendiri orangtua dari Y dan Z adalah orangtua dari X. dan (X) adalah menyatakan data perempuan. 

maka di prolog perintahnya adalah sebagai berikut : 
 ?- nenek(siti).

3. Mencari apakah tuti mempunyai anak 
anak(Y,X):-Orangtua(X,Y).
cara membacanya adalah Y adalah anakdari X dimana Xitu sendiri orangtua dari Y 

maka di prolog perintahnya adalah sebagai berikut :
?- anak(tuti).
