# PlantUML.js

PlantUML that works completely on the browser without needing a server.

Demo URL: [https://plantuml.github.io/plantuml.js/](https://plantuml.github.io/plantuml.js/)

![plantuml javascript](demo.png "PlantUML javascript")

See `examples/` for how to integrate

# Features of the editor

- Auto-rendering

- Image part is pan and zoomable

- Editor part is resizable

- Load from examples

- Ability to send the link with example loaded

## Local development

`npx http-server`

# Sample

```plantuml
@startuml
start

:ユーザーがログイン画面を開く;
:ユーザーがIDとパスワードを入力;

if (認証成功?) then (yes)
  :ユーザーのダッシュボードを表示;
else (no)
  :エラーメッセージを表示;
  stop
endif

:ユーザーがオプションを選択;
if (オプションA?) then (yes)
  :オプションAの処理を実行;
else (no)
  if (オプションB?) then (yes)
    :オプションBの処理を実行;
  else (no)
    :デフォルトの処理を実行;
  endif
endif

stop
@enduml
```
