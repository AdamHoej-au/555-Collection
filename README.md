# 555 Timeren
Jeg har en røvfuld 555'ere i skuffen, så de skal bruges... 
Det kunne være interessant at bruge dem i stedet for microcontrollere, da jeg tror læringsprocessen i at arbejde med analog elektronik frem for digital elektronik er mere... mig. 

## Ideer

- Tonegenerator med 4 faste outputs.
  - Dette kunne være 4 dekader: [25 Hz, 250 Hz, 2.5 kHz 25 kHz]
  - Variable output spænding 
- Timed trigger source
  - Holder en trigger høj i en bestemt periode
- Envelope generator
  - AD er tilstrækkeligt.
    - Attack/Decay
  - ADSR kunne være spændende
    - Attack/Decay/Sustain/Release


### 555 Synthesizeren...

Det kunne være pisse sejt at lave en synthesizer der var baseret på 555 timeren. 

Der findes allerede APC der er en astable oscillator der driver en monostable oscillator.. Men hvad med en envelope generator? Det blev ihvertfald brugt ifb. Vekselstrøms DIY synth - sammen med en Schmitt trigger, hvis jeg ikk husker helt galt..


Men det burde også være muligt at lave en AD... Hvis man laver et gate/trig signal burde det være muligt at behandle dette med et standard RC led el. lign. hvorved en $\exp(-t/RC)$ funktion.. 

Jeg ved at det klassisk med en switch til at skifte m. en stor/lille kodensator, hvorved man kan skabe to tidsperioder.. Stor og lille.. Hvilket stemmer overens med $\tau = RC$. Hvor $\tau$ er tiden det tager at stige/falde 63%/37% fra maks ampltiude til base tilstand.