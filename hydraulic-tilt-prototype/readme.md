# Hydraulisk Tilt-Prototyp för Velomobil

## Koncept
En skalprototyp för att testa ett aktivt hydrauliskt tiltsystem inspirerat av Austins Hydrolastic-system. Systemet använder hydrauliska bälgar för att kontrollera tiltningen av en trehjulig velomobil med två framhjul.

## Huvudkomponenter
- 47-203 mm hjul på 3D-utskrivna fälgar
- Hydrauliska bälgar (övre vänster och höger)
- TMC2226 stegmotordrivare (kompatibel med 36V)
- NEMA 14 stegmotor
- Kugghjulspump (3D-utskriven)
- MPU6050 accelerometer/gyroskop
- Mikrokontroller med PID-styrning
- Modulär 3D-utskriven ram

## Dimensioner
- Hjulbas: 50-60 cm
- Spårvidd: 30-40 cm

## Tekniska beslut
- Använder endast övre bälgar för lateralt vätskeflöde under tiltning
- Hydraulisk pump drivs av stegmotor för precis kontroll
- Styrning baserad på accelerometer/gyroskop-data med filtrering
- Modulär design för enkel modifiering och testning
- Strömförsörjning från 18V verktygsbatteri (36V i slutlig version)

## Mål för prototypen
1. Testa funktionaliteten hos det hydrauliska tiltsystemet
2. Mäta energiförbrukning under olika driftsförhållanden
3. Optimera PID-parametrar för stabil tiltning
4. Utvärdera stegmotor och pumpprestanda
5. Testa olika filteralgoritmer för accelerometerdata

## Nästa steg
- Design av 3D-modeller för ramkomponenter
- Val av material för hydrauliska bälgar
- Implementation av styrningskod
- Konstruktion av kugghjulspump
- Integration och testning
