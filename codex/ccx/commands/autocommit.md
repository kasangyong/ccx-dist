---
description: 이 폴더의 자동 commit(선택 push)을 켜고 끄거나 상태를 본다 (예: /ccx:autocommit on --push)
disable-model-invocation: true
---
사용자가 준 인자: `$ARGUMENTS`

ccx MCP 서버의 `ccx_autocommit` 도구를 한 번 호출하라. 인자는 사용자가 준 것만 옮긴다.
- 첫 낱말이 on·off·status 중 하나면 그것을 `state` 로, 없으면 `status`
- `--push` 가 있으면 `push: true`, `--allow-default-branch` 가 있으면 `allow_default_branch: true`, `--without-hooks` 가 있으면 `without_hooks: true`

돌려받은 내용을 고치지 말고 그대로 사용자에게 보여 줘라. 다른 도구는 쓰지 말고, git 명령이나 파일 수정도 하지 마라.
도구를 찾을 수 없으면 "ccx 플러그인의 MCP 서버가 실행되지 않았다. `/mcp` 에서 ccx 상태를 확인하세요."라고만 답하라.
