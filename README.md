<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600;800;900&family=Rajdhani:wght@500;600;700&family=Inter:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">

<style>
  :root {
    --accent-purple: #a855f7;
    --accent-glow: #c084fc;
    --dark-bg: #090d16;
    --dark-card: #131722;
    --text-primary: #f8fafc;
    --text-muted: #94a3b8;
    --border-color: #2e3748;
  }

  body, .markdown-body {
    background-color: var(--dark-bg) !important;
    color: var(--text-primary) !important;
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif !important;
    line-height: 1.65;
  }

  /* Encabezados Neón / Dark */
  h1, h2, h3, h4, h5, h6 {
    font-family: 'Rajdhani', 'Orbitron', sans-serif !important;
    letter-spacing: 1.5px;
    text-transform: uppercase;
    color: var(--text-primary) !important;
    font-weight: 700;
  }

  h1 {
    font-family: 'Orbitron', sans-serif !important;
    color: #ffffff !important;
    border-bottom: 2px solid var(--accent-purple) !important;
    padding-bottom: 12px;
    margin-top: 24px;
    text-shadow: 0 0 10px rgba(168, 85, 247, 0.4);
  }

  h2 {
    color: #ffffff !important;
    border-left: 4px solid var(--accent-purple) !important;
    padding-left: 12px;
    margin-top: 36px;
    border-bottom: 1px solid var(--border-color);
    padding-bottom: 6px;
    text-shadow: 0 0 8px rgba(168, 85, 247, 0.3);
  }

  h3 {
    color: #e2e8f0 !important;
    margin-top: 26px;
  }

  h4 {
    color: #cbd5e1 !important;
    margin-top: 18px;
  }

  /* Enlaces */
  a {
    color: var(--accent-purple) !important;
    text-decoration: none !important;
    font-weight: 600;
  }

  a:hover {
    color: var(--accent-glow) !important;
    text-decoration: underline !important;
  }

  /* Navegación */
  .disco-nav-container {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin: 20px 0 35px 0;
    padding: 16px;
    background: var(--dark-card);
    border: 1px solid var(--border-color);
    border-radius: 12px;
  }

  .disco-nav-pill {
    display: inline-block;
    padding: 8px 16px;
    background: #090d16;
    border: 1px solid var(--accent-purple);
    border-radius: 24px;
    color: #ffffff !important;
    font-family: 'Rajdhani', sans-serif;
    font-size: 0.95rem;
    font-weight: 600;
    letter-spacing: 0.5px;
    text-transform: uppercase;
    transition: all 0.25s ease;
  }

  .disco-nav-pill:hover {
    background: var(--accent-purple) !important;
    color: #ffffff !important;
    box-shadow: 0 0 12px rgba(168, 85, 247, 0.6);
    transform: translateY(-2px);
  }

  /* Banner Principal */
  .eklipse-hero {
    text-align: center;
    padding: 40px 20px;
    margin-bottom: 30px;
    background: var(--dark-card);
    border: 1px solid var(--accent-purple);
    border-radius: 16px;
    box-shadow: 0 0 20px rgba(168, 85, 247, 0.2);
  }

  .eklipse-hero h1 {
    font-size: 2.8rem;
    margin: 0;
    padding: 0;
    border: none !important;
    letter-spacing: 4px;
    color: #ffffff !important;
    text-shadow: 0 0 15px rgba(168, 85, 247, 0.6);
  }

  .eklipse-tagline {
    font-family: 'Rajdhani', sans-serif;
    font-size: 1.25rem;
    color: #cbd5e1;
    text-transform: uppercase;
    letter-spacing: 2px;
    margin-top: 8px;
    font-weight: 600;
  }

  .badge-neon {
    display: inline-block;
    padding: 4px 12px;
    background: #1e293b;
    border: 1px solid var(--accent-purple);
    color: #ffffff;
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
    background-color: var(--dark-card) !important;
    border: 1px solid var(--border-color) !important;
    border-radius: 10px !important;
    overflow: hidden !important;
  }

  th {
    background: #1e293b !important;
    color: #ffffff !important;
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
    color: #e2e8f0 !important;
  }

  tr:nth-child(even) td {
    background-color: #181f2e !important;
  }

  /* Bloques de Código */
  code, pre {
    font-family: 'JetBrains Mono', Consolas, monospace !important;
  }

  code:not(pre code) {
    background: #1e293b !important;
    color: #a855f7 !important;
    border: 1px solid var(--border-color) !important;
    padding: 2px 7px !important;
    border-radius: 4px !important;
    font-size: 0.9em;
  }

  pre {
    background: #131722 !important;
    border: 1px solid var(--border-color) !important;
    border-left: 4px solid var(--accent-purple) !important;
    border-radius: 8px !important;
    padding: 16px !important;
    color: #f1f5f9 !important;
  }

  /* Citas */
  blockquote {
    background: #131722 !important;
    border-left: 4px solid var(--accent-purple) !important;
    border-radius: 0 8px 8px 0;
    color: #cbd5e1 !important;
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
    <span class="badge-neon">🟣 Purple Accent & Dark Theme</span>
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
