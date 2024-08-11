# ObjLCC-tools
![image](https://github.com/user-attachments/assets/53e317db-ce41-4e22-b579-bd1c49e8df17)

## Installation
No need install on your device. I trying to work everything on cloud machine <br />
Optional: If you want to work on Docker It work! but you need to change path in my code. <br />
<br />

## Model
| Model  | Version | Result | Comment |
| ------------- | ------------- | ------------- | ------------- |
| Objn001  | alpha | Very bad | Need more training |
| Objn002  | alpha | Bad | Need more Dataset |
| Objn003 | Release | Very Good | It perfect for detect Lunar crater | <br />


![M1335510874LC_segment_2_34_png rf dd90d4f8824e9a4bbeb3da1559f6f84e](https://github.com/user-attachments/assets/617f9caa-31f2-470e-bb88-3a70bb997bc4) <br />
(conf=0.2 imgsz=640)


## Plan of Project
Before I get into the details, let me talk about the order of use. <br />
Go to Colab -> Prepare environment -> Split Map lunar (LROC) -> Prediction -> Reassemble Map & Label -> Convert To SCC or SHP <br />
(ฺBase on Qgis)

| Section | Status |
| ------------- | ------------- |
| Document Manual | Working in process |
| Prepare environment | Ready to use |
| Pizza Cutter Map | I need be sorted agian but ready to use |
| Landing Zone | I need be sorted agian but ready to use |
| Prediction | Ready to use |
| Convert To SCC or SHP | Working in process |

## Usage

https://colab.research.google.com/drive/1pU76VY2_q49yPOio20xvltPwC46dPvp1 <br />
![image](https://github.com/user-attachments/assets/1d75e4a9-4d69-41cf-8853-574b0bce25e0) <br />
1.Run all cell in Prepare environment <br />
Optional: If you want to use model yolov8. You will need GPU: RTX, T4, A100 or something it could run CUDA :D <br />
2.Download TIF MAP<br />
3.Convert TIP TO PNG<br />
4.Split large image to 1280x1280 and resize to 640x640 for put in to Yolov8 model<br />
5.Ready to Prediction or Training<br />
6.Predict by yolov8 model<br />
7.Reassemble Map & Label (Need to update)<br />
8.Convert Map & Labels to SCC OR SHP(Need to update)<br />

### Pizza Cuter Map
This is the part about cutting and joining scattered images and labels into a single file.

### Landing Zone
It is like a file manager that can be used to connect to Google Drive or other devices<br />

## License
GPL-3.0 license

## Credit
Natakorn Vijaranayarn - Geologist<br />
Phusin Tararukmongkol - Developer & AI <br />
Noppasit Sotawong - Worker<br />
