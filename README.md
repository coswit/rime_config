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

