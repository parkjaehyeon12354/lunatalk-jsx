# lunatalk-jsx

[LUNATALK](https://lunatalk.chat) 채팅 답변 안에 들어가는 작은 화면(JSX 에셋)을 만드는 저장소입니다.
호감도 막대, 상태창, 선택지 버튼, 폰·메신저 화면 같은 위젯을 HTML·SVG·JavaScript(React 포함)로 만듭니다.

- 공식 설명서: https://lunatalk.chat/jsx_guide
- 오픈 공지: https://lunatalk.chat/b/v/notice/523
- 등록 위치: 마이페이지 → 내 콘텐츠 → 내 에셋

## 구조

```
.claude/skills/   Claude Code 스킬 (디자인·코드 품질)
.mcp.json         Playwright MCP — 위젯을 브라우저로 띄워 화면 확인
CLAUDE.md         LUNATALK JSX 규칙 요약 (작업할 때 먼저 읽는 파일)
```

위젯 소스는 에셋 하나당 폴더 하나로 둡니다. 등록은 LUNATALK 편집기에서 코드를 붙여 넣어 합니다.

## 스킬

| 스킬 | 용도 |
|---|---|
| `ui-ux-pro-max` | 스타일·색·글꼴·UX 규칙 검색 |
| `taste-skill` | 밋밋한 AI 디자인을 피하는 프런트엔드 규칙 |
| `ponytail*` | 최소한의 코드로 끝내기, 리뷰·감사 |

가져온 스킬의 라이선스는 [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md) 에 있습니다.

## 시험하는 법

미리보기에서는 `LT` 함수가 가짜로 동작합니다. `LT.sendToAI`, `LT.setValue` 같은 실제 동작은 채팅방에서만 확인할 수 있습니다.
로컬에서는 `LT` 를 흉내 낸 가짜 객체를 붙여 Playwright 로 화면을 확인합니다.
