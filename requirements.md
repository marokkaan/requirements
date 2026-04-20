# Business Intelligence Requirements – The Chocolate Firm

## Functional Requirements

---

### FR-01 – Integratie van databronnen
**Omschrijving**  
Als organisatie wil ik dat data automatisch kan worden opgehaald uit Odoo en externe bronnen (zoals marketing- en verkooptools), zodat alle bedrijfsdata centraal beschikbaar is voor analyse.

**Achtergrond**  
De organisatie gebruikt meerdere systemen zonder centrale koppeling. Dit leidt tot versnipperde data en inefficiënte besluitvorming.

**Prioriteit**  
Must have

**Uitwerking**
- Ondersteuning voor Odoo (ERP/CRM) als primaire databron  
- Mogelijkheid tot koppeling met externe verkoop- en marketingtools. 
- Automatische data-import zonder handmatige Excel-imports  

---

### FR-02 – Opzetten van datawarehouse
**Omschrijving**  
Als organisatie wil ik een centraal datawarehouse waarin alle bedrijfsdata wordt opgeslagen volgens een gestandaardiseerd datamodel, zodat er één bron van waarheid ontstaat.

**Achtergrond**  
Er is momenteel geen centrale opslagstructuur voor data.

**Prioriteit**  
Must have

**Uitwerking**
- Staginglaag + geïntegreerde datalaag  
- Historische opslag van data  
- Ondersteuning voor meerdere afdelingen en KPI-structuren  

---

### FR-03 – KPI-dashboard voor management
**Omschrijving**  
Als management wil ik interactieve dashboards met gestandaardiseerde KPI’s, zodat ik prestaties snel kan beoordelen.

**Achtergrond**  
Management heeft behoefte aan centrale stuurinformatie op basis van KPI’s. 

**Prioriteit**  
Must have

**Uitwerking**
- KPI’s zoals marge per product/klant, cashflow, voorraadwaarde, omzet per regio  
- Filters op tijd, klantsegment en productcategorie  
- Visualisaties (grafieken)  
- Consistente KPI-definities (single source of truth)  

---

### FR-04 – Rapportage op meerdere niveaus
**Omschrijving**  
Als BI-gebruiker wil ik rapportages kunnen bekijken op verschillende detailniveaus, zodat ik analyses kan uitvoeren op product, klant en regiosniveau. 

**Achtergrond**  
Verschillende afdelingen hebben behoefte aan verschillende niveaus van detail. 

**Prioriteit**  
Must have

**Uitwerking**
- Het systeem moet rapportages ondersteunen op productniveau, klantniveau en regioniveau. 

---

### FR-05 – Self-service BI functionaliteit
**Omschrijving**  
Als BI-gebruiker wil ik zelf rapportages kunnen maken zonder IT-ondersteuning, zodat ik snel inzichten kan verkrijgen. 

**Achtergrond**  
IT-capaciteit is beperkt en moet niet belast worden met standaard rapportages. 

**Prioriteit**  
Must have

**Uitwerking**
- Gebruikers moeten na een korte training (1–2 dagen) zelfstandig rapportages kunnen maken binnen het BI-systeem.  

---

### FR-06 – Rolgebaseerde toegangscontrole
**Omschrijving**  
Als IT-directeur wil ik dat gebruikers alleen toegang hebben tot data waarvoor zij geautoriseerd zijn, zodat vertrouwelijkheid en datasegmentatie gewaarborgd blijven. 

**Achtergrond**  
Gevoelige data moet beschermd blijven.

**Prioriteit**  
Must have

**Uitwerking**
- Het systeem moet zo gehete ‘role-based access control’ ondersteunen waarbij elke afdeling een eigen datasegment heeft, met daarnaast een centraal managementoverzicht. 

- Mogelijkheid tot management-overview met volledige toegang   

---

### FR-07 – Dagelijkse rapportage-updates
**Omschrijving**  
Als BI-gebruiker wil ik dat data automatisch dagelijks wordt vernieuwd, zodat dashboards altijd gebaseerd zijn op recente informatie. 

**Achtergrond**  
Realtime data is niet nodig, maar actuele daginformatie wel. 

**Prioriteit**  
Must have

**Uitwerking**
- Data refresh minimaal 1x per 24 uur  
- Geen handmatige acties  
- Melding maken bij mislukte data-updates

---

### FR-08 – KPI-configuratie
**Omschrijving**  
Als BI-gebruiker wil ik KPI’s kunnen beheren en aanpassen, zodat het systeem flexibel blijft bij veranderende bedrijfsdoelen.

