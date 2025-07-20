# Unitree Robotics – Postoji li Business case za humanoidne robote?

Unitree Robotics je svjetski poznata tvrtka za istraživanje, razvoj, proizvodnju i prodaju višenamjenskih četveronožnih i humanoidnih robota te robotskih ruku za industrijske, civilne i sigurnosne namjene.

Posjetio sam njihov HQ u Hangzhou koji se nalazi u dijelu grada koji ima više centara velikih tehnoloških kompanija (NetEase, Alibaba, Didi, Hikvision, Megvii itd.), no u Unitree-u se još uvijek ponašaju kao startup. Sama zgrada je gotovo neprimjetna bez oznaka i raskošnog kampusa, no u izložbenom salonu koji se prostire na otprilike 100 (skromnih) kvadratnih metara stalno je bila gužva i veliki broj posjetitelja.

## Kratka povijest kompanije

Unitree je osnovao Wang Xingxing 2016. godine nakon što je u sklopu magisterija mehaničkog inženjerstva razvio robotskog psa (XDOG). Wang je 2 godine radio u DJI-u (proizvođač dronova), nakon čega se posvetio Unitree-u i iterativno razvio više verzija četveronožnih robota. To znači da kompanija ima gotovo desetljeće fokusiranog rada na razvoju tehnologije, što je dovelo do Go2 modela koji su popularni po društvenim medijima.

Originalni dizajn nije imao nikakve kamere ni napredne elektroničke sklopove, no to se do 2021. godine promijenilo. Osim značajnih iskoraka u tehnologiji koja je postavljena na samu konstrukciju (senzori), najveći pomaci su ostvareni u agilnosti, što se primarno odnosi na napredne zglobove (prijenosnici, aktuatori i legure kao ključne komponente).

Mnoge komponente koje čine ključne elemente Unitree robota (motori, harmonijski prijenosnici, senzori) danas su javno i komercijalno dostupne. Teoretski, svatko tko nabavi iste dijelove može sklopiti robota s usporedivim karakteristikama. Pravi "trik" je u optimizaciji mehaničke geometrije, sinkronizaciji senzora i kontrolnog softvera te detaljnoj kalibraciji svakog zgloba. To zahtijeva veliko iskustvo, puno testiranja i iteracija. Unitree ima preko 200 patenata u ovom području.

## Go2 – Četveronožni model

Go2 je stekao globalnu slavu preko društvenih medija jer može raditi akrobacije poput prevrtanja, front/back flipova, hodanja naopako, kotrljanja te penjanja stubama i kretanja po neravnom terenu. Težak je cca 15 kg i lako ga je dignuti s poda, a ima nosivost od 7-8 kg. Cijena "obične" AIR verzije je oko 1.400 EUR, a programabilna verzija EDU košta oko 8.000 EUR.

### Verzije Go2 robota

- **Air/Pro verzije** ne podržavaju otvoreni razvojni Software Development Kit (SDK) i ne mogu se "programirati" vlastitim kodom – mogu se kontrolirati isključivo putem mobilne aplikacije ili predefiniranih načina rada
- **Edu verzija** dolazi s punom podrškom za unitree_SDK2 (C++ i Python) i ostale razvojne alate, što otvara mogućnosti za prilagođene aplikacije i istraživanja
- **Baterija** traje od 4-8 sati, ovisno o korištenju

### Sustav percepcije

Sustav percepcije temelji se na 2 ključne komponente:

1. **4D LiDAR** s 360° × 90° vidnim poljem – detekcija prepreka od vrlo bliske udaljenosti (≥ 0,05 m) i izrada 3D karte okoline u realnom vremenu

2. **IMU (inerciometar i žiroskop)** visoke frekvencije za precizno praćenje nagiba, ubrzanja i orijentacije robota. IMU je mali "čip" koji mjeri ubrzanje i rotaciju robota te drži robota stabilnim. Ako mu noga sklizne, IMU "osjeti" naginjanje i kontroler brzo ispravlja pokret. Pomaže u praćenju položaja kad kamere nisu dovoljne (npr. u mraku)

### AI i algoritmi

Algoritmi su nepoznanica – u službenim materijalima spominje se GPT-pogon i trening AI kroz simulacije, ali bez detalja o tome koja se točno neuralna mreža ili model koristi. I tu dolazimo do glavnog pitanja oko budućih use case-ova ovih robota.

Unitree robote prvo "uče" u virtualnoj simulaciji (NVIDIA Isaac Gym), gdje isprobavaju i usavršavaju svoje korake u umjetno generiranom okruženju koje imitira stvarni svijet. Kada se pokaže da simulirani algoritam radi pouzdano, prenosi se u fizički robot i dodatno se prilagođava podacima iz senzora (LiDAR, IMU).

## H1 – Humanoidni robot

Imao sam priliku "hrvati se" s modelom H1-1, visine 160 cm i težine cca 47 kg. Iako sam ga pokušavao jako gurnuti, dosta se dobro držao na nogama. Novi model, H1-2 je viši (180 cm) i teži (70 kg), pa mislim da bi ga srušiti bilo još izazovnije. Po društvenim medijima lako se nađu videa gdje ih ljudi dosta grubo udaraju i guraju, no H1 se bez problema održi stabilnim.

### Cijena H1 modela

- **Osnovni, ne-programabilni model**: oko 15.000 EUR
- **Napredniji model**: oko 85.000 EUR

## "Embodied Intelligence: AI + Robot"

To je pojam kojim Unitree najavljuje integraciju AI modela (npr. LLM-ova) direktno na robota. Cilj bi bio da robot sam u realnom vremenu donosi složene odluke, prilagođava nagib ili strategiju kretanja te komunicira s okolinom i korisnikom. No pitanje je imaju li in-house kapacitete za razvoj takvih rješenja ili će morati ući u strateško partnerstvo za budući iskorak u sposobnostima.

### Izazovi za budući razvoj

Unitree prvenstveno dominira mehatronikom i kontrolom pokreta – njihov "core competency" je dizajn motora, mehaničkih zglobova, prijenosnika, sustava percepcije i kontrolnih petlji. Za Embodied Intelligence koncept dodatno će biti potrebno razviti cijeli sustav "fleet-learning" infrastrukture i Machine/Reinforcement Learning inženjeringa kakav imaju Baidu, Tesla i vodeći projekti autonomije.

Zbog impresivnog napretka u stabilnosti i agilnosti robota naglo su stekli globalnu reputaciju, pa mi izgledaju kao potencijalna akvizicijska meta za velike korporacije koje žele ući u svijet robotike.

## Zaključak

Unitree Robotics predstavlja zanimljiv slučaj tehnološke tvrtke koja je uspjela stvoriti impresivne robote s relativno skromnim resursima. Njihova snaga leži u izvrsnoj mehatronici i kontroli pokreta, dok je buduća konkurentnost uvjetovana sposobnošću integracije naprednih AI sustava. Business case za humanoidne robote još nije jasan, ali Unitree je pozicionirao sebe kao jedan od ključnih igrača u ovom nastajućem tržištu.
