# JobFlow

## Csapattagok

* Borbély Attila
* Tóth Áron Máté

---

## 1. Az alkalmazás célja

A JobFlow egy modern, reszponzív álláskereső és álláshirdető webalkalmazás, amelynek célja, hogy egy közös platformon kapcsolja össze a munkát kereső felhasználókat és a munkavállalókat kereső vállalatokat.

Az alkalmazás lehetőséget biztosít a munkakeresők számára, hogy részletes szakmai és személyes profiljukat létrehozzák, különböző szempontok alapján állások között keressenek, majd a számukra megfelelő állásokra jelentkezzenek.

A projekt egyik fontos újítása, hogy a hagyományos, külön elkészítendő és feltöltendő önéletrajz helyett a felhasználó részletes digitális profilt tölthet ki. A profil a végzettséget, munkatapasztalatot, készségeket, nyelvismeretet és egyéb releváns információkat strukturált formában tartalmazza.

Ennek célja, hogy a felhasználónak ne kelljen minden alkalommal külön önéletrajzot készítenie vagy frissítenie. A részletes profil egyszeri kitöltése után az adatok több funkcióban is felhasználhatók, például állások kereséséhez, jelentkezésekhez és az AI alapú jelöltértékeléshez.

A rendszer további innovációja, hogy a felhasználó bizonyos, a foglalkoztatási támogatások szempontjából releváns személyes körülményeket is opcionálisan megadhat. Ezek alapján a rendszer a munkáltató számára jelezheti, hogy érdemes lehet utánanézni az adott jelentkezőhöz kapcsolódó támogatási lehetőségeknek.

Ezek az adatok nem kötelezőek. A felhasználó maga döntheti el, hogy megadja-e őket, mivel egyes személyes körülmények – például a családi állapot – magánjellegű információk lehetnek.

A projekt másik kiemelt funkciója egy AI alapú jelöltértékelési rendszer, amely az álláshirdetés követelményeit és a jelentkező rendelkezésre álló szakmai adatait összevetve 0–100 közötti megfelelési pontszámot és részletes szöveges értékelést készít.

A rendszer célja egy átlátható, könnyen használható és technikailag jól strukturált webalkalmazás létrehozása, amely alkalmas az álláskeresési és munkaerő-kiválasztási folyamat digitális támogatására.

---

## 2. Az alkalmazás általános bemutatása

A JobFlow két fő felhasználói szerepkört kezel: a munkavállalót és a munkáltatót.

A látogatók regisztráció nélkül is megtekinthetik az álláshirdetéseket és használhatják az álláskeresési funkciókat. Jelentkezéshez, illetve álláshirdetés létrehozásához azonban regisztráció és bejelentkezés szükséges.

A regisztráció során a felhasználó meghatározza saját szerepkörét. Ettől függően a rendszer a megfelelő funkciókat és felületet biztosítja számára.

A munkavállalók részletes digitális profilt tölthetnek ki, amely tartalmazhatja többek között a végzettséget, munkatapasztalatot, készségeket, nyelvismeretet és munkavégzési preferenciákat.

A profil célja, hogy strukturált formában tartalmazza azokat az információkat, amelyeket egy hagyományos önéletrajzban is meg lehetne adni. Így a felhasználónak nincs szüksége külön önéletrajz-fájl készítésére és feltöltésére.

A profil egyes, támogatási lehetőségek szempontjából releváns adatai opcionálisan adhatók meg. A felhasználó eldöntheti, hogy megosztja-e ezeket az információkat.

A munkáltatók saját vállalati profilt hozhatnak létre, majd ezen keresztül álláshirdetéseket adhatnak fel. Az álláshirdetésben megadhatják a munkakör legfontosabb jellemzőit, a fizetési tartományt, a munkaidőt, a műszakbeosztást és a minimális követelményeket.

Az álláshirdetések alapértelmezett érvényességi ideje 30 nap. A lejárathoz közeledő hirdetésekről a rendszer előre meghatározott időpontokban, például 7 és 1 nappal a lejárat előtt, értesítést készít.

---

## 3. Felhasználói szerepkörök

### 3.1. Munkavállaló

A munkavállaló az álláskeresésben és a meghirdetett pozíciókra történő jelentkezésben vesz részt.

A munkavállaló lehetőségei:

* regisztráció és bejelentkezés
* email-cím megerősítése
* részletes személyes és szakmai profil létrehozása
* végzettség megadása
* munkatapasztalatok rögzítése
* készségek és azok szintjének megadása
* nyelvismeret megadása
* munkavégzési preferenciák beállítása
* teljes vagy részmunkaidős munkavégzés megadása
* opcionális, támogatási lehetőségek szempontjából releváns adatok megadása
* álláshirdetések keresése és szűrése
* álláshirdetések részletes megtekintése
* állásokra történő jelentkezés
* korábbi jelentkezések és azok állapotának megtekintése.

A részletes profil szolgál a jelentkezések és az AI alapú jelöltértékelés szakmai adatforrásaként.

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
* jelentkezők részletes szakmai profiljának megtekintése
* jelentkezések státuszának módosítása
* lehetséges támogatási lehetőségekre vonatkozó jelzések megtekintése
* AI alapú jelöltértékelés használata.

---

## 4. Főbb funkciók

### 4.1. Regisztráció és bejelentkezés

A rendszer külön regisztrációs lehetőséget biztosít a munkavállalók és a munkáltatók számára.

A regisztráció során a felhasználó megadja a szükséges adatokat, valamint kiválasztja a kívánt szerepkört.

A jelszavakat a rendszer nem egyszerű szövegként, hanem biztonságos hash formájában tárolja. A bejelentkezett felhasználó munkamenetét PHP session kezeli.

