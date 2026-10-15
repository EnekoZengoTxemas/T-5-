<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600;800;900&family=Rajdhani:wght@500;600;700&family=Inter:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">

<style>
  :root {
    --accent-purple: #7c3aed;
    --light-bg: #000000;
    --light-card: #f8fafc;
    --text-primary: #000000;
    --text-muted: #475569;
    --border-color: #cbd5e1;
  }

  body, .markdown-body {
    background-color: var(--light-bg) !important;
    color: var(--text-primary) !important;
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif !important;
    line-height: 1.65;
  }

  /* Encabezados en texto negro plano sin resplandor */
  h1, h2, h3, h4, h5, h6 {
    font-family: 'Rajdhani', 'Orbitron', sans-serif !important;
    letter-spacing: 1.5px;
    text-transform: uppercase;
    color: #000000 !important;
    font-weight: 700;
    text-shadow: none !important;
  }

  h1 {
    font-family: 'Orbitron', sans-serif !important;
    color: #000000 !important;
    text-shadow: none !important;
    border-bottom: 2px solid var(--accent-purple) !important;
    padding-bottom: 12px;
    margin-top: 24px;
  }

  h2 {
    color: #000000 !important;
    border-left: 4px solid var(--accent-purple) !important;
    padding-left: 12px;
    text-shadow: none !important;
    margin-top: 36px;
    border-bottom: 1px solid var(--border-color);
    padding-bottom: 6px;
  }

  h3 {
    color: #000000 !important;
    margin-top: 26px;
  }

  h4 {
    color: #1e293b !important;
    margin-top: 18px;
  }

  /* Enlaces normales */
  a {
    color: var(--accent-purple) !important;
    text-decoration: none !important;
    font-weight: 600;
    text-shadow: none !important;
  }

  a:hover {
    color: #4c1d95 !important;
    text-decoration: underline !important;
    text-shadow: none !important;
  }

  /* Navegación */
  .disco-nav-container {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin: 20px 0 35px 0;
    padding: 16px;
    background: var(--light-card);
    border: 1px solid var(--border-color);
    border-radius: 12px;
  }

  .disco-nav-pill {
    display: inline-block;
    padding: 8px 16px;
    background: #000000;
    border: 1px solid var(--accent-purple);
    border-radius: 24px;
    color: #000000 !important;
    font-family: 'Rajdhani', sans-serif;
    font-size: 0.95rem;
    font-weight: 600;
    letter-spacing: 0.5px;
    text-transform: uppercase;
    transition: all 0.25s ease;
  }

  .disco-nav-pill:hover {
    background: var(--accent-purple) !important;
    color: #000000 !important;
    transform: translateY(-2px);
  }

  /* Banner Principal */
  .eklipse-hero {
    text-align: center;
    padding: 40px 20px;
    margin-bottom: 30px;
    background: var(--light-card);
    border: 1px solid var(--accent-purple);
    border-radius: 16px;
  }

  .eklipse-hero h1 {
    font-size: 2.8rem;
    margin: 0;
    padding: 0;
    border: none !important;
    letter-spacing: 4px;
    color: #000000 !important;
    text-shadow: none !important;
  }

  .eklipse-tagline {
    font-family: 'Rajdhani', sans-serif;
    font-size: 1.25rem;
    color: #334155;
    text-transform: uppercase;
    letter-spacing: 2px;
    margin-top: 8px;
    font-weight: 600;
  }

  .badge-neon {
    display: inline-block;
    padding: 4px 12px;
    background: #f1f5f9;
    border: 1px solid var(--accent-purple);
    color: #000000;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin: 4px;
  }

  /* Tablas */
  table {
    width: 100% !important;
    border-collapse: separate !important;
    border-spacing: 0 !important;
    margin: 20px 0 !important;
    background-color: #000000 !important;
    border: 1px solid var(--border-color) !important;
    border-radius: 10px !important;
    overflow: hidden !important;
  }

  th {
    background: #f1f5f9 !important;
    color: #000000 !important;
    font-family: 'Rajdhani', sans-serif !important;
    font-size: 1.05rem !important;
    letter-spacing: 1px !important;
    text-transform: uppercase !important;
    border-bottom: 2px solid var(--accent-purple) !important;
    padding: 12px 14px !important;
    text-align: left !important;
  }

  td {
    border-bottom: 1px solid var(--border-color) !important;
    padding: 11px 14px !important;
    color: #000000 !important;
  }

  tr:nth-child(even) td {
    background-color: #f8fafc !important;
  }

  /* Bloques de Código */
  code, pre {
    font-family: 'JetBrains Mono', Consolas, monospace !important;
  }

  code:not(pre code) {
    background: #f1f5f9 !important;
    color: #000000 !important;
    border: 1px solid var(--border-color) !important;
    padding: 2px 7px !important;
    border-radius: 4px !important;
    font-size: 0.9em;
  }

  pre {
    background: #f8fafc !important;
    border: 1px solid var(--border-color) !important;
    border-left: 4px solid var(--accent-purple) !important;
    border-radius: 8px !important;
    padding: 16px !important;
    color: #000000 !important;
  }

  /* Citas */
  blockquote {
    background: #f8fafc !important;
    border-left: 4px solid var(--accent-purple) !important;
    border-radius: 0 8px 8px 0;
    color: #1e293b !important;
    padding: 14px 20px !important;
    margin: 20px 0 !important;
  }

  hr {
    border: 0;
    height: 1px;
    background: var(--border-color);
    margin: 40px 0;
  }
</style>

<div class="eklipse-hero">
  <div style="font-size: 3rem; margin-bottom: 5px;">⚡ 🍸 🎶</div>
  <h1>EKLIPSE DISCO</h1>
  <div class="eklipse-tagline">Arkitektura Teknologikoa, pfSense Proxmox, Zibersegurtasuna eta Kudeaketa Osoa</div>
  <div style="margin-top: 15px;">
    <span class="badge-neon">🟣 Purple Accent & Light Mode</span>
    <span class="badge-neon">🛡️ pfSense 2.6.0 Proxmox VE</span>
    <span class="badge-neon">🌐 Eklipse.eus & GLPI</span>
    <span class="badge-neon">🌱 Euskadi 2030 Agenda</span>
  </div>
</div>

## 📌 Aurkibidea (Eduki-Taula)

<div class="disco-nav-container">
  <a class="disco-nav-pill" href="#1-datu-baseen-estrategia-eta-arkitektura---diskoteka">1. Arkitektura & IoT</a>
  <a class="disco-nav-pill" href="#2-datu-baseak">2. Datu-Baseak (SQL & Mongo)</a>
  <a class="disco-nav-pill" href="#3-ziber-eta-segurtasuna">3. Zibersegurtasuna & pfSense</a>
  <a class="disco-nav-pill" href="#4-eklipse-disco-aretoetarako-proposamen-tekniko-ekonomiko-eta-orokorra">4. Hardwarea & Aurrekontua</a>
  <a class="disco-nav-pill" href="#5-jasangarritasun-plana">5. Jasangarritasuna (GJH)</a>
  <a class="disco-nav-pill" href="#6-eklipse--webgunea-eta-glpi-dokumentazioa">6. Webgunea & GLPI Osoa</a>
</div>

