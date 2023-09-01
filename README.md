# nativefier-weread
自用 nativefier 构建 weread

```shell
docker run --rm -v /Users/sykoh/Desktop/weread:/target/ nativefier/nativefier --name "weread" --icon /target/book.icns --platform mac --arch x64 https://weread.qq.com/ /target/
```

挂载 /Users/sykoh/Desktop/weread 到 target 的目的，只是为了读取其中的 icns 图标文件，无其他用途

-----

----- official? sample commands -----

```shell
docker run --rm -v 
~/my-icons-folder/:/src -v 
$TARGET-PATH:/target nativefier/nativefier 
--icon /src/icon.png 
--name whatsApp 
-p linux 
-a x64 https://web.whatsapp.com/ /target/
```
```shell
docker run --rm -v 
~/nativefier-apps:/target/ nativefier/nativefier 
https://mail.google.com/ /target/
```