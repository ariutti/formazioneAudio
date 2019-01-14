
carica il file ABC.wav

obiettivo (alzare il livello e eliminare, se possibile, il rumore)

normalizza
lo scopo in genere è quello di allineare il sample più grande con un valore impostabile.

E' differente dal processo di compressione ed espansione che vedremo in seguito.

rumore --> scrivici il silenzio

lasicate aperto audacity -->ve lo faccio vedere in reaper che è più pratico

create una nuova traccia con doppio click
inserite un nuovo item
zoom
dobbiamo normalizzare (come avevamo fatto in precedenza su audacity)


## Esempio pratico su un file di voce (32 minuti)

potremmo scrivere silenzio --> infattibile
abbiamo visto in reaper il gate
vediamo in audacity anche se è più complesso
applichiamo
dove l'audio ha una ampiezza sotto la goglia scrive zero
altrove lascia il file originale --> abbiamo ancora il rumore
più fastidioso che altro --> è come se ce ne accorgessimo di più ora perchè non è più parte di un fondo costante
al quale il nostro cervello può abituarsi e cancellarlo per noi
il gate non va bene
usiamo il noise reduction

eventuale problema dello zero crossing

step1 get noise profile
spiegazione
step2 remove noise
spiegazione:
è meglio farne di più e meno incisivi
artifatti

normalizzazione
non funziona

compressione

(rivedi)

[Leveler](https://ttmanual.audacityteam.org/man/Leveller) --> è una combinazione di Compressione e Limiter

ulteriore passaggio di noise reduction

confronto

ancora qualcosa che non va in alta frequenza, un altro passaggio di noise removal

ci sono basse frequenze --> usiano un EQ e filtriamole

spettro della voce (lo abbiamo fatto prima?)

Leveler --> se usato con settaggio di tipo hard/heavy può causare distorsioni (mostra cosa è successo sui picchi problematici)

l'expander lo fai dopo
