[🇺🇸 English](./README.md) | [🇰🇷 한국어](./README.ko.md)

# 📚 책 추천 시스템

**Team Bookaholic**의 프로젝트에 오신 것을 환영합니다! 이 프로젝트는 Mason Liebe, Nami Kim, San Kim, Wai-Sum Wu가 개발한 개인화된 책 추천 시스템입니다. 펜실베이니아 대학교의 CIS5450 수업에서 배운 내용을 바탕으로, 단순한 "이 책도 좋아하실 거예요" 수준을 넘는 추천 알고리즘을 구현했습니다.

🔗 웹 앱 체험하기: [Streamlit App](https://cis545-book-project-60m9b4032y8.streamlit.app/Parameter_based_book_recommender)  
🖥️ 프론트엔드 리포지토리: [https://github.com/wuwaisum0517/cis545-book-project](https://github.com/wuwaisum0517/cis545-book-project)


## 프로젝트 개요

우리는 다음과 같은 질문에서 출발했습니다:  
> *"다음에 무슨 책을 읽지?"*

이 질문에 답하기 위해 BookCrossing에서 수집한 대규모 데이터를 분석하고, 사용자의 과거 평가 및 인구통계 정보(나이, 지역)를 활용하여 책을 예측하는 추천 시스템을 만들었습니다.


## 데이터셋

출처: Kaggle [Book Recommendation Dataset](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset)

- **Users:** `user_id`, `location`, `age`  
- **Books:** `ISBN`, `title`, `author`, `publisher`, `year`, `cover image URL`  
- **Ratings:** `user_id`, `ISBN`, `rating` (1–10 점수)

이 데이터셋을 선택한 이유는 사용자 나이 및 지역과 같은 인구통계 정보가 포함되어 있어 **개인화된 추천**을 구현하기에 적합했기 때문입니다.


## 주요 기능

- **협업 필터링 (Collaborative Filtering)** — 사용자-도서 평점 매트릭스 기반
- **콘텐츠 기반 필터링 (Content-based Filtering)** — 사용자 지역 및 나이 활용
- **콜드 스타트 문제 해결** — 클러스터링 및 메타데이터 활용
- **Streamlit 인터페이스** — 다양한 추천 모드를 실시간 체험 가능


## 노트북 보기  
https://github.com/namikimlab/book-recommender/blob/main/Final_notebook.ipynb


## 🧰 기술 스택

| 분류             | 도구 / 라이브러리                          |
|------------------|---------------------------------------------|
| **언어**          | Python 3                                   |
| **데이터 처리**    | Pandas, NumPy                              |
| **시각화**         | Matplotlib, Seaborn                        |
| **머신러닝**       | Scikit-learn, KMeans                       |
| **앱 프레임워크**   | Streamlit                                 |
| **개발 환경**      | Jupyter Notebook                           |
| **데이터 출처**     | Kaggle BookCrossing 데이터셋              |


## 배운 점과 도전 과제

이 프로젝트를 통해 다음과 같은 경험을 쌓았습니다:

- 크고 복잡한 데이터셋의 정제 및 전처리  
- 희소 행렬 기반의 추천 모델 설계  
- 결측치, 이상치, 콜드 스타트 문제 해결 전략  
- 간단하면서도 직관적인 사용자 인터페이스 설계

그리고 무엇보다도, 정말 재미있었어요 😄
