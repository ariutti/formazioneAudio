## Caratteristica: ampiezza


## Suono

la propagazione di una perturbazione dello stato di quiete delle particelle di un mezzo elastico


<!-- .slide: data-background-size="contain" data-background-color="#fff" data-background-image="https://28oa9i1t08037ue3m1l0i861-wpengine.netdna-ssl.com/wp-content/uploads/2016/03/red-dot.gif" -->
<!-- red dot -->


<!-- .slide: data-background-size="contain" data-background-color="#ccc" data-background-image="images/Spherical_pressure_waves.gif" -->
<!-- spherical wave -->


<!-- .slide: data-background-color="#fff" -->
<!--
<svg width="60%" viewBox="0 0 350.26 240.16">

<svg class="fragment" data-fragment-index="2">
	<use xlink:href="images/sinusoid.svg#ordinate">
</svg>

<svg class="fragment" data-fragment-index="3">
	<use xlink:href="images/sinusoid.svg#rest">
</svg>

<svg class="fragment" data-fragment-index="4">
	<use xlink:href="images/sinusoid.svg#sinusoid">
</svg>

	<svg data-fragment-index="1">
		<use xlink:href="images/sinusoid.svg#ascisse">
	</svg>

</svg>
-->


<!-- .slide: data-background-color="#fff" -->
![sinusoid](images/sinusoid.png)
<!-- .element: style="position:absolute; top:0; left:0;" -->
<!-- sinusoid -->








ampiezza di picco
ampiezza picco picco
ampiezza RMS (valore efficiace)


curve isofoniche accenni


## Audio digitale accenni


grafico pressione microfono ADC audiofile


audio campionato (frequenza di campionamento / bit depth)


se anzichè un microfono ne avete due potete raccogliere il doppio delle informazioni da due punti diversi dello spazio e magari ottenere un file che si dice essere stereofonico


* mono / stero / multicanale
*

### Esercizio A: dialogo-fireworks.wav

audacity

**Parentesi**: userò due tool in modo intercambiabile, principalmente allo scopo di mostrarvi al meglio le cose
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

### Esercizio B: ABC.wav

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

Perchè non funziona sempre?
a volte il contributo utile è miscelato al contributo indesiderato
compromesso

esportazione in Reaper
