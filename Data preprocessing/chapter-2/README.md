# 파이썬 기초
---
+ 데이터(data) : 이론을 세우는데 기초가 되는 사실, 또는 바탕이 되는 자료
+ 정보(information) : 데이터를 가공하지 않은 경우, 이를 위한 기초적인 자료가 데이터
+ 단순구조 : 정수, 실수, 문자(숫자이외의 정보를 표현하는 방법), 문자열(둘 이상의 문자의 결합)등
+ 인코딩 : 문자를 컴퓨터가 이해할 수 있는 숫자로 변환(아스키 코드)
+ 데이터 타입 : 데이터의 형태, 의미, 크기와 해당 자료형의 값이 저장되는 방식
<br/> 문자(character) ex) "A", "Hello"
<br/> 유리수(numeric) ex) 10, 20, 1.178
<br/> 정수(integer) ex) 5, 10, 2
<br/> 논리값(logical) ex) TRUE, FALSE
<img width="623" alt="image" src="https://github.com/user-attachments/assets/0d7d09f8-2a74-43aa-8349-a5ec97074cc8">
<img width="619" alt="image" src="https://github.com/user-attachments/assets/c439b930-aa01-4d29-aba6-51245fd73665">

코드 : 설명
<br/>\n : 문자열 안에서 줄을 바꿀 때 사용
<br/>\t : 문자열 사이에 탭 간격을 줄 때 사용
<br/>\\ : 문자 \를 그대로 표현할 때 사용
<br/>\' : 작은따옴표(')를 그대로 표현할 때 사용
<br/>\" : 큰따옴표(")를 그대로 표현할 때 사용



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
<br/>pip install jupyter notebook
<br/>pip install ipykernel
