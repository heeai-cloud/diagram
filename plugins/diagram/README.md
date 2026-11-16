# 희림 다이어그램 for Claude

Claude 채팅·Cowork·Claude Code에서 희림 사내 «사이트 다이어그램 생성기»의 대지분석 다이어그램을 주소와 반경으로 만들고 대화로 SVG를 고칩니다.

- 명령: `/diagram 강남역 반경 500m 건축물 용도` (Claude Code는 `/diagram`, Cowork는 `/diagram:diagram`, 채팅에서는 그냥 말해도 됩니다)
- 연결: 커넥터 주소는 `https://diagram.heeai.cloud/mcp`입니다. 연결할 때 heeai.cloud 로그인 화면이 뜹니다(희림 아이디, 사내 도구 대문과 같은 아이디).
- 지역: 한국 전역, 두바이
- 주고받는 곳: diagram.heeai.cloud 한 곳입니다. 찾은 주소와 만든 도판은 희림 사내 서버에 저장됩니다. Claude Code에서는 도판 파일(SVG·PNG)을 작업 폴더에 내려받을 때 curl을 씁니다.
- 설치 안내: https://diagram.heeai.cloud/claude/ (희림 아이디로 로그인해서 엽니다)

© HeeAI. All rights reserved.
