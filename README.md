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
<img width="503" height="665" alt="Schermafbeelding 2025-09-21 195347" src="https://github.com/user-attachments/assets/4b8eedc1-1abb-4ed7-acb4-a0843e951d02" />


### <a id="ss2"></a>SS2 – Inleiding deelvraag 2
<img width="607" height="286" alt="Schermafbeelding 2025-09-22 202415" src="https://github.com/user-attachments/assets/529fb119-27ab-4b96-a861-7233517bab7f" />


### <a id="ss3"></a>SS3 – Conclusie deelvraag 2
<img width="1200" height="889" alt="Schermafbeelding 2025-09-22 202941" src="https://github.com/user-attachments/assets/a19c76bf-868e-4a12-8d19-e0520535ec94" />


### <a id="ss4"></a>SS4 – Beoordelingsschaal gap-analyse
<img width="1160" height="1086" alt="Schermafbeelding 2025-09-22 203258" src="https://github.com/user-attachments/assets/d2966f91-406f-45b8-ba95-cbe51cc15e19" />


### <a id="ss5"></a>SS5 – Gap-analyse onderbouwing (CMDB/back-up)
<img width="628" height="626" alt="Schermafbeelding 2025-09-22 211205" src="https://github.com/user-attachments/assets/99b19d1a-8d9c-4042-8d00-0edd49de1f7a" />


### <a id="ss6"></a>SS6 – Risicomatrix en top-risico’s
<img width="911" height="805" alt="Schermafbeelding 2025-09-22 203735" src="https://github.com/user-attachments/assets/81aa91ba-42a4-443c-be16-ba662e2d969a" />


### <a id="ss7"></a>SS7 – Risicoregister (excerpt)
<img width="916" height="730" alt="Schermafbeelding 2025-09-22 203723" src="https://github.com/user-attachments/assets/93617bdf-e182-45c7-b0d5-12529784ee2b" />


### <a id="ss8"></a>SS8 – Productselectie (10 tools)
<img width="905" height="946" alt="Schermafbeelding 2025-09-22 204200" src="https://github.com/user-attachments/assets/cef48f0f-0743-469e-8775-549075de8529" />


### <a id="ss9"></a>SS9 – Voorbeeld geteste tools
<img width="645" height="1039" alt="Schermafbeelding 2025-09-22 204933" src="https://github.com/user-attachments/assets/a28385b3-f89b-45da-98f3-b4a8fd7f7200" />


### <a id="ss10"></a>SS10 – Inleiding POC
<img width="630" height="432" alt="Schermafbeelding 2025-09-22 205804" src="https://github.com/user-attachments/assets/cdcc2005-ea06-46f0-a166-eb9e9c212f47" />


### <a id="ss11"></a>SS11 – Implementatieplan
<img width="628" height="773" alt="Schermafbeelding 2025-09-22 210152" src="https://github.com/user-attachments/assets/d14c9156-0f15-4848-86c4-e7e728f6f53b" />


### <a id="ss12"></a>SS12 – Trainingsplan
<img width="616" height="985" alt="Schermafbeelding 2025-09-22 210312" src="https://github.com/user-attachments/assets/364d507b-b769-4f26-a562-9c69d9e0b587" />

### <a id="ss13"></a>SS13 – Deel change management
<img width="615" height="708" alt="Schermafbeelding 2025-09-22 210425" src="https://github.com/user-attachments/assets/6266e55b-7421-4a60-aafc-d0270f772c21" />


### <a id="ss14"></a>SS14 – Kostenanalyse
<img width="618" height="625" alt="Schermafbeelding 2025-09-22 210604" src="https://github.com/user-attachments/assets/da268d88-1365-4bc0-8ec1-9e3fedad7ef9" />


### <a id="ss15"></a>SS15 – SMART batenanalyse
<img width="630" height="966" alt="Schermafbeelding 2025-09-22 210617" src="https://github.com/user-attachments/assets/2b739cfa-3f17-44a6-9b04-8a3ae31f3e6c" />


### <a id="ss16"></a>SS16 – Eindconclusie
<img width="641" height="294" alt="Schermafbeelding 2025-09-22 210819" src="https://github.com/user-attachments/assets/f09c30bc-b715-4d65-8484-6bda68b77445" />
