# Objektssegmentierung mit YOLO

Dieses Repository enthält die Implementierung und den Vergleich verschiedener YOLO-Modelle (YOLOv8, YOLOv11, YOLOv12) zur Instanzsegmentierung im Kontext des **RoboCup@Work**.

## Inhalt
- `Trained_Annotation.ipynb` - Erstellung der Labels für den gegebenen Datensatz(Polygon Masken)
- `YOLOv8_seg.ipynb` – Training und Konversion mit YOLOv8  
- `YOLO11_seg.ipynb` – Training und Konversion mit YOLOv11  
- `YOLO12_seg.ipynb` – Training und Konversion mit YOLOv12
- `FineTuning.ipynb` - Training (Fine Tuning aller vorigen Modelle) und Konversion mit allen Modellen
- `README.md` – Projektbeschreibung
- `Videos` - Ordner mit den Videos

## Datensatz
Verwendet wurde ein bestehender Datensatz mit drei Objektklassen aus dem RoboCup@Work-Set:
**Motor**, **Kugellager**, **Schraubenzieher**.


## Ziel
Vergleich der Modellarchitekturen im Hinblick auf:
- Genauigkeit  
- Inferenzgeschwindigkeit  
- Eignung für Edge-Hardware (NVIDIA Jetson Orin, OAK-D Pro)

## Umgebung
Das Training wurde in **Google Colab** durchgeführt.  
Modelle basieren auf den offiziellen Implementierungen von **Ultralytics**.
