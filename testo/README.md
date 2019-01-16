# README

## Introduzione

Introduzione agli strumenti per veloci correzione ai contenuti audio. Livelli, compressione, normalizzazione, alcuni esempi.

Introduzione ad strumenti veloci per la riduzione del rumore nei contenuti audio.
Approfondimento equalizzazione, gating, noise removal.

## materiale necessario per il relatore

* cavo a y oppure
* scatola a y + cavo miniTRS-miniTRS + 2x cavi TS-TS
* 2x altoparlanti
* (opzionale) scheda audio

## presequisiti

Nessun prerequisito richiesto

## materiale richiesto ai partecipanti

### hardware

* laptop
* una paio di cuffie o auricolari (facoltativo)

### software

* installazione di Audacity (free software, multipiattaforma, gratuito)
* installazione (facoltativa) di Reaper (fully-functional demo, economico, multipiattaforma)
* scaricare una cartella di samples preparati


## a che domande dobbiamo rispondere?

* finalizzando il tutto alla pubblicazione su Youtube (musica e altro hanno altre regole)
* volume basso o alto!
* suona male? ha un buon contenuto in frequenza?


## Caratteristica 1: ampiezza (perturbazione - livello - volume) (30 minuti)

souno è una perturbazione della pressione dello stato di quiete delle particelle di un mezzo elastico (gassoso, solido o liquido)
particelle di un mezzo elastico compressione e rarefazione

[gif animata]()

ampiezza di picco
ampiezza picco picco
ampiezza RMS (valore efficiace)

