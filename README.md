# 📱💻 폰고 전자기기 거래 서비스 분석

### 본 프로젝트는 코드스테이츠 AIB 교육 과정에서 진행한 기업협업 프로젝트입니다.
---
전체 프로젝트 내용은 [여기](https://github.com/Jinseon-Kim/-/blob/main/%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3%20%E1%84%8C%E1%85%A5%E1%86%AB%E1%84%8E%E1%85%A6%20%E1%84%87%E1%85%A9%E1%84%80%E1%85%B5.pdf)를 통해 보실 수 있습니다.

• 진행기간 : 2022년 11월 17일 ~ 12월 14일

• 기업명 : 피에로컴퍼니

• 팀원 : 김진선, 주민선

## 1. 프로젝트 개요
### **1️⃣ 프로젝트 목적**

- 사용자의 거래 이탈 원인 분석과 거래 예약율을 높이기 위한 액션 제안 

### **2️⃣ 기업 및 서비스 소개**

피에로컴퍼니는 전자기기 리퍼비시 플랫폼, '폰고'를 운영하는 스타트업입니다. 

해당 플랫폼은 휴대폰을 비롯한 전자기기의 수리 및 거래를 돕는 O2O(online to offline) 서비스를 제공하며 사용자로부터 매입한 기기를 재정비 후 판매와 렌탈 서비스로 연결시킴으로써 자원의 선순환을 실현하고 있습니다. 

이번 프로젝트는 ***폰고의 전자기기 거래 서비스***만을 대상으로 진행하였습니다.
   
 <p align="center"><img width="804" alt="폰고 서비스 설명" src="https://user-images.githubusercontent.com/106254025/210538389-35255478-46ce-4a5d-adcb-21f9c32c7178.png"></p>
   
### **3️⃣ 문제정의**
2022년 피에로컴퍼니는 2023년 리퍼비시 전자기기 렌탈 서비스 추진을 위해 전자기기 매입 확대에 주력했습니다. 서비스 홍보를 위한 광고, 이벤트 집행으로 매달 사용자 유입은 증가했지만 거래 예약율(견적요청 대비 거래예약 사용자수)은 평균 10%대에 머물렀습니다. 데이터 전담조직이 존재하지 않아 데이터 활용 능력이 낮은 피에로컴퍼니에서 DA 직무를 수행하며 사용자 이탈에 대한 원인을 분석하고 핵심 지표 개선을 위한 액션을 제안했습니다.

<p align="center"><img width="500"src="https://user-images.githubusercontent.com/106254025/211009794-cf9d7dcf-bce4-4d05-8d8e-11cd1b52fb02.png"></p>

### **4️⃣ 분석 방향**

- AARRR 프레임워크 중 Activation 단계에 대한 퍼널 분석 
   - 폰고 서비스에 유입된 사용자가 거래를 완료하기까지의 과정은 다음과 같이 5단계로 구성되며 폰고 서비스의 핵심 가치를 거래예약으로 선정하였습니다. 또한 견적 요청 후 업체로부터 견적이 도달하기까지 사용자의 이탈이 불가피하기 때문에 서비스 유입 ~ 거래예약 여정을 서비스 유입 ~ 견적요청, 견적조회 ~ 거래예약 2개 파트로 나눈 후 페이지뷰를 기준으로 세부 퍼널을 구성하였습니다.
   
 <p align="center"><img width="500" alt="image" src="https://user-images.githubusercontent.com/106254025/211472731-c71935d6-344c-471f-8f19-a2590190d8ab.png"></p>

<p align="center"><img width="500" alt="image" src="https://user-images.githubusercontent.com/106254025/211473976-5b461240-9363-40cc-bd3d-22e88a8af852.png"></p>

- 코호트별 거래 예약율 분석
   - 폰고 사용자 데이터를 기반으로 거래예약율에 영향을 미치는 코호트를 발견한 후 폰고 서비스 광고 및 이벤트 설계 적합성을 검토하였습니다.

   
## 2. 프로젝트 결과
- AARRR 프레임워크 중 Activation 단계에 대한 퍼널 분석
   - 해당 기업의 구글 애널리틱스 로그는 사용자의 세부 액션을 알 수 있는 행동 로그 설계가 미흡한 상황이었으므로 페이지뷰별 URI를 추출하여 퍼널 분석을 진행하였습니다.
   - 사용자 유입 ~ 견적 요청 5단계 퍼널 분석 결과를 통해 퍼널 축소를 고려해보았으며 특히, sns에서 서비스 페이지로 사용자 유입을 유도하는 광고 랜딩 페이지의 변화가 견적 요청 전환율에 긍정적인 영향을 미치는지 살펴보았습니다. 또한 유입 채널별 전환율을 비교하여 상대적으로 전환율이 낮은 채널에 대한 원인을 분석했습니다.
   - 견적 조회 ~ 거래 예약 4단계 퍼널 분석 결과, 재방문자의 거래 예약 동선이 불편함을 파악하였으며 재방문자의 반복적인 과정 노출을 최소화 시킬 수 있는 UX 개선을 제안하였습니다.

- 코호트별 거래 예약율 분석
   - 폰고 사용자 데이터 EDA를 통해 '전자기기 상태 등급'과 '견적요청 시간' 2가지 코호트에서 거래예약율 차이가 존재함을 확인하였습니다. 기존 마케팅 및 이벤트의 사용자 타기팅이 적절했는지를 검토한 후 거래 예약 전환율이 높은 코호트를 중심으로 서비스 개선을 제안하였습니다.
   

- [기업측으로부터 받은 피드백 바로가기](https://www.notion.so/b4a18fd258db4ccf85693acce2b2ad2b)


## 3. 데이터 설명 
- 구글 애널리틱스(UA) 로그

- 폰고 사용자 데이터, shape(3064, 10)
   - 폰고 서비스로 견적 요청한 사용자에 대한 기본정보(견적요청날짜, 주소, 기기 정보, 진행 상태, 요청 사항 등)

## 4. 자체 평가 의견
- 좋았던 점
   - 실제 비즈니스 문제를 가지고 AARRR 프레임 워크의 고객 활성화(Activation)에 대한 퍼널 분석 진행
   - 기업 서비스 및 시장 분석을 통해 도메인 이해 
   - 단계별 전환율을 구하고 해당 데이터에 근거하여 기업에 액션 제안 
- 아쉬운 점
   - 구글 애널리틱스의 사용자 행동 로그, user-id 미설정으로 도출할 수 있는 데이터 해석의 한계 존재 
   - BI 솔루션을 활용하여 SQL을 통한 데이터 추출과 시각화를 계획했으나 스프레드 시트 단독 사용
   