1. [Datu-Baseen Estrategia eta Arkitektura — Diskoteka](#1-datu-baseen-estrategia-eta-arkitektura---diskoteka)
   - [1.1. Denbora Errealeko Sarrera (IoT eta Lokalaren Monitorizazioa)](#11-denbora-errealeko-sarrera-iot-eta-lokalaren-monitorizazioa)
   - [1.2. Harrera Zerbitzua eta Bezeroen Kudeaketa](#12-harrera-zerbitzua-eta-bezeroen-kudeaketa)
   - [1.3. Logistika eta Eragiketa Datuak (Stock-a eta Salmentak)](#13-logistika-eta-eragiketa-datuak-stock-a-eta-salmentak)
   - [1.4. Erresilientzia eta Erabilgarritasun Handia (HA)](#2-erresilientzia-erabilgarritasuna-eta-erabilgarritasun-handia-ha)
   - [1.5. Justifikazio Teknikoa eta Sistemaren Monitorizazioa](#3-justifikazio-teknikoa-eta-sistemaren-monitorizazioa)
2. [Datu Baseak](#2-datu-baseak)
   - [2.1. Eredu Zirkularra eta 3NF Egitura](#2-datu-baseak)
   - [2.2. Taulen Definizioa DDL (SQL)](#taulen-definizioa-ddl-sql)
   - [2.3. Diseinuaren Punturik Garrantzitsuenak](#diseinuaren-punturik-garrantzitsuenak)
   - [2.4. Erabiltzaile eta Portuen Justifikazioa](#erabiltzaile-eta-portuen-justifikazioa---zergatik)
   - [2.5. MongoDB Sentsoreak eta JSON Dokumentuak](#mongodb-instalazioa-eta-konfigurazioa-eklipse-proiektua)
3. [Ziber eta segurtasuna & pfSense Proxmox-en](#3-ziber-eta-segurtasuna)
   - [3.1. Informazio publikoa eta zerbitzuen eskaneoa (Nmap & Hydra)](#informazio-publikoaren-bilakaera)
   - [3.2. Agertoki bakoitzeko Erantzun-Planak (A–E)](#segurtasuna)
   - [3.3. Kontingentzia-Aurrekontuaren Estimazio Osoa](#3-kontingentzia-aurrekontuaren-estimazio-osoa)
   - [3.4. Pasahitzen Politika eta Segurtasun Fisikoa](#pasahitzen-politika)
   - [3.5. pfSense Proxmox VE-n: Instalazio eta Konfigurazio Gida Aurreratua](#pfsense-proxmox-en-instalazio-gida-laburra)
   - [3.6. Sarearen Topologia, DMZ eta Suebaki-Arauak](#sarearen-diseinua)
   - [3.7. Urruneko Sarbidea (OpenVPN) eta NIDS (Suricata)](#urruneko-sarbidea-vpn)
4. [EKLIPSE DISCO aretoetarako proposamen tekniko, ekonomiko eta orokorra](#4-eklipse-disco-aretoetarako-proposamen-tekniko-ekonomiko-eta-orokorra)
   - [4.1. Ekipamenduen Xehetasunak (Portatilak, Mini PCak, Mahaigainekoak)](#osagai-eta-gailuen-aurrekontu-xehatua)
   - [4.2. Aurrekontu Orokorra eta Finantza Laburpena (BEZ %21)](#aurrekontu-orokorra-eta-finantza-laburpena)
   - [4.3. Muntaia, ESD Lanabesak, PRL eta RAEE Birziklatzea](#muntaia-eta-konfiguraziorako-lanabesak)
5. [Jasangarritasun Plana (SDG Compass eta GJHak)](#5-jasangarritasun-plana)
   - [5.1. SDG Compass Metodologia eta ESG Zutabeak](#eklipse-ren-jasangarritasun-plana)
   - [5.2. Landutako GJHak (7, 8, 9, 12, 13 eta Euskadiko 18. GJHa)](#12-eklipsen-landuko-ditugun-garapen-jasangarrirako-helburuak-gjhak)
   - [5.3. Inpaktuen Matrizea eta Gobernantza](#13-gobernantza-ardatza-erantzukizuna-eta-gardentasuna)
6. [Eklipse – Webgunea eta GLPI Dokumentazioa (Osoa eta Eguneratua)](#6-eklipse--webgunea-eta-glpi-dokumentazioa)
   - [6.1. Helburua eta Tresnen Laburpena](#61-helburua)
   - [6.2. WordPress Webgunea (`eklipse.eus`)](#62-wordpress-webgunea)
     - [A. Erabilera eta CMS Hautaketa](#webgunearen-erabilera)
     - [B. Orriak eta Edukia](#edukia-eta-orriak)
     - [C. Ezarritako Parametroak eta Pluginak](#instalazioan-ezarritako-parametroak)
     - [D. Erabiltzaileak eta Rolak](#erabiltzaileen-egitura)
     - [E. Kubio Diseinua eta CSS Aldaketak](#web-orriaren-diseinua)
   - [6.3. GLPI IT Kudeaketa Sistema (`glpi.eklipse.eus`)](#63-glpi)
     - [A. Erabilera eta Parametroak](#glpi-erabilera)
     - [B. 9 Erabiltzaileak eta Baimen-Matrizea](#glpi-erabiltzaileen-zerrenda)
     - [C. Enpresako Ekipoak (Aktiboak) eta Tiketak](#enpresako-ekipoak)
     - [D. 3 Segurtasun-Oharrak eta Konponbideak](#glpi-segurtasun-oharrak)
   - [6.4. Hurrengo Urratsak](#64-hurrengo-urratsak)

---

## 1. Datu-Baseen Estrategia eta Arkitektura - Diskoteka

### 1. Datu Bilketa eta Sarrera

Proiektu/erronka honetan, informazioa biltzeko estrategia hibrido bat ezarri da, datuen izaera eta sorkuntza-abiaduraren arabera banatuta:

#### 1.1. Denbora Errealeko Sarrera (IoT eta Lokalaren Monitorizazioa)

Nahi diren neurriak etengabe jasotzen dira establezimendutik barrena dauden sentsore eta sistema banatuen bidez, segurtasuna, erosotasuna eta kudeaketa operatiboa optimizatzeko:

- **Ingurumen-sentsoreak:** Tenperatura eta hezetasun sentsoreak, aretoetako klimatizazioa uneko afororaren arabera erregulatzeko.
- **Alkohol kontsumoaren eta tabernaren telemetria:** Emari-neurgailuak eta banagailu adimendunak, zerbitzatutako alkohol bolumena eta portzentajea automatikoki zenbatze aldera.
- **Aforoaren eta soinu-mailaren kontrola:** Pertsonen sarrera-irteerak zenbatzeko sentsore optikoak eta soinu-maila (dezibelioak - dB) neurtzeko sentsoreak, araudia betetzen dela bermatzeko.
- **Energia-kontsumoa:** Argiztapen eta soinu ekipamenduen elektrizitate-gaitasuna denbora errealean monitorizatzea.

#### 1.2. Harrera Zerbitzua eta Bezeroen Kudeaketa

Sarreran edo erregistro komertzialean jasotzen diren datuak:

- **Sarrera orokorra:** Adina egiaztatzea eta esparrura sartzeen oinarrizko erregistroa.
- **Fidelizazio programa (Bazkideak):** Datu pertsonal aurreratuen erregistroa (izena, abizenak, posta elektronikoa, telefonoa, jaiotze-data), profilen kudeaketarako, sustapenetarako eta lehentasunezko sarbiderako.

#### 1.3. Logistika eta Eragiketa Datuak (Stock-a eta Salmentak)

Inbentarioaren eta merkataritza-transakzioen fluxua kontrolatzea:

- **Produktuen trazabilitatea:** Botilen irekieren erregistroa, eta barra-kodeen edo RFID irakurketak stock-a berritzerakoan.
- **Salmenta puntuak (TPV):** Tabernetan egindako salmentak, VIP mahaien erreserbak eta biltegi bakoitzean geratzen den stock-a denbora errealean.

### 2. Erresilientzia, Erabilgarritasuna eta Erabilgarritasun Handia (HA)

Ezintasun teknikoen edo hardware akatsen aurrean datu-baseak funtzionatzen jarraituko duela bermatzeko, Denbora Errealeko Replikazio Aktibo/Pasiboko eskema bat ezarri da:

| Osagaia | Rola Arkitekturan | Sinkronizazio Mekanismoa |
| :--- | :--- | :--- |
| **Nodul Nagusia (Primary/Master)** | Idazketak eta irakurketak jasotzen ditu denbora errealean. | Transakzio-logen etengabeko sinkronizazioa. |
| **Bigarren Mailako Nodulua (Secondary/Replica)** | Nagusiaren kopia berdina itxaronaldi aktiboan. Nagusiak huts eginez gero zerbitzua hartzen du. | Sinkronizazio sinkrono edo asinkronoa denbora errealean. |

- **Failover Estrategia (Akatsen aurreko tolerantzia):** Datu-base nagusiak huts eginez gero, sistemak automatikoki bigarren mailako nodulura aldatzen du zerbitzua, daturik galdu gabe eta salmenta zein sarbide prozesuak gelditu gabe.
- **Segurtasun-copien Politikak (Backup):** Eguneroko kopia automatiko metagarriak, lan-ordutegitik kanpo programatuta.

### 3. Justifikazio Teknikoa eta Sistemaren Monitorizazioa

#### 3.1. Datu-Base Motorren Aukeraketa

- **MySQL (Erlazionala / OLTP):** Osotasun zorrotza behar duten transakzio kritikoak egituratzeko (bazkideen datu pertsonalak, fakturazioa, TPV eta logistika inbentarioa).
- **MongoDB (NoSQL / Dokumentala / Denbora Seriakoak):** IoT sentsoreetatik datorren abiadura handiko fluxua jasotzeko (tenperatura, aforoa, dezibelioak), bere eskema malgutasunagatik.

#### 3.2. Egoera Egiaztatzea Terminal Bidez eta Konfigurazio Fitxategiak

Datu-baseen funtzionamendu egokia egiaztatzeko, log-ak aztertzeko eta klusterraren zein replikazioaren konfigurazioa berrikusteko, prozedura hauek erabiltzen dira komando-kontsolatik:

**MySQL Berrikuspena** (`/etc/mysql/mysql.conf.d/mysqld.cnf`):
```bash
sudo systemctl status mysql
tail -f /var/log/mysql/error.log

mysql -u admin -p
SHOW MASTER STATUS;
SHOW SLAVE STATUS\G
```

**MongoDB Berrikuspena** (`/etc/mongod.conf`):
```bash
sudo systemctl status mongod
tail -f /var/log/mongodb/mongod.log

mongosh
rs.status()
```

---

## 2. Datu Baseak

```
[Bazkideak] ───< [VIP Erreserbak] ───< [Sarrerak]
      │
[Produktuak / Inbentarioa] ──< [Salmenta Enpt.] ───< [Salmentak]
      │                                                     │
[Stock Mugimenduak]                                  [TPV Terminalak]
```

Datu-base hau **Hirugarren Forma Normalari (3NF)** jarraituz diseinatu dugu, diskotekaren eguneroko jarduera kaotikoan datuak ez bikoizteko, eragiketak azkartzeko eta informazioaren osotasuna bermatzeko. Aplikazioa lau modulu nagusitan banatu dugu:

- **→ Bazkideak** (`bazkideak`): Bezeroen datu pertsonalak segurtasunez eta bakarrean gordetzen ditu (NAN eta posta elektronikoa bikoiztu gabe), sarreren eta VIP erreserben moduluarekin erraz lotzeko.
- **→ Logistika eta BEZa** (`produktuak`, `bez_motak`, `stock_mugimenduak`): Inbentarioaren eta barretan banatutako alkoholaren trazabilitatea zehatz-mehatz mantentzen du.
- **→ Salmentak eta TPV** (`salmentak`, `salmenta_enptizioak`): Transakzio bakoitzaren burua eta xehetasunak bananduta daude. Erosketa unean prezioa eta BEZa 'argazki' gisa gordetzen dira.
- **→ Sarrerak eta VIP** (`ekitaldiak`, `sarrerak`, `vip_erreserbak`): Atean QR bidezko sarbide azkarra eta VIP mahaien erreserbak kudeatzen ditu.

### Taulen Definizioa DDL (SQL)

#### A. Bazkideak eta Fidelizazioa
```sql
CREATE TABLE bazkideak (
    bazkide_id INT AUTO_INCREMENT PRIMARY KEY,
    izena VARCHAR(100) NOT NULL,
    abizenak VARCHAR(100) NOT NULL,
    nan_dni VARCHAR(20) UNIQUE NOT NULL,
    helbide_elektronikoa VARCHAR(150) UNIQUE NOT NULL,
    telefono_zenbakia VARCHAR(20),
    jaiotze_data DATE NOT NULL,
    alta_data TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    aktibo BOOLEAN DEFAULT TRUE
);
```

#### B. Logistika eta Inbentarioa
```sql
CREATE TABLE bez_motak (
    bez_id INT AUTO_INCREMENT PRIMARY KEY,
    ehunekoa DECIMAL(5,2) NOT NULL,
    deskribapena VARCHAR(50)
);

CREATE TABLE produktuak (
    produktua_id INT AUTO_INCREMENT PRIMARY KEY,
    izena VARCHAR(100) NOT NULL,
    kategoria ENUM('Alkohola', 'Freskagarria', 'Janaria', 'Merchandising', 'Beste bat') NOT NULL,
    oinarrizko_prezioa DECIMAL(10,2) NOT NULL,
    bez_id INT NOT NULL,
    uneko_stocka INT DEFAULT 0,
    gutxieneko_stocka INT DEFAULT 10,
    FOREIGN KEY (bez_id) REFERENCES bez_motak(bez_id)
);

CREATE TABLE stock_mugimenduak (
    mugimendua_id INT AUTO_INCREMENT PRIMARY KEY,
    produktua_id INT NOT NULL,
    mota ENUM('Hornitzaile_Sarrera', 'Barra_Banaketa', 'Hondatzea_Haustura', 'Doitzea') NOT NULL,
    kantitatea INT NOT NULL,
    jatorri_kokapena VARCHAR(50),
    helburu_kokapena VARCHAR(50),
    data TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    FOREIGN KEY (produktua_id) REFERENCES produktuak(produktua_id)
);
```

#### C. Salmentak eta TPV
```sql
CREATE TABLE tpv_terminalak (
    tpv_id INT AUTO_INCREMENT PRIMARY KEY,
    barra_izena VARCHAR(50) NOT NULL,
    kokapena VARCHAR(50)
);

CREATE TABLE salmentak (
    salmenta_id INT AUTO_INCREMENT PRIMARY KEY,
    tpv_id INT NOT NULL,
    bazkide_id INT NULL,
    salmenta_data TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    oinarri_zergapea DECIMAL(10,2) NOT NULL,
    bez_totala DECIMAL(10,2) NOT NULL,
    prezio_totala DECIMAL(10,2) NOT NULL,
    ordainketa_mota ENUM('Eskudirutan', 'Txartela', 'Bizum', 'Mistoa') NOT NULL,
    FOREIGN KEY (tpv_id) REFERENCES tpv_terminalak(tpv_id),
    FOREIGN KEY (bazkide_id) REFERENCES bazkideak(bazkide_id)
);

CREATE TABLE salmenta_enptizioak (
    enptizio_id INT AUTO_INCREMENT PRIMARY KEY,
    salmenta_id INT NOT NULL,
    produktua_id INT NOT NULL,
    kantitatea INT NOT NULL,
    unitate_prezioa_oinarria DECIMAL(10,2) NOT NULL,
    bez_ehunekoa DECIMAL(5,2) NOT NULL,
    azpitotala DECIMAL(10,2) NOT NULL,
    FOREIGN KEY (salmenta_id) REFERENCES salmentak(salmenta_id),
    FOREIGN KEY (produktua_id) REFERENCES produktuak(produktua_id)
);
```

#### D. Sarrerak eta VIP Erreserbak
```sql
CREATE TABLE ekitaldiak (
    ekitaldi_id INT AUTO_INCREMENT PRIMARY KEY,
    izena VARCHAR(100) NOT NULL,
    ekitaldi_data DATETIME NOT NULL,
    edukiera_maximoa INT NOT NULL
);

CREATE TABLE vip_erreserbak (
    erreserba_id INT AUTO_INCREMENT PRIMARY KEY,
    ekitaldi_id INT NOT NULL,
    bazkide_id INT NULL,
    bezero_izena VARCHAR(100) NOT NULL,
    kontaktuko_telefonoa VARCHAR(20) NOT NULL,
    vip_eremua VARCHAR(20) NOT NULL,
    baimendutako_pertsonak INT NOT NULL,
    gutxieneko_kontsumoa DECIMAL(10,2) DEFAULT 0.00,
    erreserba_prezioa DECIMAL(10,2) NOT NULL,
    egoera ENUM('Zain', 'Baieztatua', 'Ezeztatua', 'Osatua') DEFAULT 'Zain',
    FOREIGN KEY (ekitaldi_id) REFERENCES ekitaldiak(ekitaldi_id),
    FOREIGN KEY (bazkide_id) REFERENCES bazkideak(bazkide_id)
);

CREATE TABLE sarrerak (
    sarrera_id INT AUTO_INCREMENT PRIMARY KEY,
    ekitaldi_id INT NOT NULL,
    salmenta_id INT NOT NULL,
    erreserba_id INT NULL,
    qr_kodea VARCHAR(255) UNIQUE NOT NULL,
    sarrera_mota ENUM('Arrunta', 'VIP', 'Aurretiarra', 'Zerrenda') NOT NULL,
    kontsumizioa_barne BOOLEAN DEFAULT TRUE,
    Sarrera_egoera ENUM('Erabili_gabea', 'Sartuta', 'Ezeztatua') DEFAULT 'Erabili_gabea',
    sarrera_data DATETIME NULL,
    FOREIGN KEY (ekitaldi_id) REFERENCES ekitaldiak(ekitaldi_id),
    FOREIGN KEY (salmenta_id) REFERENCES salmentak(salmenta_id),
    FOREIGN KEY (erreserba_id) REFERENCES vip_erreserbak(erreserba_id)
);
```

### Diseinuaren Punturik Garrantzitsuenak

- **BEZ eta Zerga Kontrola** (`bez_motak` / `salmentak`): Salmenta bakoitzean `oinarri_zergapea`, `bez_totala` eta `prezio_totala` bereizten dira kontabilitate garbia izateko.
- **Stockaren Mugimenduak** (`stock_mugimenduak`): Biltegi nagusitik tabernako barra desberdinetara pasatzen den stocka uneoro trazatzen du.
- **VIP Erreserbak eta Sarrerak** (`sarrerak` / `vip_erreserbak`): `qr_kodea` erabiliz sarbide azkarra eta VIP mahaien esleipen automatikoa bermatzen du.

### Erabiltzaile eta portuen justifikazioa - zergatik?

Datu-basearen segurtasuna eta kudeaketa egokia bermatzeko, zerbitzua atzitzeko portu zehatzak eta baimen desberdintasunak dituzten erabiltzaileak definituko dira.
- **3306 portua (MySQL/MariaDB):** Barne-sareko komunikazio fidagarrirako soilik.
- **443 portua (HTTPS):** Aplikazio-zerbitzariarekin edo TPV terminalekin REST API segurua ezartzeko.

Erabiltzaile-rolak:
- `admin_diskoteka`: Zerbitzuaren kudeatzaile nagusia, baimen osoekin (DDL/DML eta backupak).
- `tpv_langilea`: Terminaletako salmentak erregistratzeko baimen mugatuekin.
- `atezaina_sarrerak`: Sarreretako QRak egiaztatzeko eta egoera eguneratzeko baimen soilarekin.
- `kudeatzailea_logistika`: Biltegiak, stock-mugimenduak eta hornitzaileak kudeatzeko baimenekin.

### MongoDB Instalazioa eta Konfigurazioa: EKLIPSE Proiektua

Datuak tokian bertan gordetzeko:
- **MongoDB Community Server (v9.0.2):** Windows zerbitzari gisa konfiguratuta (`mongodb://localhost:27017`).
- **MongoDB Compass:** Datuen ikuskapen grafikorako.
- **Datu-basea:** `eklipse_sentsoreak` | **Bilduma:** `sentsoreak`

```json
[
  { "sentsorea": "Tenperatura", "balioa": 21.5, "unitatea": "ºC", "egoera": "normala", "data": "2026-10-13T13:45:00Z" },
  { "sentsorea": "Dezibelioak", "balioa": 58.4, "unitatea": "dB", "egoera": "normala", "data": "2026-10-13T13:45:00Z" },
  { "sentsorea": "Alkoholimetro Sentsorea", "balioa": 0.0, "unitatea": "mg/L", "egoera": "seguroa", "data": "2026-10-13T13:45:00Z" }
]
```

![MongoDB Compass - eklipse_sentsoreak bilduma](assets/datu-baseak-mongodb-compass.png)

---

## 3. Ziber eta segurtasuna

### Informazio publikoaren bilakaera

Windows Serverraren egiaztapen orokor bat egin da IP mapa bat osatzeko.

### Zerbitzu edo aplikazio aktiboen eskaneoa

Kali Linux bidez egindako Nmap eskaneoan ikusi dugu zerbitzu aktiboak zabalik daudela eta OS detekzioak Windows Server 2019 adierazten duela.

![Nmap zerbitzu-eskaneoa eta OS detekzioa](assets/ziber-nmap-servicios.png)

### Ahultasun edo hedapen bilaketa

TCP portu irekiak eta ahultasunak aztertu dira. Hydra bidez saiatu arren, brute-force erasoa geldotuta geratu da sarbide-politika zorrotzengatik.

![Nmap vuln script - ahultasun bilaketa](assets/ziber-nmap-vuln.png)

![Hydra bidezko brute-force saiakera](assets/ziber-hydra-bruteforce.png)

### Ahultasun ustiaketa

> [!WARNING]
> Zerbitzuetan ez sartzeko eta arriskuak minimizatzeko: login saiakera mugak ezarriko dira, sare-mapa publikotik ezkutatuko da eta pfSense bidezko isolamendua ezarriko da.

### Segurtasuna

#### 1. Agertoki bakoitzeko erantzun-plan zehatzak

| Agertokia | Arrazoia / Abiarazlea | 1. Urratsa: Berehalako erreakzioa (0–15 s) | 2. Urratsa: Kontrola eta arintzea (1–5 min) | 3. Urratsa: Berrabiaraztea eta normalizazioa | Arduradun zuzena |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **A. Konektibitate edo sare-akatsa** | Latentzia > 2.000 ms, pakete-galera > % 15 edo zuntz optikoaren erorketa. | Tokiko bukle grafiko erreaktibora aldatze automatikoa. DJak musikaren erritmoa igotzen du. | Sarearen komutazioa ordezko 5G bideratzailera (routerra). Bigarren mailako ISParekin diagnostikoa. | Seinalea berriro konektatzea latentzia < 100 ms denean eta tasa egonkorra denean. | AV Teknikaria / VJ |
| **B. Eduki zakarra edo legez kanpokoa** | Biluztasuna, istiluak, legez kanpoko kontsumoa kameraren aurrean. | "Larridura-botoia" sakatzea. 5 s-ko atzerapen-bufferrak beste hirira iristea eragozten du. | Kortina grafikoa proiektatzea ("Seinalea doitzen..."). Segurtasuna bertaratu. | Inplikatutakoak kanporatu. Emisioa berriro aktibatu egiaztatu ondoren. | VJ Operadorea / Segurtasuna |
| **C. Ikus-entzunezko hardware-akatsa** | LED pantaila/proiektorea itzaltzea edo AV eskalatzailea izoztea. | Bideo-irteera tokiko ohiko argiteria-sistemara bideratzea. | Ordezko ekipoa jartzea edo LED prozesadorea berrabiarazi. | Seinale grafikoa berriro lerrokatu eta tenperaturak egiaztatu. | Guardiako AV Teknikaria |
| **D. Urruneko eboluzioa edo larrialdia** | Urruneko pantailan izua/alarmak/sutea ikustea edo abisua jasotzea. | Pantailan berehala beltzera igaro eta kanpoko audioa guztiz moztu. | Tokiko saioarekin jarraitu argiteria eta DJ propioarekin lokala bakartuz. | Zuzendaritzarekin balorazioa egin saioa berriz aktibatu edo bertan behera uzteko. | Eragiketen Zuzendaria / DJ |
| **E. Zibererasoa edo seinalearen hackeoa** | Kanpoko seinalea txertatzea, ransomwarea edo DDoS erasoa. | Sareko kablea fisikoki deskonektatu eta offline seinalera pasatu. | SRT/RTMP kredentzialak aldatu eta VLAN seguru batean bakartu. | 2FA duen ordezko zerbitzari enkriptatura migratu. | IT Teknikaria / VJ Operadorea |

#### 2. Agertoki bakoitzari lotutako beharrezko baliabideen matrizea

| Baliabidea / Tresna | Mota | Zein agertokitan aplikatzen den | Funtzio espezifikoa |
| :--- | :--- | :--- | :--- |
| **Failover 5G duen Dual-WAN bideratzailea** | Sarea | A agertokia, E agertokia | Trafikoa 5G sarera igortzen du zuntzak huts eginez gero. |
| **Atzerapen-buffer prozesadorea + Larridura-botoia** | AV Hardwarea | B agertokia, E agertokia | Irudi desegokiak blokeatzen ditu 5 s-ko atzerapenarekin. |
| **Ordezko AV Ekipoak (Kamera / Kodetzailea)** | AV Hardwarea | C agertokia | Osagai elektroniko nagusiek huts eginez gero ordezkatze azkarra. |
| **Lineaz kanpoko edukien zerbitzaria (B Plana)** | Softwarea / PCa | A, B, C, D, E agertokiak | Bideo-bukleak lokalki sortzen ditu konexiorik gabe. |
| **Firewall industriala VPN / SRT enkriptatzearekin** | Zibersegurtasuna | E agertokia | Sarbide ez-baimenduak eta DDoS erasoak blokeatzen ditu. |
| **IP Dedikatuko Interkomunikadorea / Comlink** | Komunikazioak | D agertokia, E agertokia | Zuzendarien arteko ahots-kanal segurua mantentzen du. |
| **SAI / UPS Sistema (3 kVA)** | Energia | A, B, C, D, E agertokiak | AV/IT rack-a babesten du tentsio-jaitsieren aurrean. |
| **Kabinako AV / VJ Operadorea** | Pertsonala | A, B, C, D, E agertokiak | Komutazioak burutu eta berehalako erantzuna kudeatzen du. |
| **Kamera eremuko Segurtasun-agentea** | Pertsonala | B agertokia | Ikusleen portaera moderatu eta istiluak prebenitzen ditu. |
| **Guardiako IT Espezialista** | Pertsonala | A agertokia, C agertokia, E agertokia | Sare-arazoak, elektronika-akatsak eta intrusioak ebazten ditu. |

#### 3. Kontingentzia-aurrekontuaren estimazio osoa

| Kontzeptua | Kategoria | Deskribapen teknikoa | Estimatutako kostua (€) |
| :--- | :--- | :--- | :--- |
| **Dual-WAN bideratzailea + 5G Modulu Industriala** | CAPEX (Inbertsioa) | Trafikoaren konmutazio automatikoa < 1 s-tan egiten duen sare-sistema. | 1.200 - 1.800 € |
| **Atzerapen-buffer prozesadorea + Etengailua** | CAPEX (Inbertsioa) | HD/4K seinalearen atzerapenerako botoi fisikoa duen hardwarea. | 1.500 - 2.500 € |
| **Ordezko AV Hardwarea (Kamera + Kodetzailea)** | CAPEX (Inbertsioa) | Bigarren mailako HD kamera eta ordezkatze azkarrerako komutatzailea. | 800 - 1.500 € |
| **Zibersegurtasun Firewall-a + VPN/SRT Lizentzia** | CAPEX (Inbertsioa) | Zibererasoen aurkako babesa, IP iragazketa eta puntuz puntuko enkriptatzea. | 1.000 - 2.000 € |
| **3 kVA-ko SAI/UPS Sistema AV/IT Rack-erako** | CAPEX (Inbertsioa) | Saretarako, prozesamendurako eta bideorako energia-babesa. | 800 - 1.200 € |
| **Redundante den linea + SIM 5G M2M** | OPEX (Hilero) | IP finkodun ISP sekundario independentea + datu mugikor mugagabeak. | 180 - 300 € / hilabete |
| **AV/IT Guardiako teknikari espezializatua** | OPEX (Hilero) | Sare, hardware eta zibersegurtasun laguntzarako urruneko/aurrez aurreko estaldura. | 200 - 400 € / hilabete |

### Pasahitzen politika

Pasahitz guztiek gutxienez 12 karaktere, letra handi/txikiak, zenbakiak eta ikur bereziak dituzte:
- `M00nD4nc3r1_` *(Donostiako bezero Admin)*
- `M00nD4nc3r2#` *(Bilboko bezero Admin)*
- `5unW4tch3r0_` *(Kali Linux)*
- `V13wM4n4g3r#` *(Windows Server)*
- `S4f3lyL00k5_` *(Linux Server)*

### Sarbide fisikoen eta ingurumenaren politika

- **Ingurumen-baldintzak:** Zerbitzariak gela klimatizatu independente batean kokatuko dira, beti **goiko solairuan eta lurretik altxatuta**, uholde eta hezetasun arriskuak deuseztatzeko.
- **Sarbide fisikoa:** Gela teknikora sartzeko sarbide-teklatua eremu diskretuan jarriko da (argi zuzenik gabe), eta langile bakoitzak kredentzial indibidualak izango ditu sarbide-erregistro automatikoarekin.

---

### pfSense Proxmox-en: instalazio-gida laburra

pfSense 2.6.0 Proxmox VE-ren barruko makina birtual batean dabil, eta hiru sare-segmentu bereizten ditu: **WAN**, **LAN** eta **OPT1 (DMZ)**.

#### Sistemaren datuak
| Atala | Balioa |
| :--- | :--- |
| **Bertsioa** | pfSense 2.6.0 (amd64), FreeBSD 12.3 oinarrian |
| **Plataforma** | KVM guest, SeaBIOS, QEMU CPU |
| **Izena (Hostname)** | `pfSense.home.arpa` |
| **Laguntza** | Community Support |

#### Interfazeak
| Interfazea | Txartela | IP helbidea | Mota |
| :--- | :--- | :--- | :--- |
| **WAN** | `vtnet0` | `192.168.71.218/24` | DHCP |
| **LAN** | `vtnet1` | `192.168.0.254/24` | Estatikoa |
| **OPT1 (DMZ)** | `vtnet2` | `192.168.2.254/24` | Estatikoa |

#### Virtualizazioa Proxmox-en
pfSense Proxmox VE-ren barruko makina birtual gisa dabil. Birtualizazioari esker ekipo fisiko berririk ez da behar, sare birtualak segundotan sortzen dira eta snapshot eta babeskopiak egin daitezke aldaketa arriskutsuen aurretik.

| Ezaugarria | Balioa |
| :--- | :--- |
| **Proxmox ostalaria (IPa)** | `192.168.71.160` |
| **VM-aren izena eta ID-a** | `VM 100 - pfSense-Eklipse` |
| **CPU, RAM eta diskoa** | 2 vCPU kores, 2048 MB RAM, 16 GB VirtIO Disk |
| **Sare-txartelak (VirtIO)** | `net0` → WAN (`vtnet0`), `net1` → LAN (`vtnet1`), `net2` → OPT1 (`vtnet2`) |
| **Proxmox-eko zubiak** | `vmbr1` eta `vmbr2` Linux bridgeak |

#### Instalazio-urratsak
1. Proxmox-en pfSense 2.6.0-ren ISO-a igo (`local` → *ISO Images*).
2. VM bat sortu: SeaBIOS, QEMU CPU eta VirtIO motako hiru sare-txartel, bakoitza bere zubian.
3. VM-a abiarazi, instalatzailea jarraitu eta amaitzean ISO-a kendu.
4. Kontsolan:
   - `1) Assign Interfaces`: `vtnet0` WAN, `vtnet1` LAN eta `vtnet2` OPT1.
   - `2) Set interface(s) IP address`: WAN DHCP bidez; LAN eta OPT1 IP finkoekin.
5. LAN-eko ordenagailu batetik `https://192.168.0.254` ireki, admin gisa sartu, pasahitza aldatu eta wizard-a bete.
6. **Status → Dashboard** aztertu: bertsioa, plataforma eta interfazeak zuzen daudela egiaztatu.
7. Konfigurazio egokiarekin, Proxmox-en **snapshot bat egin** (itzulera-puntua).

#### Suebakiaren aukeraketa eta kokapena

| Aukera | Alde onak | Alde txarrak |
| :--- | :--- | :--- |
| **pfSense (Aukeratua)** | Doakoa, web interfaze grafikoa, stateful suebakia, NAT, VPN eta IDS pakete sendoak | FreeBSD-ren ezagutza pixka bat behar da arazoak konpontzeko |
| **OPNsense** | Antzekoa eta interfaze modernoagoa | Ez du abantaila nabarmenik pfSense-rekin alderatuta erronka honetarako |
| **iptables / ufw** | Oso arina, ez du VM berezirik behar | Komando-lerroa soilik, arauen kudeaketa eta VPN/IDS zailagoak |

> [!NOTE]
> **Kokapena:** VM-a WAN eta barne-sareen artean kokatuta dago, hiru interfazerekin. Horrela barne eta DMZ sareetako trafiko guztia suebakitik pasatzen da, eta ez dago saihesbiderik.

#### Sarearen diseinua

```
Internet / Router ─── WAN vtnet0 (192.168.71.218) ─── [ pfSense ] ─── LAN vtnet1 (192.168.0.254) ─── Barne Sarea
                                                            │
                                                            └─── OPT1/DMZ vtnet2 (192.168.2.254) ─── Zerbitzariak
```

| Zona | Sarea | pfSense IPa | Zerbitzuak | Zergatik |
| :--- | :--- | :--- | :--- | :--- |
| **WAN** | `192.168.71.0/24` | `192.168.71.218` (DHCP) | Irteera Internetera | Kanpoko sarearekiko muga |
| **LAN** | `192.168.0.0/24` | `192.168.0.254` | Erabiltzaileak, TPVak eta pfSense-ren administrazioa | Sare fidagarria, DMZ-tik isolatuta |
| **DMZ (OPT1)** | `192.168.2.0/24` | `192.168.2.254` | Streaming, Webgunea eta bideo-zerbitzariak | Kanpotik eskuragarri egongo diren zerbitzuak LAN-etik bereizteko |

*Oharra: OPT1 interfazeari DMZ izena jarri zaio (Interfaces → OPT1 → Description).*

#### Suebaki-arauak

PfSense-k lehenespenez WAN-ean sarrera guztia blokeatzen du, LAN-ean dena baimentzen du, eta OPT1-en ez du ezer baimentzen arau bat gehitu arte:

| Interfazea | Ekintza | Jatorria → Helmuga | Portua | Zergatik |
| :--- | :--- | :--- | :--- | :--- |
| **WAN** | Blokeatu | edozein → WAN | guztiak | Kanpotik baimendu gabeko sarrerarik ez (lehenetsia) |
| **WAN** | Baimendu (NAT) | edozein → DMZ zerbitzaria | 80, 443 | Web zerbitzu publikoa eta streaminga |
| **LAN** | Baimendu | LAN → edozein | guztiak | Barne erabiltzaileek Internetera eta DMZ-ra sartzeko |
| **LAN** | Baimendu | LAN → pfSense | 443 | WebGUI HTTPS bidez administratzeko |
| **DMZ** | Blokeatu | DMZ → LAN | guztiak | Erasoa DMZ-n gertatuz gero, barne sarea zorrozki babesteko |
| **DMZ** | Baimendu | DMZ → WAN | 53, 80, 443 | DNS eta eguneraketak soilik |

*Garrantzitsua: Blokeatzeko araua baimentzekoaren gainetik kokatzen da DMZ-ko arau-zerrendan.*

#### Urruneko sarbidea (VPN)

| Aukera | Alde onak | Alde txarrak |
| :--- | :--- | :--- |
| **OpenVPN (Aukeratua)** | Oso zabaldua, bezero-fitxategiak esportatzeko morroia, UDP/TCP | Zertxobait motelagoa CPU mugatuetan |
| **WireGuard** | Oso azkarra eta konfigurazio sinplea | Pakete gehigarri gisa instalatu behar da |
| **IPsec** | Estandarra, sare-sare konexioetarako ona | Konfigurazio konplexuagoa |

**OpenVPN Ezarpena:**
1. `System → Cert. Manager`: CA propioa eta zerbitzariaren ziurtagiria sortu.
2. `VPN → OpenVPN → Wizards`: Local User Access, UDP 1194 portua, tunel-sarea `10.0.8.0/24` eta tokiko sarea `192.168.0.0/24`.
3. `System → Package Manager`: `openvpn-client-export` instalatu eta bezero-konfigurazioa esportatu.
4. Router nagusian UDP 1194 portua pfSense-ren WAN IPra birbideratu da.

#### IDS eta HTTPS
- **IDS (Suricata):** `System → Package Manager` bidez instalatuta. WAN interfazean ETOpen arauak aktibatu dira Alert Mode moduan.
  - *Egiaztapen proba:* LAN-eko ekipo batetik `curl http://testmynids.org/uid/index.html` exekutatu eta alerta agertzen dela egiaztatu da.
- **HTTPS WebGUI:** pfSense-ren kudeaketa HTTPS bidez soilik gaituta dago (`System → Advanced → Admin Access`).
- **Segurtasun mantentzea:** Diagnostics bidez XML babeskopiak eta Proxmox mailako backup automatikoak programatuta daude.

---

## 4. EKLIPSE DISCO aretoetarako proposamen tekniko, ekonomiko eta orokorra

### Osagai eta Gailuen Aurrekontu Xehatua

#### 1. Harrera eta Lana Egiteko Potentzia Handiko Portatilak (2 Unitate)

| Osagaia / Gailua | Ezaugarri Teknikoak | Unitateko Prezioa (BEZ gabe) |
| :--- | :--- | :--- |
| **Portatil Potentea** | Intel Core i7-13700H / AMD Ryzen 7 7735HS, 32 GB DDR5 RAM, 1 TB SSD NVMe PCIe 4.0, NVIDIA RTX 4060 8GB, 15.6" IPS Full HD/QHD pantaila | 1.350,00 € |
| **Guztira Portatilak (2 Unitate):** | | **2.700,00 €** |

![Harrerako portatilak erabiltzen](assets/eklipse-harrera-portatilak.png)

#### 2. Pantaila Handiak eta Mini PC Kutsuak/Ezkutatzekoak (2 Unitate)

| Osagaia / Gailua | Ezaugarri Teknikoak | Unitateko Prezioa (BEZ gabe) |
| :--- | :--- | :--- |
| **Mini PC Trinkoa** | VESA euskarria duena, Intel Core i5-13400 / Ryzen 5 5600H, 16 GB DDR4, 512 GB SSD NVMe, Wi-Fi 6 + BT, HDMI 2.1 (4K 60Hz) | 480,00 € |
| **Pantaila Handia** | 65" edo 75" LED/4K UHD Babes-pantaila komertziala (24/7 erresistentzia), HDMI anitz | 850,00 € |
| **VESA Euskarria eta Kableak** | Hormako euskarri artikulatua eta HDMI 2.1 kableak | 60,00 € |
| **Guztira Mini PC + Pantaila Pack (2 Unitate):** | | **2.780,00 €** |

#### 3. Mahaigaineko PCak eta Periferikoak (12 Unitate)

| Osagaia / Gailua | Ezaugarri Teknikoak | Unitateko Prezioa (BEZ gabe) |
| :--- | :--- | :--- |
| **Prozesadorea (CPU)** | Intel Core i5-13400 / AMD Ryzen 5 5600G | 165,00 € |
| **Plaka Ama** | Chipset B760M / B550M babes elektrikoekin | 95,00 € |
| **RAM Memoria** | 16 GB DDR4 3200 MHz (2x8GB) | 45,00 € |
| **Biltegiratzea** | SSD NVMe M.2 500 GB PCIe | 45,00 € |
| **Elikadura Iturria** | 550W 80 Plus Bronze | 55,00 € |
| **Kaxa / Chasis** | Micro-ATX formatua, hauts-iragazki integratuekin | 50,00 € |
| **Monitorea** | 24" Full HD IPS 75Hz, altuera erregulagarria | 120,00 € |
| **Periferikoen Pack-a** | Teklatu eta sagu erresistenteak (USB) + Entzungailu mikrofonodunak | 40,00 € |
| **Subtotal Mahaigaineko PCak (12 Unitate):** | | **7.380,00 €** |

![Mahaigaineko PC pack-aren erabilera](assets/eklipse-mahaigaineko-pack.jpg)

### Aurrekontu Orokorra eta Finantza Laburpena

| Kategoria | Kontzeptua eta Azalpena | Subtotala (BEZ gabe) |
| :--- | :--- | :--- |
| **Portatil Potenteak** | 2x Harrerako eta lan grafiko arinetarako portatilak | 2.700,00 € |
| **Mini PC eta Pantaila Erraldoiak** | 2x Mini PC (VESA) + 2x 65"/75" Pantaila komertzialak + Euskarriak | 2.780,00 € |
| **Mahaigaineko PCak eta Periferikoak** | 12x Mahaigaineko PC osoak (Dorreak, Monitoreak, Teklatuak, Saguak, Entzungailuak) | 7.380,00 € |
| **Software Lizentziak** | 16x Windows 11 Pro / IoT lizentziak, ERP/TPV kudeaketa eta babes antivirusa | 1.450,00 € |
| **ESD Lanabesak eta Taller Materiala** | Tentsioaren aurkako eskulekuak, alfombrillak, kableatua, bridak eta tresneria | 220,00 € |
| **Lan-eskua eta Zerbitzuak** | 16 gailuen muntaia lantegian, sistemen instalazioa, kableatzea eta lokaleko konfigurazioa | 2.100,00 € |
| **Seinalizazioa eta PRL** | Segurtasun-seinalak, babes elektrikoak eta birziklatze-eremuen antolaketa | 150,00 € |
| **OINARRI IMPONIBLEA GUZTIRA:** | | **16.780,00 €** |
| **BEZ (%21):** | | **3.523,80 €** |
| **AURREKONTU OSOA GUZTIRA:** | | **20.303,80 €** |

### Muntaia eta Konfiguraziorako Lanabesak

Aparatuen muntaia lan-segurtasuneko eta deskarga elektrostatikoen (**ESD**) araudia jarraituz egingo da:
- **Tentsioaren aurkako eskulekua (Anti-ESD Pulsera):** Osagai elektroniko sentikorrak babesteko, lurra-hartunera lotuta.
- **Zehaztasunezko bihurkin magnetizatuak:** Zirkuituak ez kaltetzeko.
- **ESD Alfonbra Antiestatikoa:** Lan-azalera seguru eta eroalea.
- **Alkohol Isopropilikoa (99.9%) eta pasta termiko dielektrikoa:** Bero-transmisio optimorako.

![Muntaia lantegia eta lanabesak](assets/eklipse-muntaia-lanabesak.png)

![Birziklatze sistema eta hondakinen kudeaketa lantegian](assets/eklipse-birziklatze-sistema.jpg)

---

## 5. Jasangarritasun Plana

### Eklipse-ren Jasangarritasun Plana

Eklipse diskoteketan teknologia ingurumen- eta gizarte-erantzukizunez baliatzen dugu, **Euskadiko LH Basque Country 2030 Agenda** eta **SDG Compass** gidaren 5 urratsak aplikatuz:

| 1. URRATSA | 2. URRATSA | 3. URRATSA | 4. URRATSA | 5. URRATSA |
| :---: | :---: | :---: | :---: | :---: |
| 2030 Agenda ulertzea | Inpaktuak aztertzea | Helburuak eta KPIak ezartzea | Integrazioa eta Ekintzak | Txostena eta Komunikazioa |

### 1.0. Jasangarritasunaren kontzeptua eta nazioarteko esparruak

Jasangarritasuna egungo beharrak asetzea da etorkizuneko belaunaldien baliabideak arriskuan jarri gabe, hiru ardatzetan: **Ingurumena, Gizartea eta Gobernantza (ESG)**.
Oinarrizko esparruak:
- **2030 Agenda eta Garapen Jasangarrirako 17 Helburuak (NBE, 2015).**
- **Parisko Akordioa (2015):** Karbono-aztarnaren murrizketa.
- **Euskadiko LH Basque Country 2030 Agenda:** 18. GJH bereziarekin (hizkuntza eta kultura aniztasuna).
- **SDG Compass Gida:** Enpresa-estrategian GJHak txertatzeko ibilbide-orria.

### 1.2. Eklipsen Landuko Ditugun Garapen Jasangarrirako Helburuak (GJHak)

- 🟢 **7. GJHa (Energia eskuragarria eta ez-kutsatzailea):** IoT bidezko klimatizazio adimenduna aforoaren arabera eta LED argiztapen eraginkorra.
- 🟢 **8. GJHa (Lan duina eta hazkunde ekonomikoa):** PRL informatizatua, txanda orekatuak eta TPV bidezko lan-kargaren murrizketa.
- 🟢 **9. GJHa (Industria, berrikuntza eta azpiegitura):** Proxmox bidezko birtualizazio berdea eta telemetria adimenduna stock-galketak saihesteko.
- 🟢 **12. GJHa (Ekoizpen eta kontsumo arduratsua):** Ekodiseinua (RAM/SSD berrerabilpena), paperaren ezabapena (faktura digitalak) eta RAEE hondakinen kudeaketa profesionala.
- 🟢 **13. GJHa (Klimaren aldeko ekintza):** Zerbitzarien efizientzia energetikoa eta berotegi-efektuko gasen murrizketa.
- 🟢 **Euskadiko 18. GJHa (Hizkuntza eta Kultura Aniztasuna):** Webgunea, TPV interfazeak eta kudeaketa euskaraz bermatzea, LANEKI/JAKINBAI terminologiarekin bat eginez eta tokiko musika sustatuz.

### 1.3. Gobernantza-ardatza: erantzukizuna eta gardentasuna

- **Gardentasuna:** Urteko Jasangarritasun Txostena publikoa (`eklipse.eus/jasangarritasuna`) eta DBOL/RGPD auditoretzak.
- **Erosketa Arduratsua:** Eraginkortasun energetikoa egiaztatuta duten hardware-hornitzaileak lehenestea.
- **Portaera-kodea:** Langileentzako jazarpenaren aurkako protokoloa eta salaketa-kanal konfidentziala.

---

## 6. Eklipse – Webgunea eta GLPI Dokumentazioa

Dokumentazio atal honek Eklipse diskotekaren zerbitzu digital nagusiak biltzen ditu: kanpo-erabilerarako **WordPress webgunea** eta barne-kudeaketarako **GLPI zerbitzua**.

### 6.1. Helburua

- **WordPress Webgunea:** Bezeroentzako erakusleiho publikoa, diskotekaren nortasuna, ekitaldiak eta proiektuaren txostenak erakusteko.
- **GLPI IT Kudeaketa:** Ekipoen inbentario zehatza, baimendutako erabiltzaile-rolak eta intzidentzien tiketak bideratzeko sistema.

| Ezaugarria | WordPress | GLPI |
| :--- | :--- | :--- |
| **Erabilera** | Eklipse-ren webgune publikoa | IT zerbitzuen eta intzidentzien kudeaketa |
| **Helbidea** | `eklipse.eus` | `glpi.eklipse.eus` |
| **Editorea / Panela** | Kubio Builder | GLPI Kudeaketa Panela |
| **Letra-tipoak** | CSS gehigarria: Rajdhani & Inter | Lehenetsiak (Sistemakoak) |

![WordPress eta GLPI Aurkezpena](assets/WP.png)

---

### 6.2. WordPress Webgunea

#### Webgunearen erabilera
Webgunea Eklipse diskotekaren aurpegi publikoa da. Honako helburuak ditu:
1. Diskotekaren irudia eta aurkezpena erakustea (logoa, testu laburra eta bi ekintza-botoi: «Egin bazkide» eta «Kontaktatu gurekin»).
2. Erronkaren dokumentazioaren atal nagusiak argitaratzea: Hardware Analisia, Kontingentzia Plana Hacking eta Jasangarritasun Plana.

#### Zergatik WordPress: erabileraren eta CMS-aren arteko lotura

| Webguneak behar duena | WordPress-en funtzionalitatea |
| :--- | :--- |
| **Orri estatikoak** (hasiera, planak, analisiak) | Orriak (*Pages*) eta bloke-editorea |
| **Itxura zaindua kodea idatzi gabe** | Kubio editore bisual aurreratua |
| **Edukia jende ez-teknikoak aldatu ahal izatea** | Administrazio-panela eta erabiltzaile-rolak |
| **Segurtasun-kopiak eta migrazioak** | All-in-One WP Migration plugina |
| **Itxura korporatiboa pertsonalizatzea** | «CSS gehigarria» atala |

#### Edukia eta orriak

![WordPress-eko orrien zerrenda](assets/wp-orriak.png)

| Orria | Egoera | Funtzioa eta Deskribapena |
| :--- | :--- | :--- |
| **Hasiera** | Argitaratuta | Erakusleiho nagusia, branding-a eta ekintza-botoi deigarriak |
| **Hardware Analisia** | Argitaratuta | Diskotekako azpiegitura eta gailu teknikoen azalpena |
| **Kontingentzia Plana Hacking** | Argitaratuta | Zibersegurtasuneko protokoloak eta erantzun-neurriak |
| **Jasangarritasun Plana** | Argitaratuta | GJHak, Euskadi 2030 eta ingurumen konpromisoak |
| **Adibide-orria** | Argitaratuta | Diseinu probetarako orria |
| **Pribatutasun-politika** | Argitaratuta | RGPD eta bezeroen datu-babesaren lege-orria |

#### Instalazioan ezarritako parametroak

| Parametroa | Balioa |
| :--- | :--- |
| **WordPress bertsioa** | 6.6.x (azken bertsio egonkorra) |
| **Helbidea (URL)** | `eklipse.eus` |
| **Webgunearen izenburua** | EKLIPSE DISCO — Nightclub & Technology Hub |
| **Administratzaile-erabiltzailea** | `admin` |
| **Datu-basea** | `eklipse_wordpress` (MySQL / MariaDB 10.11) |
| **Web-zerbitzaria eta PHP** | Apache 2.4 + PHP 8.2 |
| **Taulen aurrizkia** | `wp_` |
| **Hizkuntza** | Euskara (lehenetsia) |

#### Pluginak
Webgunean 7 plugin instalatu dira zerbitzua eta segurtasuna optimizatzeko:

![WordPress Pluginak](assets/image1.png)

| Plugina | Funtzioa |
| :--- | :--- |
| **Kubio** | Orrien editore bisuala eta estilo-blokeak |
| **All-in-One WP Migration** | Webgunearen segurtasun-kopiak eta migrazio errazak |
| **Wordfence Security** | Firewall aplikatiboa eta brute-force babesa |
| **WPForms** | Harremanetarako formulario seguruak |
| **Yoast SEO** | Bilatzaileetarako posizionamendu optimizatua |
| **LiteSpeed Cache** | Kargatze-abiadura hobetzeko katxea |
| **WP Multilang / Polylang** | Euskara eta gaztelaniaren kudeaketa elebiduna |

#### Erabiltzaileen egitura

| Erabiltzailea | Rola | Zertarako sortu da | Zer egin dezake |
| :--- | :--- | :--- | :--- |
| `admin` | Administratzailea | Webgunearen administrazio osoa | Dena: pluginak, gaiak, erabiltzaileak, zerbitzariaren konfigurazioa |
| `editorea` | Editorea | Edukia argitaratu eta aldatzeko | Orriak sortu, editatu eta argitaratu; ez du plugin/erabiltzaile baimenik |
| `egilea` | Egilea | Bere artikuluak soilik idazteko | Ekitaldien berriak eta sustapenak idatzi eta argitaratu |

#### Web orriaren diseinua eta CSS aldaketak

Webgunearen diseinua diskotekaren giroarekin bat datorren **itxura iluna eta futuristarekin** egin da: irudi iluna eta argi koloretsuak, logoa erdian eta kontraste handiko testua.

**Hasiera orriaren egitura:**
1. **Goiburua:** Eklipse logoa eta nabigazio-menua (*Hasiera*, *Ekitaldiak*, *VIP*, *Dokumentazioa*).
2. **Erakusleihoa:** Atzeko irudi dinamikoa, «EKLIPSE» izenburua eta aurkezpen-testua.
3. **Ekintza-botoiak:** «Egin bazkide» eta «Kontaktatu gurekin» (neon estiloarekin nabarmenduta).

##### Letra-tipoen pertsonalizazioa (CSS gehigarria)
Diskotekaren estetika bermatzeko, Kubio-ren **«CSS gehigarria»** atalean kode hau txertatu da:

![Kubio-ren CSS gehigarria atala](assets/wp-kubio-css.png)

```css
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&family=Rajdhani:wght@600;700&display=swap');

/* Títulos con estilo electrónico/futurista */
h1, h2, h3, h4, h5, h6 {
    font-family: 'Rajdhani', sans-serif !important;
    text-transform: uppercase;
    letter-spacing: 1.5px;
}

/* Texto general */
body, p, a, button, input {
    font-family: 'Inter', sans-serif !important;
}
```

- **Izenburuak (`h1–h6`):** `Rajdhani` letra-tipoa, letra larriz eta 1,5 px-ko tartearekin; izaera elektroniko eta modernoa ematen dio.
- **Gainerako testua (`body, p, a, button, input`):** `Inter` letra-tipoa, irakurgarritasun garbia eskainiz gailu guztietan.

---

### 6.3. GLPI

#### GLPI Erabilera
GLPI barne-erabilerarako IT kudeaketa sistema aurreratua da. Eklipse diskotekan honetarako erabiltzen da:
- Diskotekako **ekipoak** (ordenagailuak, pantaila handiak, TPVak, inprimagailuak) inbentariatzeko.
- **Erabiltzaileak** eta haien baimenak kontrolatzeko.
- **Intzidentzien tiketak** erregistratu eta jarraipena egiteko.

Helbidea: `glpi.eklipse.eus`

#### Instalazioan ezarritako parametroak

| Parametroa | Balioa |
| :--- | :--- |
| **GLPI bertsioa** | 10.0.15 (LTS) |
| **Helbidea (URL)** | `glpi.eklipse.eus` |
| **Web-zerbitzaria eta PHP** | Apache 2.4, PHP 8.2 |
| **Datu-basea** | `eklipse_glpi` (MariaDB 10.11) |
| **SO / Zerbitzaria** | Debian 12 / Proxmox VM |
| **Hizkuntza** | Euskara / Gaztelania |
| **Administratzaile-kontua** | `glpi` (Super-Admin perfilarekin) |

#### Hasierako panela

![GLPI-ren hasierako panela](assets/glpi-panela.png)

Panelak hauek erakusten ditu: ekipo-motak (softwarea, ordenagailuak, monitoreak, inprimagailuak), hileko tiketen egoera eta segurtasun-abisuak.

#### GLPI Erabiltzaileen zerrenda

Sisteman **9 erabiltzaile** daude konfiguratuta, guztiak aktibo:

![GLPI-ko erabiltzaileen zerrenda](assets/glpi-erabiltzaileak.png)

| Erabiltzailea | Mota | Perfila (rola) | Zertarako / Funtzioa |
| :--- | :--- | :--- | :--- |
| `glpi` | Lehenetsia | Super-Admin | Administrazio eta konfigurazio osoa |
| `glpi-system` | Lehenetsia (sistema) | — | Sistemaren barne-zeregin automatikoak |
| `tech` | Lehenetsia | Technician | Intzidentzia teknikoak konpontzea |
| `normal` | Lehenetsia | Erabiltzaile arrunta | Tiketak sortu eta haien jarraipena egitea |
| `post-only` | Lehenetsia | Post-only | Mezuak/tiketak bidaltzeko soilik |
| `eneko` | Sortua | Super-Admin | Zuzendaritza teknikoa eta azpiegitura osoaren kontrola |
| `jakes` | Sortua | Technician | Sare-konexioak eta pfSense/VPN mantentzea |
| `joan` | Sortua | Technician | AV, pantaila handiak eta DJ kabinako euskarria |
| `xabier` | Sortua | Technician | TPVak, barrako inprimagailuak eta hardware mantentzea |

#### Enpresako ekipoak

GLPI-n erregistratutako Eklipse-ko azpiegitura teknikoa:

| Ekipoa | Mota | Kokapena | Egoera |
| :--- | :--- | :--- | :--- |
| `EKLIPSE-SRV-01` | Zerbitzaria (Proxmox VE) | Gela Teknikoa (Goiko solairua) | Martxan (Ekoizpena) |
| `EKLIPSE-FW-PFSENSE` | Suebaki Birtuala (VM 100) | Proxmox Ostalaria | Martxan (Aktiboa) |
| `PORTATIL-HARRERA-01/02` | Portatil Potenteak (i7 / RTX 4060) | Sarrera / Harrera Nagusia | Martxan |
| `MINIPC-DISP-01/02` | Mini PC Trinkoak + 65"/75" Pantailak | Areto Nagusia / VIP Eremua | Martxan |
| `PC-DESK-01..12` | 12x Mahaigaineko PCak | Barrak, Bulegoak eta Biltegia | Martxan |
| `TPV-PRINTER-01..06` | Tiket Inprimagailu Termikoak | Tabernetako Barrak | Martxan |

#### Tiketak

GLPI bidez erregistratutako intzidentzia arrunten fluxua:
- Tiketa: *«Barra 1eko TPV inprimagailuak ez du papera mozten»* → Esleitua: `xabier` → Egoera: Konponduta.
- Tiketa: *«VIP aretoko pantaila erraldoiaren seinalearen egiaztapena»* → Esleitua: `joan` → Egoera: Amaituta.

#### GLPI Segurtasun-oharrak

![GLPI Segurtasun Oharrak](assets/image3.png)

GLPI-ren hasierako panelak **hiru segurtasun-abisu** erakusten ditu, eta hurrengo ekintzekin zuzendu dira:

| # | Abisua | Arrazoia | Konponbidea |
| :---: | :--- | :--- | :--- |
| **1** | **Erabiltzaile lehenetsien pasahitzak aldatu** | `glpi`, `normal`, `post-only` eta `tech` kontuen gakoak publikoak dira | *Administrazioa → Erabiltzaileak* atalean pasahitz sendoak (12+ karaktere) ezarri dira |
| **2** | **`install/install.php` ezabatu** | Instalatzailea berriro exekutatzeko arriskua | `rm -f /var/www/html/glpi/install/install.php` komandoaren bidez fitxategia ezabatu da |
| **3** | **PHP-n `session.cookie_httponly` aktibatu** | XSS bidezko saio-lapurretak saihesteko | `/etc/php/8.2/apache2/php.ini` fitxategian `session.cookie_httponly = On` jarri eta zerbitzaria berrabiarazi da |

---

### 6.4. Hurrengo Urratsak

![GLPI eta Webgunearen Garapena](assets/image4.png)

- [x] **pfSense 2.6.0 Proxmox VE-n** instalatu, WAN/LAN/DMZ segmentatu eta OpenVPN zein Suricata konfiguratu.
- [x] **GLPI-ko 3 segurtasun-abisuak** zuzendu (pasahitzak aldatu, `install.php` kendu eta `session.cookie_httponly` aktibatu).
- [x] **WordPress eta Kubio diseinua** ezarri, Rajdhani eta Inter letra-tipoekin batera.
- [ ] **Jasangarritasun Plana** webgune publikoan behin betiko argitaratu (`eklipse.eus/jasangarritasuna`).
- [ ] Diskotekako **12 PC, 2 portatil eta 2 pantaila handien** inbentarioa eta agente automatikoak GLPI-rekin sinkronizatu.

---

<div style="text-align: center; padding: 25px 10px; color: var(--text-muted); font-size: 0.9rem;">
  <p>🍸 <strong>EKLIPSE DISCO PUB</strong> — Sistema Informatikoak, Sareak eta Zibersegurtasuna © 2026</p>
  <p style="color: var(--neon-purple); font-weight: 600;">Neon Purple & Dark Theme • Dokumentazio Osoa Eguneratua</p>
</div>
