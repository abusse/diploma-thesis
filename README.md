# Diplomarbeit - SSD-basiertes Caching von Blockgeräten

This is the LaTeX source code of my diploma thesis that I wrote back in 2010 at
TU Berlin. The topic is _SSD based caching of block devices_. However, the
thesis is only available in German (sorry for the inconvenience). The document
can be build with [latexmk](https://ctan.org/pkg/latexmk). The source code for
the Linux kernel extension developed for the thesis is linked as submodule in
the `linux` directory.

In case you want to cite the document, please use the following BibTex entry:

```
@thesis{busse2010ssdcaching,
    title  = {SSD-basiertes Caching von Blockger\"aten},
    author = {Anselm Busse},
    school = {Technische Universit\"at Berlin, Germany},
    type   = {Diploma Thesis},
    year   = 2010,
    month  = jun,
    doi    = {10.14279/depositonce-6939},
    url    = {https://depositonce.tu-berlin.de/handle/11303/7761}
}
```

---

This thesis discusses whether it is feasible and reasonable to use a solid-state
drive (SSD) as cache for a traditional magnet platter based hard disk drive.

The mass storage realized through a hard disk drive is often the bottleneck in
current computers. The reason for that is that the access time of a hard disk
drive is several magnitudes inferior to the one of the next layer in the memory
hierarchy – the main memory – due to its mechanical nature. To tackle this
issue, semiconductor-based mass storage that does not display this disadvantage
was introduced in recent years as a replacement for hard disk drives. This type
of storage is marketed as solid-state drives. However, SSDs have the
disadvantage that the cost per byte is much higher in comparison to hard disks.
Because of this, the complete replacement of hard disk drives by solid-state
drives cannot be expected in the near future.

That results in the current situation where users store the most frequently used
data on a small SSD and the remaining data on a slower hard disk drive. This
approach is cumbersome for the end user. In order to overcome this issue, this
thesis proposes the use of SSDs as a transparent cache for hard disk drives.
This would require only a small degree of intervention by the user and would
still enable him or her to experience the benefits of SSDs.

The thesis is of the following structure. It starts with a discussion of the
technological background of hard disk and solid-state drives followed by the
presentation of related works and concepts relevant to the topic of this thesis.
Based on this background, a precise research question is established. To answer
it, the thesis continues with the proposition of an architecture for a block-
based cache and discusses an actual implementation of this architecture. On the
basis of this implementation, extensive simulations and measurements were
possible and the scientific question of this thesis is discussed thoroughly by
the means of their results.

---

Diese Arbeit beschäftigt sich mit der Frage, ob es möglich und sinnvoll ist ein
Solid State Drive (SSD) als Cache für eine herkömmliche Magnetscheiben-basierte
Festplatte zu nutzen.

In aktuellen Rechnersystemen stellt häufig der Massenspeicher in Form einer
Festplatte den Flaschenhals des Systems dar. Dies ist darauf zurückzuführen,
dass Festplatten auf Grund ihres mechanischen Aufbaus eine Zugriffszeit haben,
die um mehrere Größenordnungen schlechter ist als die der nächsten Stufe in der
Speicherhierarchie -- dem Arbeitsspeicher. Um dieses Problem zu beseitigen,
wurde in den letzten Jahren halbleiterbasierter Massenspeicher als Ersatz für
Festplatten eingeführt, der dieses Defizit nicht besitzt. Diese Laufwerke werden
unter der Bezeichnung SSD vermarktet. SSDs haben jedoch den Nachteil, dass die
Kosten pro Byte wesentlich über denen von Festplatten liegen. Darum ist mit
einer vollständigen Substitution von Festplatten durch SSDs in den kommenden
Jahren kaum zu rechnen.

Die momentane Situation, die daraus resultiert, ist die, dass Anwender häufig
genutzte Daten auf einer meist kleinen SSD speichern und die restlichen Daten
auf einer langsameren Festplatte. Dieses Vorgehen ist für den Nutzer jedoch sehr
umständlich. Deshalb wird in dieser Arbeit die Nutzung von SSDs als
transparenter Cache für Festplatten vorgeschlagen. Dadurch würde nur ein
geringes Eingreifen des Nutzers erforderlich sein und es ihm trotzdem
ermöglicht, die Vorteile von SSDs zu nutzen.

Es werden im Verlauf dieser Arbeit dafür zunächst die technischen Grundlagen von
Festplatten und SSDs dargestellt und andere Arbeiten betrachtet, die ein
ähnliches Konzept verfolgen bzw. für die praktische Realisierung des Cache von
Bedeutung sind. Auf Grundlage dieser technischen und theoretischen
Rahmenbedingungen wird eine konkrete Problem- und Aufgabenstellung formuliert.
Basierend auf dieser wird eine Architektur für einen blockbasierten Cache
vorgeschlagen, deren konkrete Implementierung ebenfalls in dieser Arbeit
beispielhaft dargestellt wird. Mit Hilfe dieser Beispielimplementierung wurden
für diese Arbeit Simulationen und Messungen durchgeführt. Sie ermöglichen es die
Frage zu beantworten, ob es sinnvoll ist, eine SSD als Cache zu nutzen. Somit
wird abschließend diese Fragestellung anhand der gewonnenen Messergebnisse unter
den Gesichtspunkten der Leistungssteigerung und des zusätzlichen
Ressourcenverbrauchs durch den Cache diskutiert.
