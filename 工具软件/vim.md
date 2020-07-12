# vim 中方向键和 Home End 键不能用

## 修改 ~/.vimrc 增加按键绑定

https://github.com/microsoft/WSL/issues/1154#issuecomment-595951533

```shell
set <Up>=^[[A
set <Down>=^[[B
set <Right>=^[[C
set <Left>=^[[D
set <Home>=^[[H
set <End>=^[[F
```

但是，仍会导致不同 bash 下不同的按键码导致的方向键失效问题。
