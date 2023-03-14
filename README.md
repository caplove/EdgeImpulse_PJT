# EdgeImpulse_PJT


## 파일(csv, jpg, wav)을 프로젝트에 업로드 

![image](https://user-images.githubusercontent.com/24836829/224903834-33534a8e-3ffd-4420-889f-82aa1bd7fcb8.png)

edge-impulse-uploader --clean

edge-impulse-uploader filename.csv

edge-impulse-uploader --category testing *.csv

edge-impulse-uploader --category testing *.jpg

edge-impulse-uploader --label IDLE *.jpg

edge-impulse-uploader --category testing --label ABNORMAL *.jpg


## 데몬 실행할 경우 (EI 의 AI 모형을 사용)
edge-impulse-daemon 

edge-impulse-daemon --clean

## EI에서 컴파일한후, Embedded 다운로드하고 나서, Embedded System의 AI 모형을 사용
edge-impulse-run-impulse 

edge-impulse-run-impulse --continuous


## 실시간으로 데이터를 EI 서버로 올릴때
edge-impulse-data-forwarder --frequency 1

edge-impulse-data-forwarder --baud-rate 460800 (디폴트 115,200)

