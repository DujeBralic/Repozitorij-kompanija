# Baidu Apollo Robotaxi: 

U nastavku donosim detaljniju analizu iskustva s Baiduovim Apollo robotaksijima.  
O ovoj i još nekoliko tema pisat ću u širem osvrtu s nedavnog posjeta kineskim tehnološkim kompanijama.  
U svjetlu trgovinskog „rata“, posebno je zanimljivo promotriti kineski tehnološki sektor koji – za razliku od američkih tehnoloških giganata – još uvijek nije dovoljno poznat široj javnosti na Zapadu.  
Upravo tu leže i neki od ključnih razloga sve izraženijih trgovinskih i ekonomskih tenzija između dviju sila.

## Baidu: Od tražilice do cloud computinga i autonomne vožnje u Kini

**Baidu** je vodeća kineska tehnološka kompanija, najpoznatija po svojoj internetskoj tražilici – „kineskom Googleu“.  
No, kompanija ulaže ogromna sredstva u razvoj **umjetne inteligencije**, **cloud infrastrukture** i **autonomne mobilnosti**.  
Jedan od najzrelijih projekata u tom smislu je upravo **Apollo Robotaxi** – autonomni taksi sustav koji djeluje u stvarnim urbanim okruženjima.

## Nivoi autonomije

Autonomna vozila dijele se u šest razina – od 0 do 5. Na razini 0, vozilo nema nikakvu autonomiju i sve kontrolira vozač, dok razina 1 omogućuje jednu funkciju pomoći (npr. tempomat). Na razini 2, vozilo može istovremeno upravljati i kočiti/gasiti, ali vozač mora stalno nadgledati vožnju. 
- Razina 3 omogućuje vozilu da samostalno vozi u određenim situacijama, no očekuje se da vozač preuzme kontrolu kad sustav to zatraži.
- Kod razine 4, vozilo može u potpunosti voziti bez vozača, ali samo unutar unaprijed definiranih zona (npr. pametni gradski dijelovi).

Apollo koji smo testirali stoga možemo klasificirati kao Level 3/4.

- Razina 5 znači potpuno autonomno vozilo koje može voziti bilo gdje, bez volana, papučica ili potrebe za ljudskom prisutnošću – u potpunosti preuzima ulogu vozača.


## Iskustvo vožnje: Bez osjećaja da vozač (ni)je u sjedalu

Tijekom posjeta korporativnom središtu Baidu u Pekingu, imao sam priliku isprobati Apollo robotaxi unutar Baidu kampusa nekoliko kilometara.
Vozilo se naručuje putem jednostavne aplikacije – dovoljno je nekoliko klikova, i taksi dolazi za svega par minuta.  
Vožnja je bila izuzetno ugodna i precizna, gotovo neprimjetno autonomna, unatoč postignutoj brzini od **70 km/h**.

Vozilo nas je prevezlo tih nekoliko kilometara bez potrebe za intervencijom vozača – osim na jednoj točki gdje su nedavno prebojene prometne linije, pa je sigurnosni vozač preuzeo upravljanje nakon zvučnog i vizualnog upozorenja.  
Vožnja se ne pokreće ako svi putnici nisu vezani, a svaki putnik ima ekran s prikazom okoline, senzora i navigacije u stvarnom vremenu.

Trenutno Apollo robotaksiji prometuju komercijalno u nekoliko kineskih gradova, najviše u **Wuhanu**, a javno su dostupni na korištenje u **Beijing Economic-Technological Development Area** – zoni s naprednom **V2X infrastrukturom**.  
Planira se širenje na tržišta Bliskog Istoka, uključujući **UAE**.


Kako sustav funkcionira?

## Tehnološki temelj: Tri stupa autonomije

### 1. Vehicle-to-Everything (V2X)

Vozila komuniciraju s infrastrukturom, drugim vozilima, pješacima i mobilnom mrežom. Primjerice, auto može “znati” da će semafor uskoro postati crven, da se iza ugla približava drugo vozilo, ili da pješak prelazi cestu, čak i ako ga vozač ne vidi.
**5G mreža** je ključna za ovu povezanost, ali i za uključivanje pametnih uređaja (mobitela, bicikala) u sustav upravljanja prometom.

### 2. Internet of Things (IoT) i Edge Computing

