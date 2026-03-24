# 3DS Shared Font 工具集

## [3dsfont](https://github.com/dnasdw/3dsfont)

3dsfont 是一个用于 Nintendo 3DS 的字体资源工具与格式集合，提供导入/导出 3DS 字体、生成纹理图集、编辑字符映射等功能。该项目便于在汉化、替换系统或游戏字体、以及将 3DS 字体导出为通用格式时使用，适合 ROM 修改、homebrew 开发与字体资源研究。

该项目下面的 [ctr_FontConverter](https://github.com/dnasdw/3dsfont/tree/master/bin/ctr_FontConverter) 这个工具可以通过图片、字体来生成 bcfnt 的工具。

3dsfont 下面的 bcfnt2charset 用来提取 bcfnt 中的字符集。mergecharset 用来合并字符集。charset2xlor、charset2xllt、charset2xggp 用来将字符集生成 ctr_FontConverter 下面使用的 xlor、xllt、xggp 文件。

## [nintyfont](https://github.com/hadashisora/NintyFont)

一个可以查看 bcfnt 字体的任天堂字体编辑器。不过它的编辑功能还没开发，可以当作一个 bcfnt 查看器来使用。 

## [Fontendo](https://github.com/retrohead/Fontendo)

功能跟 NintyFont 一样。但它的字形导入导出功能是好用的。如果需要修改 bcfnt 的个别字形的话，推荐用它。

## [FontTool](https://github.com/astronautlevel2/FontTool)

3DS 系统字体打包工具。可以将 bcfnt 文件转换成 CIA 格式的 3DS 系统字体安装包。不过它需要调用一些其它的工具来完成工作，比如:3dstool, ctrtool, make_cia 这些工具。另外，它还需要 python 运行环境。

## [bcfntConv](https://github.com/andot/bcfntconv)

将 Nintendo 3DS 的 bcfnt 字体与模拟器使用的 shared_font.bin 相互转换，并提供将 bcfnt 打包为 3DS 可安装 .cia 的工具 bcfnt2cia（需要外部 3dstool 与 make_cia，但不需要 python 运行环境了）。所有可执行文件包括依赖的 3dstool 和 make_cia 都已经放在该项目的 bin 目录下了，可以直接下载使用。