Pa (Pascal)
20µPa minima ampiezza percepibile da un orecchio medio (link)[https://en.wikipedia.org/wiki/Sound_pressure#Examples_of_sound_pressure]
100 Pa - la pressione sonora oltre alla quale si determinano pesanti danni al sistema uditivo
1 Pa = 94dBSPL

la risposta del nostro sistema uditivo non è sufficientemente rapida da consentire la percezione completa dell'alternarsi di picchi di compressione e rarefazione.
Questo perchè il nostro orecchio lavora su delle medie (RMS - media quadratica sotto radice) temporali effettuate per altro ad intervalli regolari di tempo ( 50 ms)
la scala logaritmica si usa per comodità di rappresentazione (il range che ci porta da 20µPa a 100Pa si estende su 8 oridini di grandezza metre una scala logaritmica comprime il tutto).

il decibel ovvero la decima parte del Bel
il Bel non è una unità di misura come potrebbe esserlo il Volt, il metro o il litro.
Si tratta piuttosto di una masura di un rapporto (relativa).

Se io dico che il valore A è il doppio del valore B ecco che uso il numero 2 non tanto in termini assoluti quanto per descrivere A in relazione a B. Se volessimo dire la stessa cosa sfruttando il concetto di dB allora diremmo che A è dB maggiore di B.
Si basano sui logaritmi che possiamo tralasciare

ma pensiamo a quanto è più semplice usare i dB piuttosto che dire 0.5, 0.24, 10000 volte di più, 100000 volte di più etc

1 Bel rappresenta la differenza in una scala relativa di valori con potenza 10
relativa significa con un riferimento

più vicino al nostro sistema percettivo 1Pa - 2Pa è percepito loud il doppio proprio come 50pa - 100pa (6dB)
20 log(valore da misurare / valore di riferimento)

curve isofoniche accenni

## Audio digitale accenni

grafico pressione microfono ADC audiofile

audio campionato (frequenza di campionamento / bit depth)

se anzichè un microfono ne avete due potete raccogliere il doppio delle informazioni da due punti diversi dello spazio e magari ottenere un file che si dice essere stereofonico

* frequenza di campionamento / bit depth
* mono / stero / multicanale
*

### Esercizio A: dialogo-fireworks.wav (30 minuti)

audacity

non esiste un unico modo per raggiungere il risultato.
Non conosco in modo super approfondito gli strumenti ma in questa occasione mi piaceva condividere quello che ho imparato sul loro utilizzo se può essere di qualche utilità.

Parentesi: userò due tool in modo intercambiabile, principalmente allo scopo di mostrarvi al meglio le cose
e dal momento che ogni tool ha i propri punti di forza useremo l'uno o l'altro a seconda dei particolari su cui ci focalizzeremo
cercherò di mostrarvi  come si fa sia in audacity che in reaper

carica il file
ascoltiamolo
obiettivo (alzare il volume)
vediamo i samples (super zoom)

la prima cosa che ci viene im mente amplificatione
usiamo un plugin - che cos'è?

amplificazione
moltiplicare significa
mantiene inalterati gli equilibri dinamici tra i suoni presenti nel materiale audio originale.

amplifichiamo di 12dB (moltiplichiamo i sample per un fattore 4)
i fireworks clippano (come si visualizzano i clip?)

annulliamo
meglio (?) un sistema chiamato normalizzazione

(che cosa fa normalize?) effettua una amplificazione del segnale audio
andando a moltiplicare i valori numerici di ciascun samples per una costante impostata


stabilisce lui un livello di amplificazione adeguato basandosi sul sample maggiore
non molto efficacie --> la voce è ancora bassa

ci piaceva con l'amplificazione? sì
torniamo ad ampligicare allora
dove sono i problemi?

tagliamo il primo firework sovrascrivendogli il silenzio
eventuale fade in (smoothing)

altrove effettuiamo una automazione del volume

esportazione

---

### Esercizio B: ABC.wav (25minuti)

Reaper
carichiamo
possiamo cominciare con il normalizzarlo

ascoltiamolo
elementi estranei

potremmo scrivere il silenzio (in reaper è più un fatto di taglia)
infattibile in termini di sbatti
infattibile perchè può capitare di sbagliarsi e sovrascrivere audio utile
un processo automatico --> gate

Gate
che cosa è e come funziona

catena audio in/out
curva lineare delle ampiezze

[illustrazione 1]

[illustrazione 2]

ora ci serve applicare il gate come si fa?
click su fx, cerchi gate, inserisci gate
avvantaggiamoci dell'interfaccia grafica che è un po' più intuitiva

modificate la th è già solo così dovreste avere l'effetto desiderato, il clock è sparito

Anche la voce potrebbe cancellarsi per via del fatto che ha un inviluppo

![grafico dell'inviluppo]()

Perchè non funziona sempre?
a volte il contributo utile è miscelato al contributo indesiderato
compromesso

esportazione in Reaper


### Esercizio Bbis: snare.wav

snare con gate


## Caratteristica 2: frequenze (contenuto spettrale)

Finora abbiamo analizzato il fenomeno suono basandoci su una delle sue caratteristiche principali: l'ampiezza.

E' anche vero che quando un corpo, sollecitato comincia a vibrare in sè lo fa in molti modi diversi.

le sue superfici si distorcono nel tempo in modo molto particolari.
Esse, spostandosi dalla propria posizione di equilibrio cominciano a spostarsi - in avanti e indietro - con diverse rapidità.

In queste distorsioni sono presenti moltissimi tipi diversi di vibrazione che, trasferite per contatto al mezzo elastico, arrivano al microfono e al nostro orecchio il quale è ingrado di percepirle tutte.

Non proprio tutte in realtà: il nostro orecchio è in grado di percepire e discriminare vibrazioni che abbiano una rapidità che varia tra 20 volte al secondo fino a 20 mila volte al secondo.

le interpreta come **Pitch** (intonazione).

L'unità di misira che sta ad indicare la rapidità di queste vibrazioni, che in altre parole e la rapidità nel susseguirsi di zone di compressione e rarefazione è l'Hertz.

L'hertz è una unità di misura per descrivere la frequenza.

esempio con Pure data

Tutte queste vibrazioni sono simultaneamente presenti nel movimento di un corpo sollecitato da un colpo o uno sfregamento, però sono presenti con energie diverse.

Tutte queste energie, distribuite su tutte queste possibili vibrazioni, concorrono a creare l'ampiezza del suono.

Il suono può essere letto quindi secondo una prospettiva differente:

* se prima interpretavamo il suono esaminando il livello di ampiezza complessivo su base del tempo;
* ora potremmo esplorare cosa succede, sempre su base temporale, all'energia delle vibrazioni individuali presenti in esso.

Costruiamo un altro tipo di rappresentazione dove sull'asse verticale sono indicate tutte le possibili vibrazioni.



### Esempio merlo

Dallo spettrogramma possiamo ricavare molte informazioni su come è il suono
e come il **timbro**: il timbro è ciò che ci permette di distinguere una chitarra elettrica da un pianoforte, anche se questi due strumenti stanno suonando la stessa nota e con lo stesso volume.

* eventualmente chirp
crea un chirp da 20 a 20000 durata 10s
mostra lo spettrogramma
fai vedere le frequenze

* shamekia
indagine sui diversi tipi di filtro, equalizzatore (peaking e shelving)
per enfatizzare o attenuare l'energia di certe vibrazioni
mantendo le latre inalterate (o quasi :)

### Esercizio C: female_hum_high_tremolo.wav (20 minuti)

hum ronza 50Hz --> equalizzatore

### Esercizio D: noise_snare.wav (20 minuti)

proviamo dappriam con un gate -- uhm, insomma il rumore resta
allora proviamo con un equalizzatore, però finisce che andiamo a modificare anche il suono utile

reaper FIR con
noise remover (learn - apply)
è sempre un compromesso perchè sì perde definizione sulle alte frequenze del rullante.

[Audacity - Noise Reduction](https://manual.audacityteam.org/man/noise_reduction.html)

---

### Esercizio E: voice_with_noise.wav



### PRO



## PS

aliasing - rolling shutter effect/wagon wheel effect

processori di dinamica: compressore
ratio, threshold, tempi di attacco e rilascio
limiter (al massimo)

limiter dipende dal software a volte sfuggono
quindi brick wall limiter (event horizon)
fallo vedere con fireworks

sistema percettivo (differenze tra individui) per questo si crea uno standard di riferimento

standard ITU

[loudness war](https://en.wikipedia.org/wiki/Loudness_war)
[alignment level](https://en.wikipedia.org/wiki/Alignment_level) = -18dBFS (RMS)

Articolo interessante a riguardo sul sito di T.C. ELectronics
https://www.tcelectronic.com/brand/tcelectronic/loudness-explained#googtrans(en|en)

### Audacity plugins

Scritti in [Nyquist](https://en.wikipedia.org/wiki/Nyquist_(programming_language))

* [installing](https://wiki.audacityteam.org/wiki/Download_Nyquist_Plug-ins#install)
* [gate audacity](https://wiki.audacityteam.org/wiki/Nyquist_Effect_Plug-ins#Noise_Gate)
