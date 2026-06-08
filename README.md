# Minimal Media Journal

GitHub Pages용 미니멀 감상 기록 페이지입니다.

## 파일 구조

```text
index.html
reviews.md
```

두 파일을 같은 폴더에 둡니다. `index.html`이 `reviews.md`를 읽어서 한 페이지에 최대 5개 항목씩 출력합니다.

## reviews.md 형식

각 항목은 아래 형식으로 작성합니다.

```md
---
id: unique-id
platform: Steam
consumed_date: 2026-06-01
review_date: 2026-06-09
recommend: yes
title: 제목
---
본문을 여기에 작성합니다.

===
```

항목과 항목 사이에는 `===`를 한 줄로 넣습니다.

## recommend 값

- `yes` 또는 `추천` → 추천
- `no` 또는 `비추천` → 비추천
- `mixed`, `neutral`, `보류`, `중립` → 보류

## 로컬 미리보기

브라우저에서 파일을 더블클릭하면 `fetch()` 제한 때문에 `reviews.md`를 못 읽을 수 있습니다.

```bash
python -m http.server 8000
```

그다음 브라우저에서 아래 주소를 엽니다.

```text
http://localhost:8000
```
