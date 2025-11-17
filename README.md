# ns-3-leo sim

## Install ns-3
https://www.nsnam.org/docs/installation/html/overview.html<br>
去把依賴裝一裝, 我因為要用 `ns-3-leo` 所以把版本回退到 `3.35`<br>
我是照著 `3.45` 的依賴弄, 具體裝了什麼我也不知道

```
git clone https://gitlab.com/nsnam/ns-3-dev.git -b ns-3.35
cd ns-3-dev
```

## Add module ns-3-leo
From https://github.com/dadada/ns-3-leo

`ns-3.35` 是最後一個使用 `./waf` 建構的版本
```
cd src
git clone https://github.com/runnywolf/leo.git
cd ..
./waf configure --enable-examples
./waf
```

編譯成功後會顯示：
```
Waf: Leaving directory `.../ns-3-dev/build'
Build commands will be stored in build/compile_commands.json
'build' finished successfully (...)

Modules built:
*****   *****             *****
*****   leo (no Python)   *****
*****   *****             *****

...
```
