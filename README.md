# Objektssegmentierung mit YOLO

Dieses Repository enthält die Implementierung und den Vergleich verschiedener YOLO-Modelle (YOLOv8, YOLO11, YOLO12) zur Instanzsegmentierung im Kontext des **RoboCup@Work**.

## Inhalt
- `Trained_Annotation.ipynb` - Erstellung der Labels für den gegebenen Datensatz (Polygonmasken)
- `YOLOv8_seg.ipynb` – Training und Konversion mit YOLOv8  
- `YOLO11_seg.ipynb` – Training und Konversion mit YOLO11  
- `YOLO12_seg.ipynb` – Training und Konversion mit YOLO12
- `FineTuning.ipynb` - Training (Fine Tuning aller vorigen Modelle) und Konversion mit allen Modellen
- `README.md` – Projektbeschreibung
- `Videos` - Ordner mit den Videos

## Datensatz
Verwendet wurde ein bestehender Datensatz mit drei Objektklassen aus dem RoboCup@Work-Set:
**Motor**, **Kugellager**, **Schraubenzieher**
Datensatz: https://drive.google.com/drive/folders/17f57NrjT8P-OMkdO7WiPx_JlayjhNLhE?usp=share_link


## Ziel
Vergleich der Modellarchitekturen im Hinblick auf:
- Genauigkeit  
- Inferenzgeschwindigkeit  
- Eignung für Edge-Hardware (NVIDIA Jetson Orin GPU, OAK-D Pro VPU)

## Umgebung
Das Training wurde in **Google Colab** durchgeführt.  
Modelle basieren auf den offiziellen Implementierungen von **Ultralytics**.
