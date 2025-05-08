# Laboratoare SSI

# Securitatea Sistemelor Informatice - Laborator 1

## 1. Noțiuni generale

Atribuirea termenilor corecți definițiilor:

- **(B) Securitate**: (1) O condiție care rezultă din stabilirea și menținerea măsurilor de protecție care permit unei organizații/sistem să își îndeplinească misiunea sau funcțiile critice, în ciuda riscurilor reprezentate de amenințări.
- **(D) Vulnerabilitate**: (2) Slăbiciune într-un sistem informațional, proceduri de securitate ale sistemului, controale interne sau implementare care ar fi putea fi exploatate sau declanșate de o sursă de amenințare.
- **(A) Adversar**: (3) O entitate (inclusiv un insider) care acționează rău intenționat pentru a compromite un sistem.
- **(E) Securitatea cibernetică**: (4) Capacitatea de a proteja / apăra spațiul cibernetic de atacuri cibernetice.
- **(C) Risc**: (5) O măsură a gradului în care o entitate este amenințată de o eventuală circumstanță sau eveniment.


## 3.

- **Conversia unei date în binar**
  - 24 (ziua nașterii) + 10 = 34
  - 34 în binar: `100010`
  - Conversia inversă: `100010` în decimal = **34**

- **Conversia unui număr hexazecimal de 4 cifre în binar**
  - Exemplu: `2F3A`
  - Conversia în binar: `0010 1111 0011 1010`
  - Conversia inversă: `0010 1111 0011 1010` → `2F3A`

## 4.

- **Codificarea ASCII a unui nume**
  - `ANDREI` → `65 78 68 82 69 73`

- **Decodificare ASCII**
  - `66 82 65 86 79` → **„BRAVO”**

## 5.

- **Codificarea unui nume în Base64**
  - Exemplu: `ANDREI` → `QU5EUkVJ`

- **Decodificare Base64**
  - `U3VudCBzdHVkZW50IGxhIEZNSS4=` → **„Sunt student la FMI.”**