A rendszer email megerősítést is használ. A regisztráció után a felhasználó egy megerősítő hivatkozással aktiválhatja a fiókját.

### 4.2. Munkavállalói profil

A munkavállaló részletes digitális szakmai profilt hozhat létre.

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

A profilban bizonyos további, támogatási lehetőségek szempontjából releváns személyes adatok is megadhatók.

Ezeknek a megadása opcionális. A felhasználó maga dönthet arról, hogy megosztja-e ezeket az információkat.

Például opcionálisan megadható lehet az egyedülálló családi állapot is, amennyiben az adott támogatási lehetőség szempontjából releváns lehet.

A profil célja, hogy a felhasználó egyetlen helyen tartsa karban a szakmai és az álláskeresés szempontjából releváns adatait, így nincs szükség külön önéletrajz-fájl elkészítésére és feltöltésére.

A profil adatai az álláskeresés és az AI alapú jelöltértékelés során is felhasználhatók.

A támogatási szempontok alapján megjelenített információk tájékoztató jellegűek. A rendszer nem állapít meg automatikusan jogi értelemben vett támogatási jogosultságot.

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

### 4.4. Álláshirdetések kezelése

A munkáltatók saját vállalati profiljukon keresztül álláshirdetéseket hozhatnak létre.

A hirdetéshez megadható:

* munkakör megnevezése
* rövid és részletes leírás
* munkavégzés helye
* kategória
* teljes vagy részmunkaidő
* hétvégi munkavégzés
* műszakbeosztás
* minimális végzettség
* szükséges szakmai tapasztalat
* szükséges készségek
* szükséges nyelvismeret
* egyéb követelmények
* minimális és maximális fizetés.

A létrehozott álláshirdetés alapértelmezett érvényességi ideje 30 nap.

A lejárt hirdetésekre a rendszer nem enged új jelentkezést.

### 4.5. Jelentkezések kezelése

A munkavállaló egy álláshirdetés részletes oldaláról jelentkezhet a meghirdetett pozícióra.

A rendszer ellenőrzi, hogy a felhasználó jogosult-e a jelentkezésre, illetve korábban jelentkezett-e már ugyanarra az állásra.

Egy munkavállaló ugyanarra az álláshirdetésre csak egyszer jelentkezhet.

A jelentkezéshez kapcsolódóan a rendszer eltárolja többek között:

* a jelentkező személyét
* az álláshirdetést
* a jelentkezés időpontját
* a jelentkezés aktuális státuszát.

A munkáltató a jelentkezések státuszát kezelheti, például megtekintett, elfogadott vagy elutasított állapotokra módosíthatja.

A jelentkezés során a munkáltató a jelentkező részletes szakmai profilját tekintheti meg a hozzáférési szabályoknak megfelelően.

### 4.6. AI alapú értékelés

A rendszer egyik kiemelt funkciója az AI alapú jelöltértékelés.

Az értékelés során a rendszer összeveti az álláshirdetésben megadott követelményeket a jelentkező strukturált szakmai profiljával.

Az értékelés eredménye tartalmazhat:

* 0–100 közötti megfelelési pontszámot
* rövid összefoglalót
* a jelentkező erősségeit
* a hiányzó követelményeket
* részletes szöveges magyarázatot.

Az értékelés célja a munkáltató munkájának támogatása és a jelentkezők közötti információfeldolgozás megkönnyítése.

Az AI eredménye nem helyettesíti a munkáltató döntését. A végső kiválasztási döntést a munkáltató hozza meg.

Az ismételt, szükségtelen AI lekérdezések elkerülése érdekében a rendszer az értékelések eredményét adatbázisban tárolhatja.

### 4.7. Támogatási lehetőségek jelzése

A rendszer egyik innovatív funkciója, hogy a munkáltató számára jelezheti, ha egy jelentkező profiljában található adatok alapján érdemes lehet utánanézni valamilyen foglalkoztatási támogatási lehetőségnek.

A funkció célja nem a támogatás automatikus megítélése, hanem a munkáltató tájékoztatása és a lehetséges lehetőségek könnyebb felismerése.

A támogatási szempontokhoz kapcsolódó bizonyos profiladatok opcionálisan adhatók meg.

A rendszer az ilyen adatok alapján nem használhatja ezeket az információkat a jelentkező szakmai alkalmasságának csökkentésére vagy növelésére.

A tényleges támogatási jogosultságot mindig az adott támogatási program aktuális feltételei alapján kell ellenőrizni.

---

## 5. Technológiák

### 5.1. Frontend

A felhasználói felület kialakításához az alábbi technológiákat használjuk:

* HTML5
* Bootstrap 5
* Tailwind CSS
* JavaScript.

A Bootstrap 5 elsősorban a reszponzív elrendezés és a komponensek kialakítását támogatja. A Tailwind CSS utility osztályai az egyes egyedi vizuális megoldások kialakításában használhatók.

A JavaScript a dinamikus felhasználói interakciókat és az oldal egyes háttérben végrehajtott kéréseit kezeli.

### 5.2. Backend

A backend XAMPP környezetben futó PHP segítségével készül.

A PHP felel többek között:

* a felhasználók kezeléséért
* a munkamenetekért
* a jogosultságok ellenőrzéséért
* az adatbázis-műveletekért
* az álláshirdetések kezeléséért
* a jelentkezések feldolgozásáért
* a profiladatok kezeléséért
* az API-szerű végpontok működtetéséért
* az AI API-val történő kommunikációért
* a támogatási lehetőségekhez kapcsolódó adatok feldolgozásáért.
