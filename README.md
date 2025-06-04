# KakaoTalk-Notice-Summary-Bot

# 카카오톡 공지사항 자동화 시스템

이 프로젝트는 카카오톡 채팅방의 공지사항을 자동으로 수집하고 분석하여 요약하는 시스템입니다.

## 주요 기능

- 카카오톡 채팅방에서 공지사항 자동 수집
- GUI 자동화 및 파일 내보내기 방식 지원
- 수집된 공지사항 자동 분류 및 요약
- 데이터 백업 및 관리

## 프로젝트 구조

```
Scraper/
├── core/                 # 핵심 로직
│   ├── extractor.py      # 추출기 메인 클래스
│   └── config.py         # 환경설정 관리
│
├── modules/
│   ├── gui/              # GUI 자동화 관련
│   ├── parser/           # 채팅 파싱 관련
│   └── io/               # 입출력 관리
│
├── data/                 # 데이터 저장소
│   ├── raw/             # 원본 데이터
│   └── processed/       # 처리된 데이터
│
└── logs/                # 로그 파일
```

## 설치 방법

1. 의존성 설치:
```bash
python requirements_install.py
```

2. 설정 파일 수정:
- `config.ini` 파일에서 채팅방 이름과 백업 경로 등을 설정

## 사용 방법

1. 메인 실행:
```bash
python main.py
```

2. 설정 옵션:
- `CHAT_ROOM_NAME`: 대상 카카오톡 채팅방 이름
- `BACKUP_DIR`: 데이터 백업 경로
- `OUTPUT_ENCODING`: 출력 인코딩 설정

## 주요 기술 스택

- Python 3.x
- pyautogui: GUI 자동화
- pandas: 데이터 처리
- scikit-learn: 머신러닝
- transformers: 자연어 처리
- tensorflow: 딥러닝

## 라이선스

이 프로젝트는 MIT 라이선스를 따릅니다.
