# Cos'è Kovri e perchè è importante per Monero?

Agosto 24, 2017 11:43 per Jamie Holmes

Nell'[episodio di OpenHours](https://www.youtube.com/watch?v=b0k5lTMFXBA) del 17 Agosto, diversi contributori di Monero si sono uniti allo show per parlare del progetto Kovri. Quest'ultimo ha l'obiettivo di migliorare ulteriormente il livello di privacy offerto da Monero, rendendo virtualmente impossibile dedurre qualsiasi informazione riguardo le transazioni. Inoltre, Kovri potrebbe diventare il metodo di riferimento per nascondere il proprio indirizzo IP.
## La relazione tra Kovri e Monero
[Kovri](https://getkovri.org/it/index.html) è un'implementazione in C++ del router i2p. In poche parole, un network di copertura per uso generale, simile a Tor. Un tipico router I2P è scritto in Java, mentre Kovri è scritto in C++, per assicurare compatibilità con la moneta privacy-centrica Monero (XMR). Al momento, 48 contributori stanno lavorando per portare il progetto nella fase alpha.

Cos'è Kovri e come ci si è arrivati? Riccardo Spagni, il manutentore leader del progetto [Monero](https://getmonero.org/), ha spiegato che "siccome Monero è un progetto incentrato sulla privacy, abbiamo iniziato ad adottare altri progetti, dei quali non beneficia solo l'intero ecosistema dietro Monero, ma anche gli appassionati di privacy ovunque siano, ed è così che è arrivato Kovri"

Gli inizi di Kovri sono simili a quelli di Monero. Entrambi sono stati forkati da altri progetti open-source, non condividendo più la direzione che il team di sviluppatori originario stava prendendo. Per Monero si trattava di [BitMonero](https://btcmanager.com/moneros-third-birthday-a-complex-history-promising-future/), per Kovri, i2pd.

All'inizio del 2015, l'autore iniziale di i2pd, un'implementazione in C++ di I2P, si è dichiarato unico contributore quando uno sviluppatore ha "spinto" un commit su GitHub. Offendendo gli altri sviluppatori, quest'azione risultò nell'inerzia di questo progetto C++. Nell'autunno 2015, Anonimal, che attualmente guida lo sviluppo di Kovri, provò a resuscitare il progetto e offrì un ramoscello d'ulivo agli sviluppatori attivi di i2pd.

L'autore originale di i2pd non rispose, ma invece ritornò a lavorare su GitHub, ma non sul ramo della repository guidato dalla community. Un atto sprezzante e allo stesso tempo una spia d'allarme per gli sviluppatori del progetto.

Per mitigare ogni danno alla prospettiva di un'implementazione C++ di I2P, Anonimal condusse una serie di meeting, che formarono le basi per il progetto Kovri a partire dal Novembre 2015. A causa della stretta piazzata agli sviluppatori, questo gruppo decise di separarsi, eseguendo una fork del progetto i2pd.

Anonimal ha spiegato per la prima volta in pubblico lo scopo di Kovri nell'episodio di OpenHours: "Essenzialmente, saremo in grado di anonimizzare ulteriolmente le transazioni di Monero, tecnicamente parlando, uno strato nel network."

Nella sua [proposta del tardo 2016](https://forum.getmonero.org/9/work-in-progress/86967/anonimal-s-kovri-full-time-development-funding-thread), ha spiegato le sue ragioni per Kovri come alternativa di [Tor](https://www.torproject.org/):

> "Mentre amo Tor tremendamente e lo difenderei con le unghie e con i denti, nel momento in cui scrivo ci sono 2 problemi che mi preoccupano di più riguardo il progetto: 

> Primo, con la nuova gestione, lo stato attuale del progetto ha un flusso discutibile: volontari chiave che sono stati con il progetto fin dai primi anni, lo stanno lasciando. Ci sono conflitti all'interno dell'organizzazione pubblicamente noti. Ci sono molte voci (sia fondate che infondate) riguardo infiltrazioni da parte del governo statunitense.

> Secondo, il tallone d'Achille di Tor: autorità, consenso, e flow-based onion-routing (come attualmente implementato in Tor), non sono veramente decentralizzate."

Ma Monero non offusca destinatari e ammontare delle transazioni? Si, ma quando effettui una transazione, comunichi al network che vuoi essere incluso nel prossimo blocco. Il tuo indirizzo IP, insieme ad altri metadati, trapela. Ma il tuo indirizzo IP non viene registrato per sempre.

Malintenzionati potrebbero provare a capire il tuo indirizzo IP se monitorano attivamente la rete e spiega perchè Kovri è così importante. SamsungGalaxyPlayer (sgp), un contributore di Monero, dice "[Kovri] renderà molto, molto difficile, speriamo impossibile, monitorare queste informazioni."

Spagni ha aggiunto che, per quanto possibile, un attacco del genere sarebbe difficile da applicare, "il tuo indirizzo IP non è incluso nella transazione. Dovrebbero avere un nodo personale, dopodichè osservare quale nodo trasmette una transazione per primo, quindi è difficile da portare a termine. è successo con Bitcoin in passato e potrebbe persino succedere con Monero, noi non lo potremmo sapere..."

### "Monero non sarà mai finito... Kovri importante per Privacy e Decentralizzazione"

alcune delle domande più interessanti uscite durante l'episodio sono a seguire; *Ipotizziamo che Kovri sia integrato e che Monero abbia portafogli per mobile, quali sono le più grandi sfide a lungo termine che Monero dovrà affrontare?*

SGP ha risposto che, per Monero, le due più grandi sfide sono: rimanere decentralizzato e continuare ad incrementare il livello di privacy. 
"Non abbiamo nessun sistema, in questo momento, che è perfettamente privato. Dobbiamo continuare ad avvicinarci a questo obiettivo ". Ha continuato dicendo che, "Siamo a un punto in cui Monero è ragionevolmente privato, adesso dobbiamo farlo diventare ragionevolmente efficente."

A causa delle qualità offuscative, le transazioni di Monero sono più grandi di quelle di Bitcoin, siccome più dati sono sonservati nella blockchain. Diminuire le dimensioni di queste transazioni è una delle priorità chiave del team. Ci sono due sviluppi importanti da questo punto di vista, come evidenziato dai recenti appunti dal [Monero dev meeting](https://monerobase.com/wiki/DevMeeting_2017-08-20). RingCT 2.0 e le ring signatures + CT, che ha il vantaggio aggiunto di non richiedere un set-up fidato.

> "Monero non sarà mai finito, quindi ci sarà sempre più lavoro. Per renderlo più decentralizzato e migliorare la privacy, Immagino Kovri sia un importante aspetto per entrambe le cose." - SGP

Oltre a miglioreare la decentralizzazione e privacy di Monero, Kovri aiuterà anche a dare una spinta al valore e all'adozione di XMR. La gente comincerà a fidarsi della cryptomoneta sempre di più una volta che saranno più fiduciosi nel fatto che ogni transazione li mantiene anonimi. Dopo il rilascio in beta di Kovri, sarà implementato di defalut in Monero, così ogni utente potrà beneficiare dell'extra strato di anonimato I2P.

## La comunità ideologica sta guidando lo sviluppo

Altri punti di discussione dell'episodio di OpenHours sono state le visioni di Spagni sul "consensus" sulla blockchain e i progressi fatti dal lato dello sviluppo, "più interessante del prezzo (di XMR) è la crescita costante dal punto di vista dello sviluppo."

> "Abbiamo visto un flusso di nuovi contributori, alcuni rimangono per poco tempo, ma altri rimangono per molto, e lavorano a qualcosa senza essere pagati. Ci sono alcuni contributori che hanno raccolto fondi tramite il nostro sistema di crowdfunding, ma la maggior parte lavora su Monero perchè gli piace e lo trovano interessante, non perchè pensano che diventeranno ricchi." - Riccardo Spagni

Come Brandon Goodell, [il matematico che è stato preso a bordo di Monero](https://btcmanager.com/no-ico-just-altruism-how-phd-mathematician-future-proof-monero/) per analizzare la cryptomoneta, anche Anonimal è stato finanziato dalla community tramite il sistema di crowdfunding interno al progetto. Ha anche suggerito durante lo show, che i due lavoreranno insieme sullo sviluppo di Kovri nel prossimo futuro.

Con più di 7000 XMR raccolti per Anonimal, può lavorare a tempo pieno sul progetto. Spagni ha aggiunto che due sviluppatori e un ricercatore sono stati finanziati in questo modo. Ha commentato, "è bello perchè va a provare che anche se ci sono un sacco di truffe in giro... puoi sempre avere un progetto che primariamente è guidato ideologicamente e ha una community disposta a finanziare lo sviluppo senza problemi."

## Kovri è importante per la privacy, non solo per Monero

Kovri non è un progetto esclusivo per Monero. Mirando ad essere un sistema agnostico, Kovri sarà utile per chiunque potrebbe aver bisogno di anonimato, come informatori e giornalisti. 

Come ha spiegato Anonimal, "A lungo termine, mi piacerebbe ridurre ciò di cui abbiamo bisogno e aumentare le implementazioni di quello che abbiamo già e anche rendere Kovri agnostico in termini di utilizzo API. Monero potrebbe usare le API, ma Kovri potrebbe evolversi nel sistema di anonimizzazione della prossima generazione...Vogliamo qualcosa che sia utile per chiunque e che sia anche una soluzione a lungo termine per anonimizzare Monero."

Mentre XMR è stato usato per finanziare Anonimal, il suo lavoro avrà effetti positivi a largo spettro, beneficiando gente all'esterno dell'ecosistema di Monero.

Mentre Kovri non ha una data di rilascio, è un progetto che è fortemente aspettato da molti nella comunità delle cryptomonete. Non è solo importante per Monero, Kovri è importante anche per la privacy in generale,  dato che avrà una doppia funzione; Un autonomo router I2P e un'interfaccia facile da utilizzare con la Monero GUI.

Analizzando la criptografia dietro al progetto durante lo show, Anonimal ha espresso il suo pensiero riguardo al fatto che Kovri è il progetto più interessante al quale un crittografo potrebbe lavorare:

> "[Kovri] è come un buffet ... è davvero divertente, questo è *il* progetto su cui lavorare, perchè abbiamo così tante cose con cui lavorare e alcune idee che sono sviluppare da più di un decennio..."


Il testo originale è disponibile a https://btcmanager.com/what-is-kovri-why-is-it-important-for-monero/. 

