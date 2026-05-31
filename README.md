# ml-project
# 체중 변화량 예측 회귀 프로젝트

## 프로젝트 개요

본 프로젝트는 개인의 식습관, 신체 활동, 수면, 스트레스 등 생활습관 요인을 바탕으로 체중 변화량을 예측하는 회귀 프로젝트이다. Kaggle의 Diet Analysis, Predict The Weight 데이터셋을 사용하였다.

## 사용 모델

* Baseline Mean Model
* Linear Regression
* Ridge Regression
* Lasso Regression
* Random Forest Regressor

모델 성능은 RMSE, MAE, R²를 사용하여 평가하였다.

## 파일 구성

```text
project.ipynb
weight_change_dataset.csv
requirements.txt
README.md
```

## 실행 방법

필요한 라이브러리를 설치한다.

```bash
pip install -r requirements.txt
```

Jupyter Notebook을 실행한다.

```bash
jupyter notebook project.ipynb
```

또는 VS Code, JupyterLab, Google Colab에서 `project.ipynb` 파일을 열어 순서대로 실행하면 된다.

## 주요 결과

| Model             |  RMSE |   MAE |     R² |
| ----------------- | ----: | ----: | -----: |
| Baseline Mean     | 4.174 | 3.567 | -0.321 |
| Linear Regression | 4.575 | 3.773 | -0.588 |
| Ridge Regression  | 4.356 | 3.625 | -0.440 |
| Lasso Regression  | 4.503 | 3.731 | -0.539 |
| Random Forest     | 3.059 | 1.936 |  0.290 |

Random Forest Regressor가 가장 좋은 성능을 보였다.

## 데이터셋 출처

Kaggle, Diet Analysis, Predict The Weight Dataset
https://www.kaggle.com/datasets/abdullah0a/comprehensive-weight-change-prediction
