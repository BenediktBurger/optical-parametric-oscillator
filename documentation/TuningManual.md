# Anleitung zur Justage eines OPOs

Die Informationen dieser Anleitung wurden aus der Justage des OPOs für [Experiment] META Aufbau neuer OPO und bei [Experiment] META MOT606 Conversion von 795 nm zu 606 nm gewonnen und nutzen die Tipps, die von verschiedenen Anwendern des Moduls Aculight Argus von Lockheed Martin gegeben wurden.

## Anwendungsbereich

Das Wissen wurde an OPOs gewonnen, die infrarot (1064 nm) gepumpt werden und deren Signalstrahlung (kürzere Wellenlänge der Differenzfrequenzgeneration) in einem Resonator um den periodisch gepolten nichtlinearen Kristall (PPLN) umläuft. Der Resonator ist in Doppel-Z-Konfiguration aufgebaut. Die Spiegel direkt am Kristall sind gekrümmt, die anderen planar.

Für die weiteren Hinweise gilt folgende Nomenklatur:

- *Einkoppler* ist der gekrümmte Kavitäts-Spiegel, durch den die Pumpe in die Kavität eingekoppelt wird.
- *Auskoppler* ist der gekrümmte Kavitäts-Spiegel, durch den Pumpe, Idler und sichtbares Licht ausgekoppelt wird.
- *Gegeneinkoppler* ist der planare Kavitäts-Spiegel, der gegenüber dem Einkoppler und zu diesem parallel steht.
- *Gegenauskoppler* ist der planare Kavitäts-Spiegel, der gegenüber dem Auskoppler und zu diesem parallel steht.

## 1. Aufbau und Vorjustage

Zu Beginn müssen die Spiegel an ihren Plätzen und in richtiger Ausrichtung aufgebaut werden, wozu eine Papierskizze helfen kann. Zur genaueren Ausrichtung kann ein sichtbarer Laserstrahl, zum Beispiel ein roter Diodenlaser oder ein grüner Laserpointer verwendet werden, solange das Licht einen Umlauf im Resonator machen kann. Dieser temporäre Laserstrahl sollte zwei Spiegel zentral treffen und die Spiegel so justiert werden, dass der Strahl einmal umläuft. Dazu ist es hilfreich, wenn der Kristall noch nicht verbaut ist. Auch kann man die Strahlen erst anhand der angefertigten Skizze ausrichten.

Der Kristall ist so verbaut, dass eine Höhenänderung die Polungsperiode ändert und er nur 0,5-1 mm breit ist.

Zur leichteren Justage sollte kein Etalon im Resonator eingebaut sein.

## 2. Justage der Pumpe

Die Pumpe sollte anfangs, mit schwacher Leistung, zentral auf die beiden gegenüberliegenden Spiegel (Einkoppler, Auskoppler) ausgerichtet werden, anschließend der Kristall eingebaut und die Pumpe so horizontal justiert werden, dass sie vorne zentral den Kristall trifft und hinten zentral verlässt, dazu ist eine Strahlkamera hilfreich, oder mit einer Wandlerkarte. Dadurch ist der Strahl in der horizontalen durch Ort und Winkel justiert.

In den verwendeten Kristallen enstand ab 0,5 W Pumpleistung die Frequenzverdoppelte der Pumpleistung, diese Frequenzverdoppelte (bei 532 nm, ab jetzt grünes Licht genannt) ist hilfreich zur weiteren Justage.

Der vertikale Ort ist relativ unwichtig, da er duch die Kristallverschiebung eingestellt wird. Der Winkel ist wichtig, um möglichst eine konstante Polungsperiode für die Pumpe zu haben. Der Winkel wird über den Spiegel der Pumpstrahlung eingestellt, der am nächsten der Kavität steht. Die verwendeten Kristalle hatten eine Beschichtung, die einen signifikanten Anteil grünen Lichtes reflektiert, sodass der Kristall wie ein Etalon wirkt und bei vertikaler Verkippung eine vertikale Reihe von Punkten erzeugt. Ziel ist es, diese Punkte zu überlagern, um ungefähr senkrecht auf den Kristall zu treffen. Umso näher man diesem Punkt kommt, umso heller wird das grüne Licht und der senkrechte Treffer zeigt sich durch eine markante Intensitätsspitze. Zwischen dem Ort maximaler Intensität und dem Ort bester Überlagerung liegt der Ort, der später die höchste Leistung bringt. Am besten auf maximale Intensität einstellen und leicht in Richtung einen Punkt gehen. Es empfiehlt sich diese vertikalen Punkte auf einem reflektierten Strahl anzuschauen, an dem die Pumpe nicht mehr vorhanden ist. Eine sinnvolle Einstellung sind 1-3 W, um genug grünes Licht zu haben.

