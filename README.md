# 2022 성균관대학교 4th_AI_Bookathon 대회 최우수상 후기

### 제 4회 성균관대학교 주관 AI x Bookathon 대회 예선, 본선 수상 후기    
<B>팀명: 테이북(김세희, 유승한, 안세윤, 전용찬)</b>


![image](https://user-images.githubusercontent.com/109735494/215828705-8da4306a-38e9-4204-9719-15e31b88de07.png)

## 예선
예선은 12월 26일에는 사전 교육, 12월 27일에는 예선 관련 강의와 함께 예선 문제 출제가 이루어졌다.

<b>1. 12월 26일(월)</b>   
금일에는 대회 진행방식과 AI에 대한 특강이 진행되었다.    
진행된 강의들은 다음과 같다.
- 성균관대학교 교수님들의 AI 관련 특강
- 전 대회 기수상자 특강
- 대회 개최 지원사 중 하나인 마인즈랩에서 개발한 AI 설명 및 서버 설명

<br> 
<b>2. 12월 27일(화)</b>       
예선 문제가 출제되었고 팀원들과 함께 예선 문제를 풀었다.     
화요일에도 특강이 진행되었고 이 특강을 모두 수강한 이후 예선 문제가 출제되었다.         
문제를 모두 풀기까지 대략 5시간이 소요되었다.    

## 본선
본선은 일정이 하루 미루어진 1월 17일(화) ~ 1월 18일(수)에 해커톤으로 진행되었다.        
본선에서 수필 작성을 위한 키워드가 공개되었다.

------------------
### 키워드: 담대한
------------------

### 대회 참여 전략
예선 합격 이후 본선까지의 약 일주일 동안 본선을 위한 준비를 하였다.      
본선에서는 이미 사전학습된 모델을 제공했으나 외부 모델을 사용해도 되었기 때문에 모델은 skt/ko-gpt2를 사용하였다.    
따라서 본선 시작 전에 사전학습을 시켜 모델을 완성시켜야 했고 본선에서 결정적으로 중요한 것은 fine-tuning이었다.      
pretraining과 fine-tuning을 위하여 최대한 많은 소설, 수필 데이터를 수집하려고 노력했다. 

<b><수집한 데이터 목록></b>
- 브런치 수필 데이터 크롤링
- 동아신춘문예 작품
- 대표에세이 문학회
- 글틴
- 모두의 말뭉치: 비출판물 데이터

해당 데이터들을 모두 전처리하여 수집하였고 사전학습을 진행하였다.    
fine-tuning은 본선에서 키워드를 보고 해커톤 진행 도중에 데이터를 수집-전처리하여 진행하기로 하였다.     

키워드가 공개된 이후 대략적인 스토리 라인을 구성하였다. <b>총 10개의 에피소드(plot)을 생성하였고 해당 에피소드에 따른 모델을 구성하기로 하였다.</b>

### 모델
앞서 총 10개의 에피소드를 구성했는데 해당 에피소드 마다 사건을 구성하는 주요 키워드를 정리하였다.          
fine-tuning을 하기 위해서 해당 키워드를 브런치에 검색하여 수필 데이터를 크롤링하여 수집했다.          
해당 데이터를 각각 학습시켜 에피소드 별로 다른 모델들을 생성하였다.       
즉, 모델 10개를 생성한 것이 된다.            

### 최종 결과물
각 에피소드 별로 생성한 모델을 사용하여 문장을 생성했다. 한 번 생성할 때 5~10개의 문장을 생성하여 문맥이 자연스럽게 이어질 수 있도록 
문장을 선택하여 이어나갔다.    
대략 2만 자의 작품을 생성해야 했으나 시간상의 문제로 인해 2만자를 다 채우지는 못하였고 1만 자 내외의 작품을 완성하여 출품하였다.





