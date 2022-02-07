# Extract word from 해커스 보카 단어 시험지

본 모듈은 '해커스'에서 제공하는 __무료 단어장 생성기__ 에서 생성된 PDF파일에서 문제와 정답(영단어)을 추출하여 csv 파일로 반환합니다.



### 1. Installation

+ windows

```
$ install.bat
```
+ mac

```
$ sh install.sh
```

### 2. Usage

a. [해커스_단어시험\_생성기](https://www.hackers.co.kr/?c=s_toeic/toeic_info/new_voca_toeic_testpaper#;) 에서 생성한 단어장을 __test_papers__  폴더에 넣는다. (※여러개의 파일이 있을 경우 파일의 기본 순서대로 결과가 만들어 짐)

b. __terminal__ 에 __python ./Extractwords.py__ 를 입력함

```
$ python ./Extractwords.py
```



### 3. Result

완성된 결과물은 해당 폴더에  __answersheet.csv__ 로 만들어 짐


----

_추가 할 일_

1. 한글 단어 배열에 발생하는 문제 해결하기. 
	+ 사용자에게 day와 타입 인자를 받게 하고 url에서 바로 pdf를 20개씩 읽어와서 문제 만들기
	+ 중복된 단어 없이 40개의 문제가 되도록 할것

2. 문제가 발생하는 특정케이스 패턴 분석하여 예외처리하기 -> 상시 + 예외 케이스 모으기

+ Google SpreadSheet와 연동하여 자동 업데이트 만들기 -> 보류   

