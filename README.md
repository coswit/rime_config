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
上屏配置wubi86.custom.yaml
```
patch:
  "style/horizontal": true
  "style/inline_preedit": true  # 內嵌編碼（僅支持TSF）
  "style/display_tray_icon": false    
  "ascii_composer/switch_key/Shift_L": commit_code
  "auto_commit": true  # 切换到英文时自动上屏
  "translator/enable_user_dict": false # 关闭用户词典
  "key_binder/bindings":
    - { when: has_menu, accept: semicolon, send: 2 }
    - { when: has_menu, accept: apostrophe, send: 3 }
  
```
wubi86.schema.yaml
```
speller:
  delimiter: " ;'"
  max_code_length: 4    #四码上屏
  auto_select: true                       # 顶字上屏
  auto_select_unique_candidate: true      # 无重码自动上屏
```

