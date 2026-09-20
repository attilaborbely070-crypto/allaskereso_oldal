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

A rendszer ellenőrzi, hogy a felhasználó jogosult-e a jelentkezésre, rendelkezik-e szükséges önéletrajzzal, illetve korábban jelentkezett-e már ugyanarra az állásra.

Egy munkavállaló ugyanarra az álláshirdetésre csak egyszer jelentkezhet.

A jelentkezéshez kapcsolódóan a rendszer eltárolja többek között:

* a jelentkező személyét
* az álláshirdetést
* a jelentkezéshez használt önéletrajzot
* a jelentkezés időpontját
* a jelentkezés aktuális státuszát.

A munkáltató a jelentkezések státuszát kezelheti, például megtekintett, elfogadott vagy elutasított állapotokra módosíthatja.

### 4.6. AI alapú értékelés

A rendszer egyik kiemelt funkciója az AI alapú jelöltértékelés.

Az értékelés során a rendszer összeveti az álláshirdetésben megadott követelményeket a jelentkező szakmai profiljával.

Az értékelés eredménye tartalmazhat:

* 0–100 közötti megfelelési pontszámot
* rövid összefoglalót
* a jelentkező erősségeit
* a hiányzó követelményeket
* részletes szöveges magyarázatot.

Az értékelés célja a munkáltató munkájának támogatása és a jelentkezők közötti információfeldolgozás megkönnyítése.

Az AI eredménye nem helyettesíti a munkáltató döntését. A végső kiválasztási döntést a munkáltató hozza meg.

Az ismételt, szükségtelen AI lekérdezések elkerülése érdekében a rendszer az értékelések eredményét adatbázisban tárolhatja.

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
* a fájlfeltöltések kezeléséért
* az API-szerű végpontok működtetéséért
* az AI API-val történő kommunikációért

### 5.3. Adatbázis

Az alkalmazás adatait MySQL adatbázis tárolja, amelyet fejlesztés közben phpMyAdmin segítségével kezelünk.

Az adatbázis több, egymással kapcsolatban álló táblát tartalmaz, például:

* `users`
* `employee_profiles`
* `employer_profiles`
* `work_experiences`
* `skills`
* `user_skills`
* `languages`
* `user_languages`
* `resumes`
* `jobs`
* `job_required_skills`
* `job_required_languages`
* `applications`
* `ai_evaluations`
* `email_verifications`
* `expiry_notifications`

Az adatbázisban elsődleges és idegen kulcsok biztosítják a táblák közötti kapcsolatokat.

## 6. Reszponzív kialakítás

A JobFlow felülete reszponzív kialakítású, ezért különböző képernyőméreteken is használható.

Az asztali nézetben a rendszer többoszlopos elrendezést alkalmazhat, például keresési és szűrési területet, központi álláslistát és kiegészítő információkat tartalmazó oldalsávot.

Kisebb kijelzőkön az elemek egymás alá rendeződnek, a navigáció és az űrlapok pedig mobil eszközön is használható formában jelennek meg.

A reszponzív kialakítás megvalósításában elsősorban a Bootstrap 5 grid rendszere és komponensei kapnak szerepet.



