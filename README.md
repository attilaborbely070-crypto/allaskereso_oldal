# JobFlow

## Csapattagok

* Borbély Attila
* Tóth Áron Máté

---

## 1. Az alkalmazás célja

A JobFlow egy modern, reszponzív álláskereső és álláshirdető webalkalmazás, amelynek célja, hogy egy közös platformon kapcsolja össze a munkát kereső felhasználókat és a munkavállalókat kereső vállalatokat.

Az alkalmazás lehetőséget biztosít a munkakeresők számára, hogy személyes és szakmai profiljukat létrehozzák, önéletrajzukat feltöltsék, különböző szempontok alapján állások között keressenek, majd a számukra megfelelő állásokra jelentkezzenek.

A munkáltatói oldalon a rendszer lehetőséget biztosít vállalati profil létrehozására, álláshirdetések készítésére és kezelésére, valamint a beérkező jelentkezések áttekintésére.

A projekt egyik kiemelt funkciója egy AI alapú jelöltértékelési rendszer, amely az álláshirdetés követelményeit és a jelentkező rendelkezésre álló szakmai adatait összevetve 0–100 közötti megfelelési pontszámot és részletes szöveges értékelést készít.

A rendszer célja egy átlátható, könnyen használható és technikailag jól strukturált webalkalmazás létrehozása, amely alkalmas az álláskeresési és munkaerő-kiválasztási folyamat digitális támogatására.

---

## 2. Az alkalmazás általános bemutatása

A JobFlow két fő felhasználói szerepkört kezel: a munkavállalót és a munkáltatót.

A látogatók regisztráció nélkül is megtekinthetik az álláshirdetéseket és használhatják az álláskeresési funkciókat. Jelentkezéshez, illetve álláshirdetés létrehozásához azonban regisztráció és bejelentkezés szükséges.

A regisztráció során a felhasználó meghatározza saját szerepkörét. Ettől függően a rendszer a megfelelő funkciókat és felületet biztosítja számára.

A munkavállalók részletes profilt tölthetnek ki, amely tartalmazhatja többek között a végzettséget, munkatapasztalatot, készségeket, nyelvismeretet és munkavégzési preferenciákat. A rendszerhez PDF vagy DOCX formátumú önéletrajz is feltölthető.

A munkáltatók saját vállalati profilt hozhatnak létre, majd ezen keresztül álláshirdetéseket adhatnak fel. Az álláshirdetésben megadhatják a munkakör legfontosabb jellemzőit, a fizetési tartományt, a munkaidőt, a műszakbeosztást és a minimális követelményeket.

Az álláshirdetések alapértelmezett érvényességi ideje 30 nap. A lejárathoz közeledő hirdetésekről a rendszer előre meghatározott időpontokban, például 7 és 1 nappal a lejárat előtt, értesítést készít.

---

## 3. Felhasználói szerepkörök

### 3.1. Munkavállaló

A munkavállaló az álláskeresésben és a meghirdetett pozíciókra történő jelentkezésben vesz részt.

A munkavállaló lehetőségei:

* regisztráció és bejelentkezés
* email-cím megerősítése
* személyes és szakmai profil létrehozása
* végzettség megadása
* munkatapasztalatok rögzítése
* készségek és azok szintjének megadása
* nyelvismeret megadása
* munkavégzési preferenciák beállítása
* PDF vagy DOCX önéletrajz feltöltése
* álláshirdetések keresése és szűrése
* álláshirdetések részletes megtekintése
* állásokra történő jelentkezés
* korábbi jelentkezések és azok állapotának megtekintése.

A jelentkezéshez a rendszerben érvényes önéletrajznak kell rendelkezésre állnia.

### 3.2. Munkáltató

A munkáltató a munkaerő keresését és a jelentkezések kezelését végzi.

A munkáltató lehetőségei:

* regisztráció és bejelentkezés
* email-cím megerősítése
* vállalati profil létrehozása
* vállalat adatainak szerkesztése
* álláshirdetés létrehozása
* álláshirdetés módosítása
* álláshirdetések megtekintése és kezelése
* munkaköri követelmények megadása
* fizetési tartomány megadása
* munkaidő és műszakbeosztás meghatározása
* jelentkezők megtekintése
* jelentkezők önéletrajzának megtekintése
* jelentkezések státuszának módosítása
* AI alapú jelöltértékelés használata.

---

## 4. Főbb funkciók

### 4.1. Regisztráció és bejelentkezés

A rendszer külön regisztrációs lehetőséget biztosít a munkavállalók és a munkáltatók számára.

A regisztráció során a felhasználó megadja a szükséges adatokat, valamint kiválasztja a kívánt szerepkört.

A jelszavakat a rendszer nem egyszerű szövegként, hanem biztonságos hash formájában tárolja. A bejelentkezett felhasználó munkamenetét PHP session kezeli.

A rendszer email megerősítést is használ. A regisztráció után a felhasználó egy megerősítő hivatkozással aktiválhatja a fiókját.

### 4.2. Munkavállalói profil

A munkavállaló részletes szakmai profilt hozhat létre.

A profilban megadható többek között:

* teljes név
* telefonszám
* lakóhely
* legmagasabb végzettség
* szakmai bemutatkozás
* munkavégzési preferencia
* teljes vagy részmunkaidős munkavégzés
* korábbi munkatapasztalatok
* szakmai készségek
* készségszintek
* nyelvismeret
* nyelvi szintek.

A profil adatai az álláskeresés és az AI alapú jelöltértékelés során is felhasználhatók.

### 4.3. Álláskeresés

A felhasználók a rendszerben található álláshirdetések között kereshetnek.

A keresés és szűrés több szempont alapján történhet, például:

* kulcsszó
* helyszín
* kategória
* foglalkoztatási forma
* fizetési tartomány
* végzettség
* műszakbeosztás
* hétvégi munkavégzés.

Az álláshirdetések részletes oldalán megjelennek a munkakör legfontosabb adatai, a munkáltató adatai, a munkavégzés helye, a fizetési tartomány és a munkakör követelményei.