Semafori, križanja i prometnice umreženi su s **lokalnim računalnim čvorištima** (edge computing nodes) uz cestu koja omogućuju brzu obradu podataka.  

Lokalni računalni čvorovi su lokalni poslužitelji uz cestu koji u stvarnom vremenu obrađuju podatke za autonomna vozila, a uz 5G vezu visoke kvalitete smanjuju latenciju (kašnjenje i nestabilnost signala). Također omogućuju donošenje odluka lokalno pomoću lokalnih modela bez ovisnosti povezivosti s cloudom. To omogućuje brzu reakciju ako se npr. pješak pojavi naglo.


### 3. Senzorski sustavi

Apollo vozila koriste:
- **LiDAR** (3D mapiranje okoline)
- **Radar** (detekcija pri slaboj vidljivosti)
- **Kamere** (prepoznavanje traka, znakova, pješaka)
- **Ultrazvučne senzore** (detekcija na manjim udaljenostima)
- **GNSS+IMU sustav** (precizno pozicioniranje)

Svi podaci se kombiniraju s **deep learning algoritmima** za donošenje odluka u realnim prometnim situacijama. Deep learning algoritmi u V2X sustavu omogućuju vozilu da uči iz goleme količine podataka koje prima iz okoline – od kamera, senzora, drugih vozila i prometne infrastrukture – kako bi prepoznalo situacije (npr. pješak na cesti, naglo kočenje ispred), razumjelo kontekst i automatski odlučilo što treba učiniti – usporiti, stati ili zaobići prepreku. Ukratko, uči iz iskustva.

Drugim riječima, ti algoritmi omogućuju autu da ne reagira samo po pravilima, nego i da "shvati" što se događa oko njega i prilagodi se situaciji u stvarnom vremenu.

## Infrastruktura i regulativa: Ključ za skaliranje

Peking je predvodnik u omogućavanju testiranja i operacija autonomnih vozila, no i drugi kineski gradovi aktivno razvijaju vlastite **pametne prometne zone**, uz atraktivne poticaje i brže procedure licenciranja.

U Kini, **HD mapiranje** je klasificirano kao osjetljiva informacija i dozvoljeno je samo odobrenim domaćim tvrtkama.  
Podaci prikupljeni vozilima ne smiju se izvoziti bez posebnog odobrenja – dio šireg koncepta **digitalnog suvereniteta**. Baidu surađuje s lokalnim vlastima, telekomima i proizvođačima vozila na razvoju cjelovitog **ekosustava autonomne vožnje**.

Također, Tesla Elona Muska i Baidu su u strateškom partnerstvu – Tesla donosi naprednu Full Self Driving (FSD) tehnologiju , dok Baidu osigurava legalnu i tehničku infrastrukturu potrebnu za operacije u Kini. Tesla aktivno pokušava dobiti licencu za FSD u Kini. Tesla je i dalje lider u količini podataka iz prometa koje prikuplja i načinu kako iste koristi u treningu neuralnih mreža, no za pristup tržištu je potreban lokalni partner. Ovo je ustaljeni model gdje strani investitor ulazi na kinesko tržište putem domaćeg partnera koji štiti suverenitet podataka i infrastrukture.

## Budućnost autonomne mobilnosti

Za kraj, kakvi poslovni modeli i usluge mogu nastati pojavom robotaxija na ulicama? Otvara se prostor za razvoj čitavog niza digitalnih usluga – od personaliziranog infotainmenta i internetske kupovine unutar vozila, do lokacijskih preporuka i oglašavanja u realnom vremenu. Robotaksiji postaju dio šire mobilnosti kao servisa (MaaS), integrirani s javnim prijevozom i raznim loyalty sustavima. U pozadini se razvijaju pametni gradski sustavi temeljeni na prometnoj analitici i podatcima u stvarnom vremenu, dok vozila bez putnika omogućuju autonomnu dostavu hrane, paketa i robe.   Izgledno je da će u narednim godinama širenje ovih sustava se dogoditi relativno brzo na Bliskom Istoku (UAE, Saudijska Arabija), te u globalnim metropolama. No ono što bi izgledno mogla biti prepreka su infrastrukturni limiti, regulatorna crvena vrpca i pitanja oko informacijske sigurnosti, odnosno digitalnog suvereniteta.

