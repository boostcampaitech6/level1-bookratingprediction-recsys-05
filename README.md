![header](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=header&text=Level1-BookRatingPrediction&desc=RecSys-05&fontSize=40&fontColor=FFFFFF&fontAlignY=40)

일반적으로 책 한 권은 원고지 기준 800~1000매 정도 되는 분량을 가지고 있습니다.

뉴스기사나 짧은 러닝 타임의 동영상처럼 간결하게 콘텐츠를 즐길 수 있는 ‘숏폼 콘텐츠’는 소비자들이 부담 없이 쉽게 선택할 수 있지만,\
책 한권을 모두 읽기 위해서는 보다 긴 물리적인 시간이 필요합니다.\
또한 소비자 입장에서는 제목, 저자, 표지, 카테고리 등 한정된 정보로 각자가 콘텐츠를 유추하고 구매 유무를 결정해야 하기 때문에\
상대적으로 선택에 더욱 신중을 가하게 됩니다.

해당 경진대회는 이러한 소비자들의 책 구매 결정에 대한 도움을 주기 위한 개인화된 상품 추천 대회입니다.

책과 관련된 정보와 소비자의 정보, 그리고 소비자가 실제로 부여한 평점,\
총 3가지의 데이터 셋(users.csv, books.csv, train_ratings.csv)을 활용하여\
이번 대회에서는 각 사용자가 주어진 책에 대해 얼마나 평점을 부여할지에 대해 예측하게 됩니다.

# :books: Stack
<img src="https://img.shields.io/badge/Linux-FCC624?style=plastic&logo=Linux&logoColor=white"/> <img src="https://img.shields.io/badge/Ubuntu-E95420?style=plastic&logo=Ubuntu&logoColor=white"/> <img src="https://img.shields.io/badge/VS Code-007ACC?style=plastic&logo=Visual Studio Code&logoColor=white"/> <img src="https://img.shields.io/badge/Python-3776AB?style=plastic&logo=Python&logoColor=white"/> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=plastic&logo=PyTorch&logoColor=white"/> <img src="https://img.shields.io/badge/Jupyter-F37626?style=plastic&logo=Jupyter&logoColor=white"/>

# :star: Team
| **이원희** | **허 욱** | **이승준** | **곽윤석** | **배건우** |
| :------: |  :------: | :------: | :------: | :------: |
| [<img src="https://avatars.githubusercontent.com/u/64073392?v=4" height=150 width=150> <br/> @lostdesire](https://github.com/lostdesire) | [<img src="https://avatars.githubusercontent.com/u/61164286?v=4" height=150 width=150> <br/> @wooksbaby](https://github.com/wooksbaby) | [<img src="https://avatars.githubusercontent.com/u/133944361?v=4" height=150 width=150> <br/> @llseungjun](https://github.com/llseungjun) | [<img src="https://avatars.githubusercontent.com/u/149780979?v=4" height=150 width=150> <br/> @younne123](https://github.com/younne123) | [<img src="https://avatars.githubusercontent.com/u/83867930?v=4" height=150 width=150> <br/> @gunwoof](https://github.com/gunwoof) |
| EDA <br> category 전처리 <br> CatBoost 모델 설계 & 튜닝 | EDA <br> book ISBN 전처리 <br> 모델 튜닝 | EDA <br> book language 전처리 <br> CNN_FM 하이퍼파라미터 튜닝 | EDA <br> User data 전처리 <br> 모델 일반화 작업 | EDA <br> LightGbm 모델 설계 & 튜닝 |

## :pushpin: TOC
- [Project](#trident-project)
  - [1. EDA](#eda)
  - [2. Preprocessing](#preprocessing)
  - [3. Model](#model)
  - [4. Hyperparameter Tuning](#hyperparameter-tuning)
  - [5. Ensemble](#ensemble)
- [Project Architecture](#mortar_board-project-architecture)
- [Environment Requirements](#floppy_disk-environment-requirements)
- [Result](#tada-result)

## :trident: Project

1. ### EDA
  - 데이터 수량 및 기초 통계량 검토
  - 결측치 확인
  - 데이터 시각화
  - 상관관계 분석
  - 피쳐 엔지니어링

2. ### Preprocessing
  - User data 전처리
  - Book data 전처리

3. ### Model
  - CatBoost
  - LightGBM
  - CNN_FM

4. ### Hyperparameter Tuning
  - Catboost
  - CNN_FM
  - LightGBM

5. ### Ensemble
  - 최종 Ensemble
    - CatBoost_v1 : CatBoost_v2 : CatBoost_v3 : CatBoost_v4 : CNN_FM = 2 : 2 : 2 : 2 : 2
## :mortar_board: Project Architecture
![Project Architecture](https://github.com/lostdesire/Level1-BookRatingPrediction/assets/64073392/ba413a3b-922e-4eb9-849b-e63dd4aadbcd)

## :floppy_disk: Environment Requirements
[requirements.txt](https://github.com/boostcampaitech6/level1-bookratingprediction-recsys-05/blob/main/requirements.txt)

## :tada: Result
![score](https://github.com/lostdesire/Level1-BookRatingPrediction/assets/64073392/2cc6c7e2-a2f4-48a1-89bd-c6139c74c859)

<img width="1091" alt="Pasted image 20231222200217" src="https://github.com/lostdesire/Level1-BookRatingPrediction/assets/64073392/4c535cd9-5453-42d4-9c4c-82d7a4db67ae">
<img width="1092" alt="Pasted image 20231222200241" src="https://github.com/lostdesire/Level1-BookRatingPrediction/assets/64073392/0af88b59-3218-438d-812b-9a2f634da755">

| 리더보드 |  RMSE  | 순위 |
| ------ | ------ | --- |
| public | 2.1285 | 3등 |
| prviate| 2.1223 | 3등 |

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=footer&text=Thanks%20for%20Reading&fontSize=40&fontColor=FFFFFF&fontAlignY=70) 
