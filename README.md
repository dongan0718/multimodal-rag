# Multimodal RAG

PDF의 텍스트·표·이미지를 함께 검색해 답하는 멀티모달 RAG 실습입니다.

## 폴더 구조

```
multimodal-rag/
├── .env.example          # 키 없는 템플릿
├── requirements.txt      # 의존성 목록
├── requirements.lock.txt # 버전 고정 파일
├── data/
│   ├── invest.pdf        # 원본 PDF
│   └── figures/          # 추출된 이미지 (Git 제외)
├── notebooks/
│   └── Multi_modal_RAG.ipynb
└── src/
    ├── extract.py        # PDF 파싱 함수
    ├── summarize.py      # 요약 체인
    └── retriever.py      # 다중 벡터 검색기
```

## 시작하기

```bash
python -m venv .venv
.venv\Scripts\activate        # Windows
pip install -r requirements.txt
copy .env.example .env        # .env에 API 키 입력
```
