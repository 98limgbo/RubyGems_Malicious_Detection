## RubyGems 악성 패키지 탐지 모델

#### 프로젝트 개요
이 프로젝트는 **RubyGems** 패키지 공급망에서 **패키지 내부 메타데이터**를 활용하여 악성 패키지를 탐지하는 모델을 구축하는 연구입니다. 기존의 정적 및 동적 분석 방법이 악성 패키지를 탐지하는 데 시간이 많이 소요된다는 문제를 해결하기 위해, 본 연구에서는 패키지 내부 메타데이터만을 활용한 탐지 모델을 제안합니다. 이를 통해 배포 초기에도 악성 패키지를 신속하게 탐지할 수 있을 것으로 기대합니다.

* **extract_package_metadata.py**:  
  `.gem` 파일에서 패키지 메타데이터를 추출하고, CSV 파일로 저장하는 스크립트입니다.  
  패키지의 이름, 버전, 저자 등 주요 메타데이터를 추출하여 분석에 활용할 수 있습니다.

아래는 예시, 추후에 수정.
* 내부 메타데이터 분석을 통한 악성 패키지 탐지
* 머신러닝 알고리즘을 사용한 모델 학습
    * SVM(Support Vector Machine)
    * GLM(Generalized Linear Model)
    * GBM(Gradient Boosting Machine)
    * DRF(Distributed Random Forest)
* RubyGems 패키지에서 내부 메타데이터 추출
* 추출한 내부 메타데이터의 전처리

#### 설치 방법
아래는 예시, 추후에 수정.
* 의존성 패키지 설치
    ```bash
    pip install -r requirements.txt
    ```

#### 사용 방법
* **extract_package_metadata.py** 사용 방법
    1. `.gem` 파일을 `..\RubyGems_Malicious_Detection\data\package` 폴더에 넣습니다.
    2. `root_folder` 변수에 `.gem` 파일을 넣은 경로를 설정합니다. (기본값: `..\RubyGems_Malicious_Detection\data\package`)
    3. `output_filename` 변수에 저장할 CSV 파일 이름을 설정합니다. (기본값: `extracted_metadata.csv`)
    4. **extract_package_metadata.py**를 실행하여 메타데이터를 추출합니다.
    5. 결과는 `..\data\metadata\raw` 폴더에 CSV 파일로 저장됩니다.
나머지 추후에 추가.