Mit senkrechtem Treffer auf die Kristalloberfläche und guter Strahlführung durch den Kristall ist die Pumpe fertig justiert, sofern die Kavität justierbar ist.

## 3. Grobjustage der Kavität

Es empfiehlt sich, die Spiegel, die von der Pumpe durchlaufen werden (zumindest den Einkoppler), nicht anzufassen, um die Pumpe während der Justage nicht abzulenken und den Kristall zu beschädigen. Justiert wird mit Hilfe der anderen Spiegel.

Auch hier wird grünes Licht verwendet, aber nur das Licht, das vorne aus dem Kristall austritt und nicht dasjenige, das an der Austrittsseite reflektiert wird und rückwärtig umläuft. Man beobachtet das grüne Licht, das aus einem oder mehreren Spiegeln austritt an verschiedenen Orten: Nahe am Spiegel und weiter entfernt, ca 15-30 cm. Nun versucht man das Licht, das direkt aus dem Spiegel austritt mit demjenigen zu überlagern, das nach einem weiteren Umlauf erst austritt. Mit einem ersten Spiegel (Auskoppler oder Gegenauskoppler) wird auf den nahen Ort justiert, mit einem späteren Spiegel (zum Beispiel Gegeneinkoppler) wird auf den fernen Ort justiert.

Um zu erkennen, welches Licht einen weiteren Umlauf hinter sich hat, muss man den Resonator an einem Ort blocken, wo nur Licht lang kommt, das mindestens einen vollen Umlauf hat, aber keines, das auf den Schirm fällt.

Um den ersten Umlauf durch den Kristall zu justieren, kann man mit dem ersten Spiegel auf den Eintritt des Kristalls justieren und mit dem zweiten auf den Austritt. Wenn man eine feste Montage hat, zum Beispiel einen OPO Block, kann man leichter den Strahl zwischen den planaren Spiegeln parallel zum OPO-Block mit Hilfe des ersten Spiegels justieren. Anschließend justiert man mit dem zweiten Spiegel auf die Eintrittsfläche des Kristalls. Durch die Geometrie des Blocks sollte der Strahl gerade durch den Kristall gehen und man kann die Strahlen überlagern.

Bei einer guten Überlagerung bilden die Ränder der beiden Punkte ein Interferenzmuster, das wie Schmodder aussieht. Berührt man jedoch die Justierschrauben leicht, so ändert sich dieses Muster stark und ist somit als Interferenzmuster erkennbar.

Je nach Beschichtung der Spiegel, reflektiert auch die Rückseite der Spiegel das grüne Licht und man erhält eine horizontale Reihe von Punkten. In diesem Fall überlagert man den jeweils die hellsten Punkte der verschiedenen Reihen.

## 4. Feinjustage der Kavität

Wenn man den vorherigen Schritt gut gemacht hat, sollte der OPO-Prozess bei genügend Pumpleistung anlaufen. Möglicherweise muss man den Kristall ein wenig in seiner Position variieren oder an einem der Spiegel leicht drehen, um den Prozess zu starten. Mit einem Leistungsmessgerät, das die Leistung des Idlers misst, nachdem man die Pumpe rausgefiltert hat, kann man die Kavität auf maximale Leistung des Idlers justieren. Auch hier reicht es die zwei planaren Spiegel zu benutzen. Es empfiehlt sich bei stabiler OPO-Leistung die Pumpe (vertikaler Winkel) auf Leistung nachzujustieren und danach die Kavität weiterzujustieren.

Die Idler sind meist mittelinfrarot, also bieten sich thermische Messköpfe an. Auf ausreichende Leistungsreserven achten, die von uns verwendeten OPOs haben Ausgangsleistungen von ca 1 W.