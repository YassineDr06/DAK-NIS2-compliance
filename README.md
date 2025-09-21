# Project DAK – NIS2 Compliance Advies

## Objective
Het DAK-project richtte zich op het onderzoeken in hoeverre DAK Intermediairscollectief voldoet aan de aankomende **NIS2-wetgeving**, en welke aanvullende maatregelen nodig zijn om volledig compliant te worden.  
Het doel was om door middel van **gap-analyses, risicoanalyses en Proof of Concept-tests** concrete aanbevelingen te doen voor het verhogen van de digitale weerbaarheid van DAK.

## Skills Learned
- Toepassen van **NIS2-richtlijn** op een reële organisatie in de financiële sector  
- Uitvoeren van **gap-analyses** en **risicoanalyses** in een bedrijfscontext  
- Praktische ervaring met **Proof of Concept** testen van security tools  
- Opstellen van een **implementatieplan** met prioritering van maatregelen  
- Ontwikkelen van **security awareness- en trainingsplannen**  
- Samenwerken in een multidisciplinair team en vertalen van onderzoek naar **adviesrapport**  

## Tools Used
- **Microsoft Sentinel** – SIEM voor centrale loganalyse en monitoring  
- **Eye Security MXDR** – Managed Detection & Response, 24/7 monitoring  
- **Sophos Intercept X Advanced with XDR** – endpointbescherming en respons  
- **SecurityScorecard** – leveranciersbeheer en risicobeoordeling  
- **EventLog Explorer** – loganalyse en auditing  
- **1Password Business** – wachtwoordbeheer en MFA-integratie  
- **Microsoft 365 & Azure-licenties** – o.a. Defender for Endpoint, Entra ID, Power Automate  

---

