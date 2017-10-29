# Was ist Kovri und warum ist es wichtig für Monero?

24. August 2017 11:43 von Jamie Holmes

In einer neuen [OpenHours-Ausgabe](https://www.youtube.com/watch?v=b0k5lTMFXBA) vom 17. August nahmen einige Monero-Mitwirkende teil, um über das Kovri-Projekt zu sprechen. Das Projekt zielt darauf ab, die Privatsphäre im Monero-Netzwerk weiter zu verbessern, indem die Erlangung jeglicher Informationen über Transaktionen praktisch unmöglich gemacht wird. Außerdem kann Kovri potentiell zur Standardmethode werden, um IP-Adressen zu verbergen.
## Kovris Resonanz mit Monero
[Kovri](https://getkovri.org/) ist eine C++-Implementierung eines I2P-Routers. Kurz gesagt, ein universelles Anonymisierungs-Overlay-Netz, ähnlich wie Tor. Ein typischer I2P-Router ist in Java geschrieben, Kovri hingegen in der C++-Sprache, um die Kompatibilität mit der auf die Privatsphäre fokussierten Kryptowährung Monero (XMR) zu gewährleisten. Zurzeit arbeiten 48 Mitwirkende am Projekt, um es in die Alpha-Phase zu bringen.

Was ist Kovri und wie kam es dazu? Riccardo Spagni, der Lead Maintainer des [Monero](https://getmonero.org/)-Projekts, erklärte, „weil Monero als Projekt privatsphärenfreundlich ist, haben wir begonnen, uns anderer Projekte anzunehmen, die nicht nur für das Monero-Ökosystem von Vorteil sind, sondern auch für Privatsphäre-Liebhaber allerorten, und so kam Kovri zustande.“

Der Anfang von Kovri spiegelt den von Monero wider. Beide wurden von Open-Source-Projekten wegen eines fehlenden Glaubens an die Führung der ursprünglichen Entwicklungsteams geforkt. In Moneros Fall war es [BitMonero](https://btcmanager.com/moneros-third-birthday-a-complex-history-promising-future/). Bei Kovri war es i2pd.

Anfang 2015 machte sich der Urheber von i2pd, einer C++-Implementierung von I2P, [zum alleinigen Beitragenden](https://monero.stackexchange.com/questions/2324/what-is-the-difference-between-i2pd-and-kovri), nachdem ein Entwickler einen Commit auf GitHub pushte. Diese Aktion verärgerte andere Entwickler und führte zur Trägheit eines derartigen C++-Projekts. Im Herbst 2015 versuchte dann [Anonimal](https://github.com/anonimal), der derzeit die Entwicklung von Kovri leitet, das Projekt wiederzubeleben und reichte den aktiven i2pd-Entwicklern einen Ölzweig.

Obwohl der Urheber von i2pd nicht antwortete, begann die Einzelperson stattdessen wieder auf GitHub zu arbeiten, außerhalb des von der Gemeinde betriebenen Branches. Einerseits eine Trotzreaktion, aber auch ein Warnsignal für Entwickler, die einem solchen Projekt nachgehen wollten.

Um jedweden Schaden an den Aussichten einer C++-Implementierung von I2P abzumildern, führte Anonimal eine Reihe von Besprechungen durch, die ab November 2015 den Grundstein für das Kovri-Projekt legten. Diese Gruppe forkte dann weg von i2pd aufgrund des Würgegriffs, dem dessen Entwicklung ausgesetzt war.

Anonimal erklärte Kovris Zweck in der OpenHours-Ausgabe, seiner ersten öffentlichen Besprechung des Projekts: „Im Wesentlichen werden wir Monero-Transaktionen noch stärker anonymisieren können, als es derzeit, technisch gesprochen, auf der Netzwerkschicht möglich ist.“

In [Anonimals Antrag von Ende 2016](https://forum.getmonero.org/9/work-in-progress/86967/anonimal-s-kovri-full-time-development-funding-thread) legte er seine Argumentation für Kovri als eine Alternative zu [Tor](https://www.torproject.org/) dar:

> „Während ich Tor ungemein liebe und sie mit Zähnen und Klauen verteidigen werde, bestehen zum Zeitpunkt dieses Schreibens zwei Probleme, die mich hinsichtlich des Tor-Projekts am meisten beunruhigen:

> Erstens befindet sich der aktuelle Zustand des Projekts mit einem neuen Management in bedenklichem Wandel: Freiwillige, die dem Kern angehörten und seit den frühen Anfangsjahren mit dem Projekt verbunden waren, entwurzeln sich und ziehen davon, es gibt allgemein bekannte Auseinandersetzungen innerhalb der Organisation, es gibt viele Gerüchte (sowohl begründet als auch unbegründet) über eine Unterwanderung durch die US-Regierung.

> Zweitens Tors Achillesferse: Autoritäten, Konsens und flussbasiertes Onion-Routing (wie derzeit in Tor implementiert) sind nicht wirklich dezentral.“

Aber verschleiert Monero nicht Transaktionsziele und Transaktionssummen? Ja, aber, wenn man eine Transaktion durchführt, teilt man dem Netzwerk mit, dass diese im nächsten Block enthalten sein soll. Die IP-Adresse, mitsamt anderer Metadaten, wird geleakt, allerdings nicht für immer in die Blockchain eingetragen.

Böswillige Akteure könnten versuchen, IP-Adressen zu ermitteln, falls sie aktiv das Netzwerk überwachen. Das erklärt, warum Kovri so wichtig ist. Monero-Mitwirkender SamsungGalaxyPlayer (SGP) konstatierte: „[Kovri] wird es sehr, sehr schwer machen, hoffentlich unmöglich, diese Informationen nachzuverfolgen.“

Spagni ergänzte, dass ein solcher Angriff, obwohl möglich, schwer durchzuführen wäre: „Die IP-Adresse ist nicht in der Transaktion enthalten. Sie müssen eigene Netzknoten betreiben und dann beobachten, welcher Netzknoten zuerst eine Transaktion überträgt. Es ist also ein schwer durchführbarer Angriff, bei Bitcoin ist es früher schon vorgekommen und vielleicht könnte es sogar bei Monero passieren, wir würden es nicht wissen...“

### „Monero wird nie fertig sein... Kovri wichtig für Privatsphäre und Dezentralisierung“

Eine der interessanteren Fragen, die in der Sendung aufkam, lautete wie folgt: *Nehmen wir an, Kovri ist integriert und es gibt mobile Wallets für XMR, was sind die größten, langfristigen Herausforderungen, denen sich Monero gegenübersieht?*

SGP antwortete, dass die beiden größten Herausforderungen für Monero darin bestehen, dezentral zu bleiben und die Privatsphäre weiterhin zu stärken. „Wir haben im Augenblick keine Systeme, die vollkommen privat sind. Wir müssen dem immer näher kommen.“ Er führte weiter aus, dass „wir so ziemlich an einem Punkt sind, an dem Monero hinreichend privat ist, jetzt müssen wir es hinreichend effizient machen.“

Aufgrund der Verschleierungsqualitäten sind Moneros Transaktionen größer als Bitcoin-Transaktionen, da mehr Daten auf der Blockchain gespeichert werden. Die Verschlankung dieser Transaktionsgrößen ist ein vorrangiges Anliegen des Teams. Die jüngsten Mitschriften aus der [Monero-Entwickler-Besprechung](https://monerobase.com/wiki/DevMeeting_2017-08-20) stellen diesbezüglich zwei fruchtbare Zugänge heraus. RingCT 2.0 und Forscher Tim Ruffings sublineare Ringsignaturen + CT, was den zusätzlichen Vorteil hat, keinen vertrauenswürdigen Aufbau zu benötigen.

> „Monero wird nie fertig sein, es wird also immer mehr Arbeit geben. Sowohl für die Dezentralisierung als auch für die Stärkung der Privatsphäre ist Kovri wohl ein wichtiger Aspekt.“ - SGP

Ebenso wie Kovri die Dezentralisierung und die Privatsphäre von Monero stärkt, wird es auch dabei helfen, die Akzeptanz und den Wert von XMR zu erhöhen. Die Menschen werden der Kryptowährung mehr und mehr vertrauen, sobald sie überzeugt sind, dass jede Transaktion ihre Anonymität wahrt. Nach der Veröffentlichung der Beta-Version von Kovri wird es standardmäßig laufen, d.h., jeder Nutzer wird von einer zusätzlichen Schicht I2P-Anonymität profitieren.

## Die ideologische Gemeinschaft treibt die Entwicklung voran

Andere Gesprächsthemen während der OpenHours-Ausgabe waren Spagnis Ansichten über den Blockchain-Konsens und die Fortschritte auf Seiten der Entwicklung: „Interessanter als der Preis (von XMR) ist das konstante Wachstum auf Seiten der Entwicklung.“

> „Wir haben regelmäßig neue Mitwirkende, die scharenweise hereinströmen, einige von ihnen bleiben eine kurze Weile, einige aber für lange Zeit, und sie arbeiten an etwas, ohne bezahlt zu werden. Es gibt einige Mitwirkende, die über unser Crowdfunding-System Geld gesammelt haben, aber die große Mehrheit arbeitet an Monero, weil sie es gerne tun und es herausfordernd und interessant finden, nicht weil sie denken, dass sie reich werden.“ - Riccardo Spagni

Wie Brandon Goodell, Doktor (Ph.D.) der Mathematik, der zu Monero stieß, um die Kryptowährung zu verbessern, Anonimal wurde auch von der Gemeinde durch das interne Crowdfunding-System für das Projekt unterstützt. In der Show deutete er sogar an, dass die beiden in naher Zukunft zusammen an Kovri arbeiten würden.

Mit einer Finanzierung von mehr als 7.000 XMR kann Anonimal als altgedienter Monero-Mitwirkender Vollzeit am Projekt arbeiten. Spagni hob hervor, dass zwei Entwickler und ein Forscher auf diese Weise crowdfinanziert werden. Er bemerkte: „Es ist schön, weil es nur beweist, dass es trotz der vielen Betrügereien in dem Bereich ... ein Projekt gibt, das primär ideologisch getrieben ist und eine Gemeinde hat, die bereit ist, die Entwicklung und die Entwickler ohne Probleme zu finanzieren.“

## Kovri ist wichtig für die Privatsphäre, nicht nur für Monero

Kovri ist kein exklusives Projekt für Monero. Mit dem Ziel, systemagnostisch zu sein, wird Kovri für jeden, der gegebenenfalls Anonymität benötigt, wie etwa Whistleblower und Journalisten, nützlich sein.

Wie von Anonimal erläutert: „Langfristig möchte ich das, was wir brauchen, reduzieren und die Implementierung dessen, was wir haben, verbessern und außerdem Kovri zu einer systemagnostischen Anonymitätsanwendung in Bezug auf die API-Nutzung machen. Monero könnte die API nutzen, doch Kovri könnte zur nächsten Generation von Anonymitätssystemen avancieren... Wir wollen etwas, das für jeden nützlich ist und das auch eine langfristige Anonymitätslösung für Monero sein wird.“

XMR wurden zwar verwendet, um Anonimal zu finanzieren, seine Arbeit wird allerdings positive Spillover-Effekte haben und Menschen außerhalb des Monero-Ökosystems begünstigen.

Obwohl Kovri kein Erscheinungsdatum hat, ist es ein aufregendes Projekt, das von vielen in der Kryptowährungsgemeinde mit Spannung erwartet wird. Kovri ist nicht nur für Monero wertvoll, sondern auch allgemein wichtig für die Privatsphäre, denn es wird eine doppelte Funktion erfüllen: als eigenständiger I2P-Router und als einfach zu bedienende Schnittstelle zu Moneros grafischer Benutzeroberfläche (GUI).

Als Anonimal während der Show näher in die Kryptografie hinter dem Projekt eintauchte, äußerte er seine Überzeugung, dass Kovri das aufregendste Projekt sei, an dem ein Kryptograf überhaupt arbeiten könne:

> „[Kovri] ist wie ein Krypto-Sammelsurium ... also es macht wirklich Spaß, das ist *das* Projekt, in das man sich vertiefen kann, denn wir haben mit so vielen Dingen zu tun und einige wirklich tolle Ideen, die schon seit einem Jahrzehnt entwickelt werden...“


Der Originaltext in englischer Sprache findet sich unter https://btcmanager.com/what-is-kovri-why-is-it-important-for-monero/. 
