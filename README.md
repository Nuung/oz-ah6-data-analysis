# Python을 활용한 헬스케어 데이터 분석 및 시각화

온라인 라이브 강의용 수업 자료 저장소입니다.

- 과정: Python을 활용한 헬스케어 데이터 분석 및 시각화
- 기간: 총 3일
- 라이브 강의 시간: 10:00–15:00 KST
- Python: 3.13+

## 디렉토리 구조

```text
.
├── course/
│   ├── day01/
│   │   ├── notebooks/      # 1일차 강의 노트북
│   │   └── assignments/    # 1일차 실습 과제
│   ├── day02/
│   │   ├── notebooks/      # 2일차 강의 노트북
│   │   └── assignments/    # 2일차 실습 문제
│   └── day03/
│       ├── notebooks/      # 3일차 강의 노트북
│       └── assignments/    # 3일차 실습 과제
├── resources/
│   ├── curriculum/         # 커리큘럼/운영 문서
│   ├── documents/          # PDF 참고 자료
│   └── slides/             # 발표 자료
├── AGENTS.md               # 프로젝트 작업 지침
├── pyproject.toml          # Python 프로젝트 설정
├── requirements.txt        # pip 호환 의존성 목록
└── uv.lock                 # uv 잠금 파일
```

## 강의 노트북

- `course/day01/notebooks/1일차_Pandas기초와실습.ipynb`
- `course/day01/notebooks/1일차_데이터 타입의 이해.ipynb`
- `course/day02/notebooks/2일차_탐색적_데이터분석(EDA).ipynb`
- `course/day03/notebooks/3일차_데이터전처리.ipynb`
- `course/day03/notebooks/3일차_데이터시각화.ipynb`

`v1`, `v2`가 붙은 임시 버전 파일은 제거하고 최종본 이름만 유지합니다.

## 환경 설정

uv 사용 시:

```bash
uv sync
```

pip 사용 시:

```bash
python -m pip install -r requirements.txt
```

주요 런타임 의존성:

- pandas
- numpy
- matplotlib
- seaborn
- kagglehub

## Windows / macOS / Linux 한글 폰트

시각화 노트북의 첫 세팅 셀은 운영체제별 한국어 폰트를 자동 선택합니다.

- Windows: `Malgun Gothic` / `맑은 고딕`
- macOS: `AppleGothic`
- Linux·Colab: `NanumGothic`, `NanumBarunGothic`, `Noto Sans CJK KR` 계열

Colab/Linux에서 한글이 깨질 경우 `fonts-nanum` 설치 후 런타임을 재시작하세요.
Windows에서는 일반적으로 기본 설치된 `맑은 고딕`으로 그래프 한글 표시가 가능합니다.

## 작업 규칙 요약

- Python 3.13 이상을 사용합니다.
- 타입 힌트에는 `typing` 모듈 대신 built-in types를 사용합니다.
- Google Python Style Guide와 PEP 8을 따릅니다.
- 교육 자료를 수정할 때는 공식 문서와 좋은 예제를 적극적으로 참고하되, 수업 난이도와 맥락에 맞게 비판적으로 반영합니다.
