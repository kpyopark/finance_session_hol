# BigQuery ML 시작하기

이 랩은 금융 분석 교육 세션의 일부이며 예측 분석을 위한 BigQuery ML의 강력한 기능을 소개합니다. 이 실습 랩에서는 SQL을 사용하여 BigQuery 내에서 직접 머신러닝 모델을 만들고, 평가하고, 사용하는 방법을 배우게 됩니다.

## Link

https://www.cloudskillsboost.google/focuses/2157?catalog_rank=%7B%22rank%22%3A2%2C%22num_filters%22%3A1%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=35309492

## 개요

BigQuery ML은 SQL 전문가가 특수 ML 프레임워크를 배우거나 데이터를 이동할 필요 없이 모델을 구축하고 배포할 수 있도록 하여 머신러닝의 민주화를 가능하게 합니다. 이 랩에서는 Google Merchandise Store의 공개적으로 사용 가능한 전자상거래 데이터 세트를 사용하여 웹사이트 방문자가 거래를 할지 여부를 예측하는 모델을 구축합니다.

## 학습 목표

이 랩을 완료하면 다음을 수행할 수 있습니다.

* BigQuery 데이터 세트 만들기
* SQL을 사용하여 BigQuery에서 머신러닝 모델 만들기, 평가 및 사용

## 전제 조건

* SQL 또는 BigQuery에 대한 기본 지식이 권장됩니다.

## 랩 설정

**중요:** 이 랩에서는 임시 Google Cloud 환경을 사용합니다. 개인 계정에 요금이 발생하지 않도록 랩 환경 내의 지침을 주의 깊게 따르세요.

1. **랩 시작:** 랩 환경에서 제공된 "랩 시작" 버튼을 클릭합니다.
2. **Google Cloud Console 열기:** 랩 환경이 준비되면 "Google Cloud Console 열기"를 클릭합니다.
3. **임시 자격 증명 사용:** 랩 지침에 제공된 임시 사용자 이름과 비밀번호를 사용합니다. **개인 Google Cloud 자격 증명을 사용하지 마세요.**
4. **BigQuery 콘솔 열기:** Google Cloud Console에서 "탐색 메뉴 > BigQuery"로 이동합니다.

## 랩 작업

이 랩에서는 다음 작업을 안내합니다.

1. **데이터 세트 만들기:** `bqml_lab`라는 BigQuery 데이터 세트를 만듭니다.
2. **모델 만들기:** 운영 체제, 기기 유형, 국가 및 페이지 뷰와 같은 방문자 데이터를 기반으로 거래를 예측하는 로지스틱 회귀 모델(`sample_model`)을 구축합니다.
3. **모델 평가:** 정밀도, 재현율, 정확도 및 ROC AUC와 같은 측정값을 사용하여 `sample_model`의 성능을 평가합니다.
4. **모델 사용(예측):**
    * 국가별 총 거래 수를 예측합니다.
    * 사용자별(`fullVisitorId`로 식별) 총 거래 수를 예측합니다.
5. **이해도 테스트:** 학습 내용을 강화하기 위해 객관식 질문에 답합니다.

## 주요 개념

* **BigQuery ML:** SQL을 사용하여 BigQuery 내에서 머신러닝 모델을 구축하고 실행할 수 있습니다.
* **로지스틱 회귀:** 예/아니요 결과를 예측하는 데 사용되는 통계적 방법입니다.
* **모델 평가 지표:** 머신러닝 모델의 성능을 평가하는 데 사용되는 측정값(예: 정밀도, 재현율, 정확도).

## 다음 단계 및 리소스

* **BigQuery ML 문서:** [BigQuery ML 문서 링크]
* **Google Analytics 데이터 내보내기:** [Google Analytics 데이터 내보내기 가이드 링크]
* **BigQuery SQL 참조:** [BigQuery SQL 문서 링크]

이 랩은 BigQuery ML 및 금융 분석 기능에 대한 실질적인 소개를 제공합니다. 이러한 기술을 적용하면 데이터에서 가치 있는 통찰력을 얻고 더 많은 정보에 입각한 의사 결정을 내릴 수 있습니다.