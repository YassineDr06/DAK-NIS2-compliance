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
> In elke stap verwijs ik naar de bijbehorende screenshot **[SS#](#ss#)**.  

### 1) Intake, scope & aanpak (Projectstart) – zie [SS1](#ss1)
- Kick-off met opdrachtgever: scope, doel, context (NIS2 voor financiële sector), hoofdvraag en deelvragen afgestemd  
- Onderzoeksaanpak: literatuur, documentanalyse (SCIENTA), technische evaluaties en PoC-afbakening  

### 2) Bronnen verzamelen & huidige situatie – zie [SS2](#ss2)
- Geanalyseerd: SCIENTA, pentest-/auditrapporten, Microsoft-licenties, leveranciersoverzicht  
- Doel: nulmeting t.o.v. NIS2 artikel 21 (beleid, toegangsbeheer, logging, leveranciers, awareness)  

### 3) NIS2-kader & mapping – zie [SS3](#ss3)
- Koppeling NIS2-eisen aan DAK-domeinen (toegangsbeheer, logging/SIEM, BCP, leveranciers, governance)    

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

### 7) Proof of Concept – zie [SS9](#ss9), [SS10](#ss10)
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

### 9) Implementatieplan (5 stappen) – zie [SS11](#ss11)
1. **Prioriteren**: MFA, sessiebeheer, SIEM, encryptie, awareness  
2. **Techniek**: 1Password/Entra ID, Sentinel + EventLog Explorer, BitLocker, Windows FW/GlassWire  
3. **Organisatie**: IRP/BCP actualiseren, leveranciersbeheer structureren, awareness intensiveren  
4. **Monitoring & audits**: Compliance Manager, Power BI, jaarlijkse pentests  
5. **Documentatie & rapportage**: SharePoint, Power Automate, risicoregister up-to-date  

### 10) Trainingsplan & change management – zie [SS12](#ss12), [SS13](#ss13)
- 6-weeks programma (kick-off, e-learning+toets, phishing-simulatie, tool-workshop, datalek-workshop, eindtoets)  
- Borging: pre/post-toets, logboek, jaarlijkse herhaling, rapportage  

### 11) Kosten-baten & KPI’s – zie [SS14](#ss14), [SS15](#ss15)
- Investeringen: PoC-omgeving/tooling, implementatie top-5, awarenessprogramma, consultancy  
- Baten: lagere incident-impact, lagere datalek-kans, betere audit/compliance-scores, sneller MT-inzicht  

### 12) Eindadvies & governance – zie [SS16](#ss16)
- Dichten van kritieke technische gaten (MFA, SIEM, sessiebeheer, encryptie)  
- Formele borging via audits/rapportages en ketenbewaking (leveranciers)  

---

## Screenshots

### <a id="ss1"></a>SS1 – Project hoofdvraag en deelvragen
![SS1 – Projectscope en deelvragen](https://i.imgur.com/Im3HEq6.png)

### <a id="ss2"></a>SS2 – Inleiding deelvraag 2
![SS2 – Overzicht gebruikte bronnen/SCIENTA](https://i.imgur.com/wFF2Snu.png)

### <a id="ss3"></a>SS3 – Conclusie deelvraag 2
![SS3 – NIS2→Domeinen mapping](https://i.imgur.com/GYJfMOy.png)

### <a id="ss4"></a>SS4 – Beoordelingsschaal gap-analyse
![SS4 – GAP-analyse per NIS2-domein](https://i.imgur.com/p9MrIHh.png)

### <a id="ss5"></a>SS5 – Gap-analyse onderbouwing (CMDB/back-up)
![SS5 – Onderbouwing: CMDB/back-up bevindingen](https://i.imgur.com/vncRdKH.png)

### <a id="ss6"></a>SS6 – Risicomatrix en top-risico’s
![SS6 – Risicomatrix en top-risico’s](https://i.imgur.com/51IJnSA.png)

### <a id="ss7"></a>SS7 – Risicoregister (excerpt)
![SS7 – Risicoregister (excerpt)](https://i.imgur.com/VneVcw8.png)

### <a id="ss8"></a>SS8 – Productselectie (10 tools)
![SS8 – Evaluatiematrix (10 tools)](https://i.imgur.com/MHsOFfY.png)

### <a id="ss9"></a>SS9 – Voorbeeld geteste tools
![SS9 – DeelVoorbeeld geteste tools](https://i.imgur.com/7wVGO7M.png)

### <a id="ss10"></a>SS10 – Deel POC
![SS10 – Sentinel dashboards & incidents](https://i.imgur.com/3mmXfke.png)

### <a id="ss11"></a>SS11 – Implementatieplan
![SS11 – EventLog Explorer: detectie & filtering](https://i.imgur.com/nPdzzMz.png)

### <a id="ss12"></a>SS12 – Trainingsplan
![SS12 – Sophos Central: XDR-detecties/rapportage](https://i.imgur.com/td0mCnK.png)

### <a id="ss13"></a>SS13 – Deel change management
![SS13 – SecurityScorecard: leveranciersscore](https://i.imgur.com/J3QhQH8.png)

### <a id="ss14"></a>SS14 – Kostenanalyse
![SS14 – Aanbevolen toolketen (Top-5 Stack)](https://i.imgur.com/UrZNs2H.png)

### <a id="ss15"></a>SS15 – SMART batenanalyse
![SS15 – Roadmap/Gantt (5-stappenplan)](https://i.imgur.com/2UkB7gw.png)

### <a id="ss16"></a>SS16 – Eindconclusie
![SS16 – Trainingsplanning (6 weken)](https://i.imgur.com/u8FcQew.png)
