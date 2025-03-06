# Detaljerad Roadmap för Velomobilprojektet

## 1. Konceptutveckling och konfigurationsval

### Skalmodellering och utvärdering
- Skapa enkla skalmodeller (1:10) av alla fyra konfigurationer:
  * 2-hjulig: Lägst vikt och bäst aerodynamik men problematisk stabilitet och tillvänjning
  * Tilting tadpole: Optimal körkänsla men mest komplicerad konstruktion
  * Vanlig tadpole: God stabilitet i vila men problem med kurvstabilitet vid högre hastigheter
  * 4-hjuling: Bäst stabilitet och lastkapacitet men högre vikt och komplexare styrning
- Utveckla artikulerad dummy för ergonomisk utvärdering (använda antropometriska standardmått)
- Testa styrsystem och mekaniska funktioner i skalmodell
- Iterativt förbättra och eliminera mindre lämpliga konfigurationer

### Potentiella problem att lösa:
- Styrgeometri för optimal kurvtagning och stabilitet
- Balans mellan låg vikt och strukturell integritet
- Manövrerbarhet i låga hastigheter, särskilt för 2-hjuliga konfigurationer
- Lutmekanism för tilting tadpole-konfigurationen

## 2. Tekniska specifikationer

### Drivlina
- Motor: Bafang eller Tong Sheng mittmotor (36V)
- Batterisystem:
  * Snabbt bytbara batterier
  * Kompatibilitet med både dedikerade cykelbatterier och seriekopplade 18V Ryobi-batterier
  * Standardiserade kontakter för enkel integration
- Växellösning:
  * Primärt växelnav för enklare underhåll och växling i stillastående
  * Flexibilitet för både kedja och Gates remdrift
  * Överväganden för servicebarhet och delar som kan behöva bytas

### Material och struktur
- 3D-utskrivbara komponenter i PETG, ABS eller liknande material
- Transparenta paneler av akryl/polykarbonat, cylindriskt böjda (ej sfäriskt välvda)
- Fokus på standardinfästningar och lätt åtkomliga komponenter
- Designstrategi för att minimera behov av specialverktyg och former

## 3. Design och ergonomi

### Sittkonstruktion
- Flätad sadelgjordssits integrerad med skalet för:
  * Viktbesparing genom eliminering av separat ramkonstruktion
  * God ventilation och komfort
  * Enklare tillverkning och montering
- Balans mellan sitthöjd och aerodynamik:
  * Tillräckligt hög för god sikt och trygghet
  * Tillräckligt låg för aerodynamiska fördelar
  * Halvliggande position som kompromiss

### Lastkapacitet
- Dimensionering för veckohandling (ca 75-100 liter, 25-40 kg)
- Alternativa lastplaceringar:
  * Long John-stil: låg lastposition fram, god stabilitet men längre hjulbas
  * Omnium-stil: hög lastposition fram, kompaktare men högre tyngdpunkt
  * Last bakom föraren: minimal påverkan på styrning men svårare att nå under körning
- Lastsäkring och väderskydd för transporterat gods

## 4. Tillgänglighet och användbarhet

### In- och urstigning
- Bredare öppning än traditionella velomobiler
- Stöd eller handtag för att underlätta
- Optimerad instegshöjd
- Design som inte kräver extremt god rörlighet

### Daglig användbarhet
- Intuitivt handhavande även för oerfarna användare
- Stabilt läge vid stillastående (särskilt viktigt för 3- och 4-hjuliga konfigurationer)
- Praktisk för korta sträckor och vardagstransport
- Minimalt underhållsbehov

## 5. Väderskydd och komfort

### Skalkonstruktion
- Aerodynamiskt skal med cylindrisk/konisk framruta
- Öppna sidor för ventilation (så långt sitskonstruktionen medger)
- Avrinningslösningar för nederbörd
- Hänsyn till kondensbildning på insidan av transparenta ytor

### Ventilation och temperaturreglering
- System för att undvika överhettning vid varmt väder
- Balans mellan väderskydd och luftcirkulation
- Ljudnivå inuti velomobilen (vindbrus, vägljud)
- Skydd mot stänk från hjul och väg

## 6. Säkerhetsfunktioner

### Synlighet och belysning
- LED-belysning fram och bak
- Högt placerad bakbelysning för bättre synlighet i trafik
- Reflekterande material på strategiska platser
- Blinkersystem för svängsignalering

### Bromssystem
- Effektiva bromsar på minst två hjul
- Hydrauliska skivbromsar för pålitlig bromsverkan i alla väderförhållanden
- Parkeringsbroms för säker parkering
- Bromskraftsfördelning anpassad efter fordonskonfiguration

### Strukturell säkerhet
- Skalkonstruktion med förstärkningar vid kritiska punkter
- Design som förhindrar inträngning vid kollision från sidan
- Krockabsorberande zoner där möjligt
- Säker förvaring av personliga tillhörigheter under körning

## 7. Dokumentation och versionshantering (GitHub)

### Repostruktur
- `/designs` - CAD-filer och 3D-modeller
- `/docs` - teknisk dokumentation
- `/images` - foton och renderingar
- `/src` - eventuell kod för elektronik
- `README.md` - projektöversikt

### Dokumentationstyper
- Tekniska ritningar med mått och toleranser
- Bill of Materials (BOM) för standardkomponenter
- Steg-för-steg monteringsanvisningar
- Design-beslut och resonemang med visuella förklaringar (SVG/PNG)
- Testresultat med mätdata

### Versionshantering
- Git tags för viktiga milstolpar
- Branches för olika konfigurationer
- Issues för att spåra problem och idéer
- Pull requests för större designändringar

## 8. Test- och utvärderingsmetodik

### Skalmodeller
- Visuell utvärdering av proportioner och estetik
- Test av styrsystem och mekaniska funktioner
- Utvärdering av väder- och vindskyddskoncept
- Passformskontroll för standardkomponenter i skala

### Fullskalig prototyp
- Strukturell integritet och hållfasthet under verkliga förhållanden
- Ergonomisk komfort vid längre användning
- Faktisk väder- och vindskyddseffektivitet
- Köregenskaper vid olika hastigheter och underlag
- Energieffektivitet och räckvidd med elassistans
- Verifiering av lagkrav och säkerhet

## 9. Budget och resursplanering

### Utvecklingskostnader
- Minimera behov av specialtillverkade former och verktyg
- Sprida kostnader över tid genom stegvis utveckling
- Fokus på lösningar som är enkla att utveckla även om de skulle ge högre styckepris
- Utnyttja begagnade standardkomponenter när möjligt

### Tillverkningsaspekter
- Prioritera design som kan tillverkas med tillgänglig utrustning (3D-skrivare)
- Minimera behovet av specialistkunskap för montering
- Balansera material- och komponentkostnader mot hållbarhet
- Dokumentera alternativa komponenter där möjligt för flexibilitet