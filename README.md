# 동남아시아 역사 교재 — 아세안을 물들인 문자들

2027 국립세계문자박물관 특별전 준비 참고용 인터랙티브 교재.

🌐 **사이트 주소**: `https://[GitHub 아이디].github.io/asean-study/`

---

## 📁 파일 구조

```
asean-study/
├── index.html          ← 사이트 본체 (수정 불필요)
├── README.md           ← 이 파일
└── data/
    ├── tales.json      ← 📖 아세안 동화 이야기 목록
    ├── tl.json         ← 📅 역사 연표
    ├── countries.json  ← 🗺 나라별 특징
    ├── orgs.json       ← 🏛 관련 기관
    └── quiz.json       ← ✏️ 퀴즈
```

---

## ✏️ 데이터 수정 방법 (코딩 없음)

### 동화 이야기 추가/수정 (`data/tales.json`)

1. GitHub에서 `data/tales.json` 클릭
2. 오른쪽 상단 ✏️ 연필 아이콘 클릭
3. 아래 형식으로 항목 추가:

```json
{
  "country": "베트남",
  "animals": ["용", "거북"],
  "theme": "건국신화",
  "title": "이야기 제목",
  "story": "줄거리 내용...",
  "links": [
    { "t": "링크 이름", "u": "https://..." }
  ]
}
```

4. 페이지 하단 **Commit changes** 클릭 → 1~2분 후 사이트 자동 반영

### 연표 항목 추가 (`data/tl.json`)

```json
{
  "year": "1414년",
  "era": "중세",
  "title": "말라카 왕국, 이슬람 국교 선포",
  "tag": "islam",
  "countries": ["🇲🇾 말레이시아"],
  "detail": "상세 설명..."
}
```

`tag` 값: `india` / `china` / `islam` / `europe` / `modern` / `asean`

### 기관 추가 (`data/orgs.json`)

```json
{
  "country": "🇻🇳 베트남",
  "color": "#dc2626",
  "items": [
    {
      "name": "기관명",
      "sub": "영문명 또는 부제",
      "url": "https://...",
      "note": "간단한 설명"
    }
  ]
}
```

---

## 🚀 GitHub Pages 배포 방법 (최초 1회)

1. GitHub에서 `New repository` → 이름: `asean-study`
2. 이 폴더 전체를 업로드 (또는 git push)
3. 저장소 **Settings** → **Pages** → Source: `main` 브랜치, `/ (root)` 선택 → **Save**
4. 몇 분 후 `https://[아이디].github.io/asean-study/` 접속 확인

---

## 📌 탭 구성

| 탭 | 데이터 파일 | 설명 |
|---|---|---|
| 📅 역사 연표 | `tl.json` | 문화권별·나라별 필터 |
| 🗺 나라별 특징 | `countries.json` | 11개국 카드 + 상세 모달 |
| 🌊 문화권 흐름 | (index.html 내장) | 4개 파도 + 지도 |
| 📊 비교표 | (index.html 내장) | 왕조·독립 비교표 |
| ✏️ 퀴즈 | `quiz.json` | 10문제 즉시 채점 |
| 📖 아세안 동화 | `tales.json` | 나라별·동물별 필터 |
| ✍️ 문자 이야기 | (index.html 내장) | 4파도 문자 계통도 |
| 🏛 관련 기관 | `orgs.json` | 국가별 문화기관 링크 |
