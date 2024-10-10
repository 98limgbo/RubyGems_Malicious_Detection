## RubyGems 악성 패키지 탐지 모델

#### 프로젝트 개요
이 프로젝트는 **RubyGems** 패키지 공급망에서 **패키지 내부 메타데이터**를 활용하여 악성 패키지를 탐지하는 모델을 구축하는 연구입니다. 기존의 정적 및 동적 분석 방법이 악성 패키지를 탐지하는 데 시간이 많이 소요된다는 문제를 해결하기 위해, 본 연구에서는 패키지 내부 메타데이터만을 활용한 탐지 모델을 제안합니다. 이를 통해 배포 초기에도 악성 패키지를 신속하게 탐지할 수 있을 것으로 기대합니다.

#### 주요 기능
* 내부 메타데이터 분석을 통한 악성 패키지 탐지
* 머신러닝 알고리즘을 사용한 모델 학습
    * SVM(Support Vector Machine)
    * GLM(Generalized Linear Model)
    * GBM(Gradient Boosting Machine)
    * DRF(Distributed Random Forest)
* RubyGems 패키지에서 내부 메타데이터 추출
* 추출한 내부 메타데이터의 전처리

#### 설치 방법
아래는 예시, 차후에 수정.
* 의존성 패키지 설치
    ```bash
    pip install -r requirements.txt
    ```

#### 사용 방법
아래는 예시, 차후에 수정.
1. 데이터를 `data/raw/` 폴더에 저장합니다.
2. `src/data_preprocessing.py`를 실행하여 데이터를 전처리합니다.
3. `src/model_training.py`를 실행하여 머신러닝 모델을 학습합니다.
4. 결과는 `results/` 폴더에 저장됩니다.

