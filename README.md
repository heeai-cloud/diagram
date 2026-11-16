# 희림 다이어그램 for Claude

희림 사내 «사이트 다이어그램 생성기»(diagram.heeai.cloud)를 Claude에서 쓰는 플러그인입니다. 장소와 반경을 말하면 대지분석 다이어그램을 그리고 대화로 SVG를 고칩니다.

로그인은 heeai.cloud 희림 아이디로 합니다. 희림 아이디가 없으면 쓸 수 없습니다.

## Claude 앱(채팅·Cowork)

1. 사용자 지정 → 플러그인(Customize → Plugins)에서 «추가 → 마켓플레이스 추가»(Add marketplace)를 누릅니다.
2. 저장소 칸에 `heeai-cloud/diagram`을 넣습니다.
3. 목록에 나온 diagram을 추가한 다음 커넥터(Connectors) 탭에서 «연결»을 누르고 희림 아이디로 로그인합니다.

Claude를 회사 조직 계정으로 쓰면 조직 관리자가 커넥터 주소 `https://diagram.heeai.cloud/mcp`를 먼저 넣어 두어야 «연결»이 눌립니다.

## Claude Code

```
claude plugin install diagram --marketplace heeai-cloud/diagram
```

설치한 다음 `/mcp`에서 diagram을 골라 로그인합니다.

## 쓰는 법

- `/diagram 강남역 반경 500m 건축물 용도` (Cowork는 `/diagram:diagram`, 채팅에서는 그냥 말해도 됩니다)
- 지역: 한국 전역, 두바이
- 자세한 안내: https://diagram.heeai.cloud/claude/ (희림 아이디로 로그인해서 엽니다)

## 주고받는 곳

diagram.heeai.cloud 한 곳입니다. 찾은 주소와 만든 도판은 희림 사내 서버에 저장되고 Claude 대화 내용은 받지 않습니다. Claude Code에서는 도판 파일(SVG·PNG)을 작업 폴더에 내려받을 때 curl을 씁니다.

© HeeAI. All rights reserved.