- [Online Converter](https://www.rapidtables.com/convert/number/ascii-hex-bin-dec-converter.html)

## 6.

- **Malware**: Software rău intenționat utilizat pentru a compromite un sistem.
- **Virus**: Program care se atașează unui fișier și se răspândește atunci când fișierul este executat.
- **Dropper**: Program utilizat pentru a introduce un alt malware într-un sistem.
- **Downloader**: Software care descarcă și instalează malware suplimentar.
- **Trojan**: Program care pare legitim, dar conține cod malițios.
- **Spyware**: Malware care colectează informații fără consimțământ.
- **Riskware**: Software care poate fi exploatat în scopuri malițioase.
- **Ransomware**: Malware care blochează accesul la date și cere o răscumpărare.
- **Adware**: Software care afișează reclame nedorite.
- **Worm**: Malware care se răspândește independent în rețea.
- **Obfuscare**: Proces de ascundere a codului pentru a împiedica detecția.



# Securitatea Sistemelor Informatice - Laborator 2

## 1.

- **(D) Confidențialitate**: (1) Asigurarea că informațiile nu sunt dezvăluite entităților neautorizate.
- **(B) Criptografie**: (2) Disciplina care studiază principiile, mijloacele și metodele de transformare a datelor pentru a ascunde conținutul lor semantic, a preveni utilizarea lor neautorizată sau a preveni modificarea lor nedetectată.
- **(F) Disponibilitate**: (3) Asigurarea accesului și utilizării informațiilor în timp util și fiabil.
- **(A) Criptologie**: (4) Știința care se ocupă de criptanaliză și criptografie.
- **(C) Criptanaliză**: (5) Încercarea de a înfrânge protecția criptografică fără o cunoaștere inițială a cheii utilizate în furnizarea protecției.
- **(E) Integritate**: (6) Protejarea împotriva modificării sau distrugerii necorespunzătoare a informațiilor.

## 2.

1. **Salariile angajaților nu trebuie făcute publice.** → Confidențialitate
2. **Biroul casierie trebuie să aibă acces la salariile angajaților (pentru a realiza plățile).** → Disponibilitate
3. **Un angajat nu își poate modifica singur suma primită ca salariu pe luna în curs.** → Integritate
4. **Un angajat nu ar trebui să afle cât câștigă un coleg fără acordul acestuia.** → Confidențialitate
5. **Biroul casierie trebuie să aibă certitudinea că suma pe care o înmânează angajatului de plată este cea corectă.** → Integritate

Exemple de primitive criptografice:
- **Confidențialitate** → Algoritmi de criptare simetrică (AES, ChaCha20)
- **Integritate** → Funcții hash (SHA-256, SHA-3)
- **Disponibilitate** → Protocoale de redundanță și failover (RAID, servere redundante)

## 3.

1. Un adversar care are la dispoziție un timp infinit pentru criptanaliza unui sistem este un adversar PPT -- **Fals** – Un adversar PPT are timp polinomial, nu infinit.
2. Un adversar PPT are dreptul de a „ghici” cheia -- **Adevărat** – Un adversar PPT poate încerca să ghicească cheia, dar într-un timp polinomial.
3. Un adversar PPT are la dispoziție algoritmi exponențiali în timp -- **Fals** – Un adversar PPT nu are algoritmi exponențiali în timp.

## 4.

1. **𝑓(𝑛) = 2** → Ne-neglijabilă (constantă, nu tinde la zero)
2. **𝑓(𝑛) = 1/2000** → Ne-neglijabilă (constantă, nu depinde de 𝑛)
3. **𝑓(𝑛) = 1/𝑛!** → Neglijabilă (tinde foarte rapid spre zero)
4. **𝑓(𝑛) = 1/2ⁿ** → Neglijabilă (scade exponențial cu creșterea lui 𝑛)
5. **𝑓(𝑛) = 𝑓₁(𝑛) + 𝑓₂(𝑛), unde 𝑓₁(𝑛) și 𝑓₂(𝑛) sunt neglijabile** → Neglijabilă
6. **𝑓(𝑛) = 𝑓₁(𝑛) + 𝑓₂(𝑛), unde 𝑓₁(𝑛) este neglijabilă și 𝑓₂(𝑛) este ne-neglijabilă** → Ne-neglijabilă

## 5.

**Argumente pentru utilizarea securității computaționale:**
- Securitatea perfectă necesită chei mai mari decât mesajele transmise (ex. One-Time Pad), ceea ce nu este practic.
- Securitatea computațională oferă protecție rezonabilă împotriva adversarilor care au resurse limitate.
- Având în vedere puterea de calcul actuală, un sistem poate fi considerat sigur dacă un atac necesită mai mult timp decât durata de viață a datelor protejate.

## 6.

Se consideră un sistem criptografic cu cheie de 512 biți.

- **Numărul total de chei posibile:**
  \[ 2^{512} \]

- **Timpul necesar pentru a testa toate cheile cu un calculator care testează \( 2^{50} \) chei/secundă:**
  2^512 / 2^50 = 2^462 secunde

- **Eficiența atacului:**
  - Chiar și cu cel mai rapid calculator posibil, acest atac nu este fezabil. Timpul necesar pentru a testa toate cheile depășește durata de viață a universului.



# Securitatea Sistemelor Informatice - Laborator 3

# OTP

## 1.

Mesajul criptat este furnizat în format Base64, iar cheia în hex. Pentru a-l decripta, trebuie să:
1. Decodăm mesajul din Base64.
2. Convertim cheia din hex la bytes.
3. Aplicăm XOR între textul criptat și cheie.

Cod Python pentru decriptare:
```python
import base64

cipher_text_base64 = "o9/khC3Pf3/9CyNCbdzHPy5oorccEawZSFt3mgCicRnihDSM8Obhlp3vviAVuBbiOtCSz6husBWqhfF0Q/8EZ+6iI9KygD3hAfFgnzyv9w=="
key_hex = "ecb181a479a6121add5b42264db9b44b4b48d7d93c62c56a3c3e1aba64c7517a90ed44f8919484b6ed8acc4670db62c249b9f5bada4ed474c9e4d111308b614788cd4fbdc1e949c1629e12fa5fdbd9"

cipher_text = base64.b64decode(cipher_text_base64)
key = bytes.fromhex(key_hex)

plain_text = bytes([c ^ k for c, k in zip(cipher_text, key)])
print(plain_text.decode(errors='ignore'))
```
Mesajul obținut:
```
One Time Pad este un sistem de criptare perfect sigur daca este folosit corect.
```

## 2. 
```python
new_plain_text = "Orice text clar poate obtinut dintr-un text criptat cu OTP dar cu alta cheie.".encode()
new_key = bytes([c ^ p for c, p in zip(cipher_text, new_plain_text)])
print(new_key.hex())
```
Noua cheie: `ecad8de748ef0b1a857f032101bdb51f5e07c3c37931c37b3c3219ef748215708cf046a18588c1e2f897ca0076ca7f924eb1e6efcb1b905afed5d110228d24049b8242bec6e11d82699409fa12`

## 3.
Refolosirea cheii în OTP compromite securitatea. Dacă două mesaje sunt criptate cu aceeași cheie, putem deduce informații aplicând XOR între ele.

# Sisteme de criptare istorice

## 1.
Sistem ales: Cifrul lui Cezar.
- Exemplu:
  - Cheie: 3
  - Text clar: `HELLO`
  - Text criptat: `KHOOR`
  - Mod de funcționare: deplasăm literele circular din alfabet cu k (cheia) poziții.
- Securitate: slabă, vulnerabilă la analiza frecvenței.
- Criptanaliză: analiză de frecvență, brute-force (doar 25 de chei posibile).

## 2. 
Sistem ales: Transpoziția coloanelor.
- Exemplu:
  - Text clar: `HELLO WORLD`
  - Rearanjare: `HLOOLELWRD`
- Securitate: mai puternică decât substituția, dar vulnerabilă la analiză statistică.
- Criptanaliză: permutare brută, recunoaștere de modele.

# Analiza de frecvență

Cod Python:
```python
from collections import Counter

encrypted_text = "ENHFJ EWK LML EOJ GDJ BMONKC PMCG YEPMAC FOVQGMROEQDHF FMAQNJ. CHWFJ GDJHO HWUJWGHMW HW 1978, GDJV DEUJ EG MWFJ LJJW FENNJK HWCJQEOELNJ, EWK DEUJ LJJW GDJ CALXJFG MY WAPJOMAC KHUMOFJC, GOEUJNC, EWK GMOPJWGC. HW GDJ JWCAHWR VJEOC, MGDJO FDEOEFGJOC DEUJ XMHWJK GDJHO FOVQGMROEQDHF YEPHNV. GDJOJC JUJ, GDJ QECCHUJ EWK CALPHCCHUJ JEUJCKOMQQJO, PENNMOV GDJ PENHFHMAC EGGEFTJO, EWK GOJWG, GOACGJK LV ENN, XACG GM WEPJ E YJB. BDHNJ ENHFJ, LML, EWK GDJHO JSGJWKJK YEPHNV BJOJ MOHRHWENNV ACJK GM JSQNEHW DMB QALNHF TJV FOVQGMROEQDV BMOTC, GDJV DEUJ CHWFJ LJFMPJ BHKJNV ACJK EFOMCC MGDJO CFHJWFJ EWK JWRHWJJOHWR KMPEHWC. GDJHO HWYNAJWFJ FMWGHWAJC GM ROMB MAGCHKJ MY EFEKJPHE EC BJNN: ENHFJ EWK LML EOJ WMB E QEOG MY RJJT NMOJ, EWK CALXJFG GM WEOOEGHUJC EWK UHCAEN KJQHFGHMWC GDEG FMPLHWJ QJKERMRV BHGD HW-XMTJC, MYGJW OJYNJFGHWR MY GDJ CJSHCG EWK DJGJOMWMOPEGHUJ JWUHOMWPJWGC HW BDHFD GDJV BJOJ LMOW EWK FMWGHWAJ GM LJ ACJK. PMOJ GDEW XACG GDJ BMONKC PMCG YEPMAC FOVQGMROEQDHF FMAQNJ, ENHFJ EWK LML DEUJ LJFMPJ EW EOFDJGVQJ MY KHRHGEN JSFDEWRJ, EWK E NJWC GDOMARD BDHFD GM UHJB LOMEKJO KHRHGEN FANGAOJ. I.KAQMWG EWK E.FEGGEQEW FOVQGMFMAQNJ"

letter_counts = Counter(encrypted_text.replace(" ", ""))
print(letter_counts.most_common())
```

- Frecvența literelor: 
```
[('J', 122), ('E', 79), ('G', 71), ('W', 66), ('M', 66), ('H', 62), ('O', 56), ('C', 48), ('F', 45), ('D', 41), ('K', 37), ('N', 36), ('A', 28), ('Q', 24), ('L', 22), ('P', 20), ('V', 19), ('R', 17), ('U', 17), (',', 17), ('B', 16), ('Y', 13), ('.', 9), ('X', 6), ('T', 5), ('S', 4), ('1', 1), ('9', 1), ('7', 1), ('8', 1), (':', 1), ('-', 1), ('I', 1)]
```

- Textul obținut: [online tool](https://www.quipqiup.com)
```
	ALICE AND BOB ARE THE WORLDS MOST FAMOUS CRYPTOGRAPHIC COUPLE. SINCE THEIR INVENTION IN 1978, THEY HAVE AT ONCE BEEN CALLED INSEPARABLE, AND HAVE BEEN THE SUBJECT OF NUMEROUS DIVORCES, TRAVELS, AND TORMENTS. IN THE ENSUING YEARS, OTHER CHARACTERS HAVE JOINED THEIR CRYPTOGRAPHIC FAMILY. THERES EVE, THE PASSIVE AND SUBMISSIVE EAVESDROPPER, MALLORY THE MALICIOUS ATTACKER, AND TRENT, TRUSTED BY ALL, JUST TO NAME A FEW. WHILE ALICE, BOB, AND THEIR EXTENDED FAMILY WERE ORIGINALLY USED TO EXPLAIN HOW PUBLIC KEY CRYPTOGRAPHY WORKS, THEY HAVE SINCE BECOME WIDELY USED ACROSS OTHER SCIENCE AND ENGINEERING DOMAINS. THEIR INFLUENCE CONTINUES TO GROW OUTSIDE OF ACADEMIA AS WELL: ALICE AND BOB ARE NOW A PART OF GEEK LORE, AND SUBJECT TO NARRATIVES AND VISUAL DEPICTIONS THAT COMBINE PEDAGOGY WITH IN-JOKES, OFTEN REFLECTING OF THE SEXIST AND HETERONORMATIVE ENVIRONMENTS IN WHICH THEY WERE BORN AND CONTINUE TO BE USED. MORE THAN JUST THE WORLDS MOST FAMOUS CRYPTOGRAPHIC COUPLE, ALICE AND BOB HAVE BECOME AN ARCHETYPE OF DIGITAL EXCHANGE, AND A LENS THROUGH WHICH TO VIEW BROADER DIGITAL CULTURE. Q.DUPONT AND A.CATTAPAN CRYPTOCOUPLE
```

# Securitatea Sistemelor Informatice - Laborator 7

## 1. Noțiuni introductive

- **a)** Adevărat
- **b)** Fals
- **c)** Adevărat
- **d)** Fals
- **e)** Fals
- **f)** Fals
- **g)** Fals


## 3. Stocarea parolelor

- **Exemplul 1:**  
  Parolele sunt stocate în text clar, ceea ce prezintă un risc major în cazul unei breșe de securitate.

- **Exemplul 2:**  
  Parolele sunt hash-uite, dar nu folosesc un salt unic pentru fiecare utilizator, ceea ce face hash-urile vulnerabile la atacuri de tip rainbow table.

- **Exemplul 3:**  
  Se folosește o funcție hash rapidă (MD5 sau SHA-1), care este vulnerabilă la atacuri brute-force datorită vitezei mari de calcul.

- **Exemplul 4:**  
  Parolele sunt hash-uite și folosesc săruri, dar sarea este identică pentru toți utilizatorii, ceea ce reduce semnificativ protecția.

- **Exemplul 5:**  
  Parolele sunt hash-uite cu o funcție adaptivă (bcrypt) și sarea este unică pentru fiecare utilizator. Aceasta este considerată o bună practică în securizarea parolelor.