## Steps
> In elke stap verwijs ik naar de bijbehorende screenshot **[SS#]**. De screenshots voeg je onderaan toe bij **Screenshots**.

### 1) Intake, scope & aanpak (Projectstart) – zie [SS1](#ss1)
- Kick-off met opdrachtgever: scope, doel, context (NIS2 voor financiële sector) en deelvragen afgestemd  
- Onderzoeksaanpak: literatuur, documentanalyse (SCIENTA), technische evaluaties en PoC-afbakening  

### 2) Bronnen verzamelen & huidige situatie – zie [SS2](#ss2)
- Geanalyseerd: SCIENTA, pentest-/auditrapporten, Microsoft-licenties, leveranciersoverzicht  
- Doel: nulmeting t.o.v. NIS2 artikel 21 (beleid, toegangsbeheer, logging, leveranciers, awareness)  

### 3) NIS2-kader & mapping – zie [SS3](#ss3)
- Koppeling NIS2-eisen aan DAK-domeinen (toegangsbeheer, logging/SIEM, BCP, leveranciers, governance)  
- Output: mapping-tabel gebruikt als basis voor GAP-analyse  

### 4) GAP-analyse (huidig vs. gewenst) – zie [SS4](#ss4), [SS5](#ss5)
- Sterke basis (Eye Security + Microsoft), maar o.a.:  
  - Back-up/hersteltests deels verouderd  
  - CMDB/informatiearchitectuur niet overal up-to-date  
  - MFA/sessiebeheer niet overal geborgd  
  - Continue leveranciersbeoordeling ontbreekt  

### 5) Risicoanalyse & prioritering – zie [SS6](#ss6), [SS7](#ss7)
- Toprisico’s: ontbrekende (universele) MFA, zwak sessiebeheer, geen centraal SIEM  
- Risicomatrix bepaalt volgorde en quick wins  

### 6) Productselectie & criteria – zie [SS8](#ss8)
- 10 tools geëvalueerd op **Security, Usability, Maintenance, Cost**  
- Teamverdeling per tool en domein  

### 7) Proof of Concept – zie [SS9](#ss9), [SS10](#ss10), [SS11](#ss11), [SS12](#ss12), [SS13](#ss13)
- **Sentinel**: dataconnectors, analytics rules, dashboards, basistests  
- **EventLog Explorer**: Windows event logs, filtering/archivering  
- **SecurityScorecard**: leveranciers/attack surface inzicht  
- **Sophos Intercept X**: XDR, isolatie, rapportages  

### 8) Top-5 aanbevolen stack – zie [SS14](#ss14)
- SIEM/Monitoring: **Microsoft Sentinel**  
- Endpoint/XDR: **Sophos Intercept X Advanced with XDR**  
- Loganalyse/Audit: **EventLog Explorer**  
- Toegangsbeheer/MFA: **1Password Business + Entra ID P1**  
- Leveranciersbeheer: **SecurityScorecard**  

### 9) Implementatieplan (5 stappen) – zie [SS15](#ss15)
1. **Prioriteren**: MFA, sessiebeheer, SIEM, encryptie, awareness  
2. **Techniek**: 1Password/Entra ID, Sentinel + EventLog Explorer, BitLocker, Windows FW/GlassWire  
3. **Organisatie**: IRP/BCP actualiseren, leveranciersbeheer structureren, awareness intensiveren  
4. **Monitoring & audits**: Compliance Manager, Power BI, jaarlijkse pentests  
5. **Documentatie & rapportage**: SharePoint, Power Automate, risicoregister up-to-date  

### 10) Trainingsplan & change management – zie [SS16](#ss16), [SS17](#ss17)
- 6-weeks programma (kick-off, e-learning+toets, phishing-simulatie, tool-workshop, datalek-workshop, eindtoets)  
- Borging: pre/post-toets, logboek, jaarlijkse herhaling, rapportage  

### 11) Kosten-baten & KPI’s – zie [SS18](#ss18), [SS19](#ss19)
- Investeringen: PoC-omgeving/tooling, implementatie top-5, awarenessprogramma, consultancy  
- Baten: lagere incident-impact, lagere datalek-kans, betere audit/compliance-scores, sneller MT-inzicht  

### 12) Eindadvies & governance – zie [SS20](#ss20)
- Dichten van kritieke technische gaten (MFA, SIEM, sessiebeheer, encryptie)  
- Formele borging via audits/rapportages en ketenbewaking (leveranciers)  

---

## Screenshots
> Vervang `imgsrc` door je echte pad/URL. Laat de titels intact, dan blijven de interne links werken.

### <a id="ss1"></a>SS1 – Projectscope en deelvragen
![SS1 – Projectscope en deelvragen](imgsrc)

### <a id="ss2"></a>SS2 – Overzicht gebruikte bronnen/SCIENTA
![SS2 – Overzicht gebruikte bronnen/SCIENTA](imgsrc)

### <a id="ss3"></a>SS3 – NIS2→Domeinen mapping
![SS3 – NIS2→Domeinen mapping](imgsrc)

### <a id="ss4"></a>SS4 – GAP-analyse per NIS2-domein
![SS4 – GAP-analyse per NIS2-domein](imgsrc)

### <a id="ss5"></a>SS5 – Onderbouwing: CMDB/back-up bevindingen
![SS5 – Onderbouwing: CMDB/back-up bevindingen](imgsrc)

### <a id="ss6"></a>SS6 – Risicomatrix en top-risico’s
![SS6 – Risicomatrix en top-risico’s](imgsrc)

### <a id="ss7"></a>SS7 – Risicoregister (excerpt)
![SS7 – Risicoregister (excerpt)](imgsrc)

### <a id="ss8"></a>SS8 – Evaluatiematrix (10 tools)
![SS8 – Evaluatiematrix (10 tools)](imgsrc)

### <a id="ss9"></a>SS9 – Sentinel: Data connectors & Analytics rules
![SS9 – Sentinel: Data connectors & Analytics rules](imgsrc)

### <a id="ss10"></a>SS10 – Sentinel dashboards & incidents
![SS10 – Sentinel dashboards & incidents](imgsrc)

### <a id="ss11"></a>SS11 – EventLog Explorer: detectie & filtering
![SS11 – EventLog Explorer: detectie & filtering](imgsrc)

### <a id="ss12"></a>SS12 – Sophos Central: XDR-detecties/rapportage
![SS12 – Sophos Central: XDR-detecties/rapportage](imgsrc)

### <a id="ss13"></a>SS13 – SecurityScorecard: leveranciersscore
![SS13 – SecurityScorecard: leveranciersscore](imgsrc)

### <a id="ss14"></a>SS14 – Aanbevolen toolketen (Top-5 Stack)
![SS14 – Aanbevolen toolketen (Top-5 Stack)](imgsrc)

### <a id="ss15"></a>SS15 – Roadmap/Gantt (5-stappenplan)
![SS15 – Roadmap/Gantt (5-stappenplan)](imgsrc)

### <a id="ss16"></a>SS16 – Trainingsplanning (6 weken)
![SS16 – Trainingsplanning (6 weken)](imgsrc)

### <a id="ss17"></a>SS17 – Borging: pre/post-toets & KPI’s
![SS17 – Borging: pre/post-toets & KPI’s](imgsrc)

### <a id="ss18"></a>SS18 – Kostenanalyse (tabel)
![SS18 – Kostenanalyse (tabel)](imgsrc)

### <a id="ss19"></a>SS19 – SMART baten & KPI’s
![SS19 – SMART baten & KPI’s](imgsrc)

### <a id="ss20"></a>SS20 – Eindadvies & verantwoordelijkheden
![SS20 – Eindadvies & verantwoordelijkheden](imgsrc)
