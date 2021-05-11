[toc]

# guide
https://www.wireshark.org/docs/wsdg_html_chunked/index.html

# build win64 wireshark

## set env

```
set WIRESHARK_BASE_DIR=C:\Development
set QT5_BASE_DIR=C:\Qt\5.15.2\msvc2019_64
```
## Generate the build files
```
cd C:\Development\wsbuild64
cmake -G "Visual Studio 16 2019" -A x64 ..\wireshark
```
## build

```
msbuild /m /p:Configuration=RelWithDebInfo Wireshark.sln /t:Clean 
msbuild /m /p:Configuration=RelWithDebInfo Wireshark.sln
```



