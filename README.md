### 配置

weasel.custom.yaml中配置

```shell
# 配置水平方向；分号、单引号选择2、3键
patch:
  "style/horizontal": true
  "key_binder/bindings":
    - { when: has_menu, accept: semicolon, send: 2 }
    - { when: has_menu, accept: apostrophe, send: 3 }
```
上屏配置
```
patch:
  "style/horizontal": true
  "style/inline_preedit": true  # 內嵌編碼（僅支持TSF）
  "style/display_tray_icon": false      
  "auto_commit": true  # 切换到英文时自动上屏
```

