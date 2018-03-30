# Einleitung

Dieses Repository enthält verschiedene Routinen zur Plausibilitätsprüfung. Die Prüfungen können vor einem Datenimport oder nach einen Datenexport durchgeführt werden. Vor einem Datenimport, z. B. aus anderen Programmen oder beim Zusammenspielen von Datensicherungen. Beim Datenexport kann es z. B. auch verwendet werden, wenn bei einer Betriebsprüfung Daten im Sinne von "Daten vorgelagerter Systeme (DAVOS)" verlangt werden, die z. B. mit IDEAScript von Win-IDEA verarbeitet werden.

In einem Schreiben zu einer Betriebsprüfung hieß es dazu:
> Die Bp beabsichtigt einen Datenzugriff auf die der Fibu datenvorgelagerten Systeme (DAVOS), hier auf das Onlinebanking- und Fakturierungsprogramm.

In einem weiteren Absatz hieß es dann:
> Ich bitte daher mit Ihrer Mandantin abzuklären, welche Exportmöglichkeiten die jeweilige Software vorsieht. Die Bp bittet die Daten wenn möglich als .csv-Datei zur Verfügung zu stellen...

Tiefergehende Informationen dazu findet man unter [Datenzugriff GDPU](https://www.bundesfinanzministerium.de/Content/DE/Downloads/BMF_Schreiben/Weitere_Steuerthemen/Abgabenordnung/Datenzugriff_GDPdU/2014-11-14-GoBD.html) bzw. in der Fachliteratur zum Thema Betriebs- und Außenprüfung.

# Prüfungen

## fortlaufende Auftragsnummern

Prüft auf fortlaufende Auftragsnummern.

## fehlende Rechnungsnummern

Ermittelt fehlende Rechnungsnummern im Rechnungsnummernkreis des jeweiligen Kunden.

## Kunden mit Nummer 0

Ermittelt alle Kunden mit der Kundenummer 0.

## alte Rechnungsnummern von Kunden, die länger als 3 Monate zurückliegen

Ermittelt alle Kunden bei denen der Abrechnungsmonat älter als drei Monate ist und bereits Rechnungen vergeben wurden.
