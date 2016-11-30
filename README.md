KittiBELLgym app
===================

Célkitűzés
----------
Az alkalmazásban vendégként egy edzőterem órarendje és az edzések leírása tekinthető meg, bejelentkezett edzőként van lehetőség az órarend módosítására.  Van lehetőség regisztrációra, bejelentkezés után az (edző) felhasználók megtekinthetik és módosíthatják a saját edzéseiket, hozzáadhatnak újakat, valamint törölhetik őket.


----------


Funkcionális követelmények
----------
**Vendégként**:

 - a főoldalon szeretném megtekinteni az órarendet
 - szeretném megtekinteni az órák információit
 - szeretnék regisztrálni az oldalra

**Felhasználóként**:

 - szeretnék bejelentkezni az oldalra és kijelentkezni
 - szeretném tudni megtekinteni, módosítani, törölni a saját óráimat,
   illetve hozzáadni újakat


----------


Nem funkcionális követelmények
----------
 - Felhasználóbarát, ergonomikus elrendezés és kinézet.
 - Gyors működés.
 - Biztonságos működés: jelszavak tárolása, funkciókhoz való hozzáférés.


----------

Szerepkörök
----------
**Regiszrtációt nem igénylő:**

 - Látogató (visitor): megtekintheti az aktuális heti edzéseket órarend
   formájában és az edzések információit

**Regisztrációhoz kötött:**

 - Edző(trainer): saját óráit kezelheti: új, módosítás, törlés


----------


Használati esetek
----------
![hasznalatiesetek](https://github.com/kittimut/KittiBellGym/blob/master/photos/hasznalatiesetdiag.jpg)


----------


Adatmodell
----------
![adatmodell](https://github.com/kittimut/KittiBellGym/blob/master/photos/adatmod.jpg)


----------

Adatbázis
----------
![adatbazis](https://github.com/kittimut/KittiBellGym/blob/master/photos/adatb.jpg)

----------

Oldaltérkép
----------
**Publikus:**

 - Látogató:
	 - Főoldal(Órarend)
	 - Edzés információk
	 - Bejelentkezés
	 - Regisztráció

**Bejelentkezéshez kötött:**

 - Edző:
	 - Új edzés hozzáadása
	 - Meglévő saját edzés szerkesztése
	 - Meglévő saját edzés törlése
	 - Kijelentkezés

----------

Végpontok 
----------

**Mindenki által elérhető végpontok:**
*Vendég:*
/timetable - Főoldal, Órarend
/register - Regisztráció
/login - Bejelentkezés
/logout - Kijelentkezés
/timetable/:id - Edzés információk


**Autentikációhoz kötött végpontok:**
*Edző:*
/timetable/create - Új edzés hozzáadása
/timetable/:id/delete - Meglévő saját edzés törlése
/timetable/:id/edit - Meglévő saját edzés módosítása


---------


Oldalvázlatok
----------
![home](https://github.com/kittimut/KittiBellGym/blob/master/photos/Index.jpg)
![login](https://github.com/kittimut/KittiBellGym/blob/master/photos/Login.jpg)
![reg](https://github.com/kittimut/KittiBellGym/blob/master/photos/Registration.jpg)
![editTimetable](https://github.com/kittimut/KittiBellGym/blob/master/photos/editTimetable.jpg)
![createTimetable](https://github.com/kittimut/KittiBellGym/blob/master/photos/createTimetable.jpg)
![ClassPageVisitor](https://github.com/kittimut/KittiBellGym/blob/master/photos/ClassPageVisitor.jpg)
![ClassPageTrainer](https://github.com/kittimut/KittiBellGym/blob/master/photos/ClassPageTrainer.jpg)
