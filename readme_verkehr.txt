Die Daten der Verkhersdetektion Berlin werden monatsweise als Stundenwerte der fahrspurgenauen Verkehrsdetektoren bereitgestellt. 
Jedes csv-Archiv enth�lt die folgenden Datenfelder:

detid_15 - ID des Detektors (15-stellige Ziffer).
tag - Datum
stunde - Stunde des Tages f�r die die Messwerte ermittelt wurden (8 => 08:00 - 08:59).
qualitaet - gibt den Anteil der f�r die Stunde vorliegenden einwandfreien Messintervalle wieder: 1.0 = 100%.
q_kfz_det_hr - Anzahl aller Kraftfahrzeuge in der Stunde.
v_kfz_det_hr - Mittlere Geschwindigkeit [km/h] �ber alle Kraftfahrzeuge in der Stunde.
q_pkw_det_hr - Anzahl aller Pkw in der Stunde.
v_pkw_det_hr - Mittlere Geschwindigkeit [km/h] �ber alle Pkw in der Stunde.
q_lkw_det_hr - Anzahl aller Lkw in der Stunde.
v_lkw_det_hr - Mittlere Geschwindigkeit [km/h] �ber alle Lkw in der Stunde.

Hinweis: Es kann zu geringen Abweichungen zwischen der Anzahl aller Kraftfahrzeuge (q_kfz_det_hr) und der Summe f�r PKW (q_pkw_det_hr) und LKW (q_lkw_det_hr) kommen. 
Dies resultiert aus Rundungsfehlern auf Grund des gew�hlten Verfahrens.

Die Verortung der Detektoren und die Zuordnung der einzelnen Detektoren zu einem richtungsbezogenen Messquerschnitt findet sich in der Datei Stammdaten_Verkehrsdetektion_Berlin.xlsx.

Dies enth�lt die folgenden Datenbl�tter:
(1) DET
Zuordnung der Detektor ID (DET_ID15) zur ID des Messquerschnitts (MQ_ID15). 
Die Spalte LANE enth�lt Informationen zur Lage der Fahrspur (HF_R - 1. Spur von rechts auf der Hauptfahrbahn, HR_2vr - 2. Spur von rechts auf der Hauptfahrbahn, ...).

(2) MQ 
Daten des Messquerschnitts mit folgenden Spalten:

MQ_ID15	- ID des Messquerschnitts.
MQ_SHORT_NAME - Kurzname des Messquerschnitts.
POSITION - Name der Stra�e.
POSITION_DETAIL	- Beschreibung des Stra�enabschnitts.
DIRECTION - Fahrtziel
ORIENTATION	- Fahrtrichtung
X_GK4 - X-Koordinate (Gau�-Kr�ger-4)
Y_GK4 - Y-Koordinate (Gau�-Kr�ger-4)
ANZAHL_DET - Anzahl der zum Messquerschnitt geh�renden Detektoren.
