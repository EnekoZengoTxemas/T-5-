# Eklipse – Webgunea eta GLPI dokumentazioa

## 1. Helburua

Eklipse diskotekarentzat bi tresna konfiguratu dira: bezeroarentzako webgune bat (WordPress) eta barne-erabilerarako IT kudeaketa sistema bat (GLPI). Dokumentu honek bakoitzaren egitura eta konfigurazio nagusia biltzen ditu.

**[1. IRUDIA]** Hemen jarri aurkezpeneko lehen diapositiba (WordPress eta GLPI ordenagailu-pantailetan, aldamenekoz aldamen).

## 2. Laburpena

|              | WordPress                    | GLPI                    |
|--------------|------------------------------|-------------------------|
| Erabilera    | Eklipse-ren webgune publikoa | IT zerbitzuen kudeaketa |
| Helbidea     | Eklipse.eus                  | glpi.eklipse.eus        |
| Editorea     | Kubio                        | GLPI panela             |
| Letra-tipoak | CSS bidez aldatuak           | Lehenetsiak             |

## 3. WordPress webgunea

### 3.1 Edukia eta orriak

Webgunea 5 orrik osatzen dute, eta Hasiera orria da erakusleiho nagusia: Eklipse logoa, aurkezpen-testu labur bat eta bi ekintza-botoi («Egin bazkide» eta «Kontaktatu gureki»).

| Orria                       |
|-----------------------------|
| Hasiera                     |
| Hardware Analisia           |
| Kontingentzia Plana Hacking |
| Jasangarritasun Plana       |
| Adibide-orria               |

### 3.2 Pluginak

![image1.png](media/image1.png)

Webgunean 7 plugin daude instalatuta. Garrantzitsuenak Kubio (orrien editorea) eta All-in-One WP Migration (webgunearen kopia eta migrazioak egiteko) dira.

**[3. IRUDIA]** Hemen jarri WordPress-eko alboko menuaren pantaila-argazkia (Plugins, Kubio, All-in-One WP Migration... ikusten direnekoa).

### 3.3 Letra-tipoen pertsonalizazioa

Webgunearen estiloa aldatzeko, Kubio-ren «CSS gehigarria» atalean kode hau gehitu da:

- **Izenburuak (h1–h6):** Rajdhani letra-tipoa, letra larriz eta 1,5 px-ko tartearekin; itxura futurista ematen dio.

- **Gainerako testua:** Inter letra-tipoa, irakurgarritasun hobea lortzeko.

- Biak Google Fonts-etik kargatzen dira.

## 4. GLPI

![image2.png](media/image2.png)

### 4.1 Erabiltzaileak

Sisteman 9 erabiltzaile sortu dira, denak aktiboak: eneko, glpi, glpi-system, jakes, joan, normal, post-only, tech eta xabier. Erabiltzaile batzuek rol zehatza dute (adibidez, «tech» teknikariarentzat eta «post-only» mezuak bidaltzeko soilik).

### 4.2 Segurtasun-oharrak

![image3.png](media/image3.png)

GLPI-ren hasierako panelak hiru abisu erakusten ditu. Konponbide gisa hauek egitea gomendatzen da:

1.  Erabiltzaile lehenetsien pasahitzak aldatu.

2.  install/install.php fitxategia ezabatu.

3.  PHP-n session.cookie_httponly aukera aktibatu.

## 5. Hurrengo urratsak

![image4.png](media/image4.png)

- Jasangarritasun Plana amaitu eta argitaratu.

- WordPress-eko eta pluginen eguneraketa pendienteak aplikatu.

- GLPI-ko hiru segurtasun-abisuak zuzendu.