**Achtergrond**  
KPI’s kunnen in de tijd veranderen afhankelijk van bedrijfsstrategie. 

**Prioriteit**  
Should have

**Uitwerking**
- Het systeem moet KPI’s configureerbaar maken binnen het BI-platform.
  
---

### FR-09 – Ondersteuning gebruikers
**Omschrijving**  
Als BI-gebruiker wil ik dat het systeem geschikt is voor meerdere gebruikers, zodat alle medewerkers met BI kunnen werken. 

**Achtergrond**  
Ongeveer 30–50 medewerkers zullen het systeem gebruiken. 

**Prioriteit**  
Must have

**Uitwerking**
- Het BI-systeem moet minimaal 50 gelijktijdige gebruikers ondersteunen.
  
---

## Non-Functional Requirements

---

### NFR-01 – Gebruiksvriendelijkheid en self-service 
**Omschrijving**  
Als medewerker wil ik eenvoudig met het BI-systeem kunnen werken, zodat ik zonder technische kennis rapportages kan maken.

**Achtergrond**  
IT-capaciteit is beperkt en eindgebruikers moeten zelfstandig kunnen werken. 

**Prioriteit**  
Must have

**Uitwerking**
- Intuïtieve interface  
- Trainingstijd maximaal 1–2 dagen  
- Self-service rapportagefunctionaliteit

---

### NFR-02 – Beperkte IT-belasting
**Omschrijving**  
Als IT-afdeling wil ik dat het BI-systeem weinig onderhoud vereist, zodat mijn werkdruk niet toeneemt. 

**Achtergrond**  
De IT-afdeling heeft beperkte capaciteit. 

**Prioriteit**  
Must have

**Uitwerking**
- Het systeem moet zoveel mogelijk geautomatiseerd beheer ondersteunen en minimale handmatige actie vereisen.

---

### NFR-03 – Beveiliging en AVG-compliance
**Omschrijving**  
Als TI-directeur wil ik dat het BI-systeem voldoet aan de AVG, zodat persoonsgegevens veilig worden verwerkt. 

**Achtergrond**  
Het systeem verwerkt bedrijfs- en klantgegevens. 

**Prioriteit**  
Must have

**Uitwerking**
- Role-Based Access Control  
- Dataminimalisatie  
- Ondersteuning AVG-rechten  

---

### NFR-04 – Systeemarchitectuur en schaalbaarheid 
**Omschrijving**  
Als IT-directeur wil ik dat het BI-systeem schaalbaar is, zodat toekomstige groei mogelijk is. 

**Achtergrond**  
Nieuwe databronnen en gebruikers kunnen in de toekomst worden toegevoegd. 

**Prioriteit**  
Must have

**Uitwerking**
- Het systeem moet uitbreidbaar zijn met nieuwe databronnen en gebruikers. 

---

### NFR-05 – Open source en leveranciersvoorkeur 
**Omschrijving**  
Als IT-directeur wil ik voorkeur geven aan open-source oplossingen en Europese leveranciers, zodat afhankelijkheid wordt beperkt. 

**Achtergrond**  
Er is een voorkeur om niet afhankelijk te zijn van Amerikaanse softwareleveranciers. 

**Prioriteit**  
Should have 

**Uitwerking**
- Het systeem moet bij voorkeur open-source zijn en draaien op niet-Amerikaanse cloud of on-premise infrastructuur.

---

### NFR-06 – Prestatie en responstijd 
**Omschrijving**  
Als BI-gebruiker wil ik dat dashboards snel laden zodat ik efficiënt kan werken zonder wachttijden. 

**Achtergrond**  
Trage systemen verminderen productiviteit. 

**Prioriteit**  
Must have

**Uitwerking**
- Standaard dashboards laden binnen 3 seconden  
- Zware rapportages binnen maximaal 10 seconden  
- Geen vertraging bij gelijktijdig gebruik door 30–50 gebruikers
  
---

### NFR-07 – Kosten-efficiëntie
**Omschrijving**  
Als financieel directeur wil ik dat het BI-systeem kostenefficiënt is, zodat de investering binnen 1–1,5 jaar wordt terugverdiend. 

**Achtergrond**  
Er is een duidelijke break even point vanuit management. 

**Prioriteit**  
Must have

**Uitwerking**
- De totale oplossing moet binnen het vooraf gestelde budget blijven met focus op lange termijn waarde. 
---

