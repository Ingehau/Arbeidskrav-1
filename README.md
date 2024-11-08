# Arbeidskrav-1
#Arbeidskrav 1, PY1010-1-24H Grunnleggende programmering med Python

#Anta at du skal kjøpe bil. Det står mellom elbil og bensinbil, og du ønsker å sammenlikne de årlige kostnadene ved elbil #sammenliknet med bensinbil.

#Lag et Python-program som beregner og presenterer (i konsollen) de årlige totalkostnadene for elbil og for bensinbil samt #årlig kostnadsdifferanse basert på informasjonen gitt nedenfor. Du kan her for enkelhets skyld se bort fra kostnader som #renter på billån og verditap (du har da egentlig antatt at slike kostnader er like for elbil og bensinbil).

#Nedenfor er informasjon som programmet skal baseres på.

#Du kan selv velge antall kjørte km/år ut fra din typiske bilbruk. Ev. (hvis du ikke har bil) kan du anta 10.000 km.
#Forsikring: Elbil: 5000 kr/år. Bensinbil: 7500 kr/år.
#Trafikkforsikringsavgift: 8,38 kr/dag for både elbil og bensinbil.
#Drivstoffbruk: Elbil: 0,2 kWh/km. Strømpris (antar kun hjemmelading): 2.00 kr/kWh. Bensinbil: 1,0 kr/km.
#Bomavgift: Elbil: 0,1 kr/km. Bensinbil: 0,3 kr/km.

#KM = Antall km kjørt per år
KM = 10000 

#FE = Forsikringsavgift for elbil pr år
FE = 5000

#FB = Forsikringsavgift for bensinbil pr år
FB = 7500

#TF = Trafikkforsikringsavgift per år for elbil og bensinbil
TF = 3058

#DFE = Drivstoffforbruk i kr pr km for elbil
DFE = 0.4

#DFB = Drivstoffforbruk i kr pr km for bensinbil
DFB = 1

#BE = Bomavgift for elbil pr km
BE = 0.1

#BB = Bomavgift for bensinbil pr km
BB = 0.3


Drivstoffkostnad_elbil = KM * DFE

Bomkostnad_elbil = KM * BE

Fast_kostnad_elbil = FE + TF


total_kostnad_elbil = Drivstoffkostnad_elbil + Bomkostnad_elbil + Fast_kostnad_elbil


Drivstoffkostnad_bensinbil = KM * DFB

Bomkostnad_bensinbil = KM * BB

Fast_kostnad_bensinbil = FB + TF


total_kostnad_bensinbil = Drivstoffkostnad_bensinbil + Bomkostnad_bensinbil + Fast_kostnad_bensinbil


print("Årlig totalkostnad for elbil =", total_kostnad_elbil)

print("Årlig totalkostnad for elbil =", total_kostnad_bensinbil)

Differanse_kostnad_elbil_og_bensinbil = total_kostnad_bensinbil - total_kostnad_elbil

print("Årlig kostnadsdifferanse mellom elbil og bensinbil med 10 000km kjørt er", Differanse_kostnad_elbil_og_bensinbil, "kr")

