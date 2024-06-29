# 파이썬 설치 및 환경설정
---
+ Python : pip 툴을 가지고 있고 모두 수동으로 패키지를 설치해 사용해야함
+ Anaconda : 아나콘다는 여라가지 수학 및 패키지들을 기본적으로 포함하고 있는 파이썬 배포판 때문에 머신러닝이나 데이터 분석을 할 때, 다양한 패키지가 필요하므로 이를 사용함

아나콘다 설치 :  https://www.anaconda.com/download

![image](https://github.com/jwh1449/jungwoohyeok-studying-developer/assets/170517346/57fb5abb-729e-4499-b2e5-f378d0d4b95c)

Win키+R :CMD창 열기 or win창에서 cmd검색 후 명령 프롬프트 클릭

1. cmd창에 명령어 입력하여 가상환경 만들기(명령어 띄어쓰기 주의)
+ 원하는 폴더에서 경로창에서 cmd치고 들어가면 코드들 저장할때 원하는 폴더로 저장됨
+ Anaconda 안에 있는 파이썬 버전 확인 : conda search python(뜨면 conda 설치된거임)
+ Anaconda에서 가상환경 생성 : conda create -n 생성하고 싶은 이름 python=설치버전(3.11 or 3.11.4 가능)
+ Anaconda에서 가상환경 확인 : conda env list
+ Anaconda에서 가상환경 삭제 : conda env remove -n 삭제하고 싶은 이름
+ 현재 설치돼 있는 파이썬의 환경에서 설치된 package 종류 확인 : pip freeze
+ 생성된 가상환경 들어가기 : conda activate 가상환경이름 (activate 가상환경이름)
+ 생성된 가상환경 나가기 : deactivate

2. 주피터 노트북과 커널을 만들수 있는 패키지 설치 및 커널 만들기(가상환경 접속후)
+ 패키지 설치
pip install jupyter notebook
pip install ipykernel
+ 커널 생성하기 : python -m ipykernel install --user--name=커널이름 --display-name '원하는 이름' (찾기 쉽게 가상환경이름과 동일하게 짓는거 추천)
+ 주피터에 생생된 커널 목록확인하기 : jupyter kernelspec list
+ 주피터에 생성된 커널 삭제하기 : jupyter kernelspec uninstall 커널이름

3. 사용된 가상환경 패키지 저장
+ pip freeze > 이름.txt
+ pip install -r 이름.txt (txt파일이 같은경로에 있어야 함)
