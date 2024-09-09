# Free-Hand Sketch Recognition

## Pregled

Ovaj projekat se bavi kreiranjem i podešavanjem konvolucionih neuronskih mreža (CNN) za klasifikaciju ručno nacrtanih skica u 20 različitih kategorija. Cilj je eksperimentisati sa prilagođenim arhitekturama CNN-a i unapred istreniranim modelima (npr. VGG16) koristeći tehnike transfer učenja i fine tuning.

## Skup podataka

Dataset korišćen u projektu je kolekcija od 20,000 skica, svaka obeležena klasom objekta koji je označava (ukupno 250 klasa). Dataset se može naći [ovde](https://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/).

Mi smo se odlučili za podskup ovog dataseta. Naš dataset sadrži 1600 slika podeljenih u 20 različitih klasa. Razlog ovoga je to što sa našim mašinama nemamo dovoljno resursa za treniranje modela klasifikacije slika u 250 klasa. Takođe, slike su same po sebi teške za učenje, što dodatno otežava treniranje.

!!ubaciti ovde prikaz slika

### Preprocesiranje Podataka:
- **Transformacije**: 
  - Promena veličine na 224x224 (originalna dimenzija 1111x1111)
  - Slučajna rotacija i afine transformacije
  - Brisanje delova slika
  - Pretvaranje u tenzor i normalizacija

Dataset je podeljen na trening i validacioni skup (80% od ukupnog broja slika) i test skup(20% od ukupnog broja slika).

## Instalacija neophodnih zavisnosti

Da biste instalirali sve potrebne zavisnosti za projekat, koristite sledeću `pip` komandu:
    **pip install -r requirements.txt**

## Literatura

1. [Klasifikacija skica - TU Berlin](https://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/)
2. Materijali sa vežbi


## Autori

* Mirko Kordic, mirko22kordic@gmail.com
* Dragana Zdravkovic, dragana.zdravkovic602@gmail.com