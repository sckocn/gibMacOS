Py2/py3 script that can download macOS components direct from Apple

Can also now build Internet Recovery USB installers from Windows using [dd](http://www.chrysocome.net/dd) and [7zip](https://www.7-zip.org/download.html).

Thanks to:

* FoxletFox for [FetchMacOS](http://www.insanelymac.com/forum/topic/326366-fetchmacos-a-tool-to-download-macos-on-non-mac-platforms/) and outlining the URL setup
* munki for his [macadmin-scripts](https://github.com/munki/macadmin-scripts)
* timsutton for [brigadier](https://github.com/timsutton/brigadier)
* wolfmannight for [manOSDownloader_rc](https://www.insanelymac.com/forum/topic/338810-create-legit-copy-of-macos-from-apple-catalog/) off which BuildmacOSInstallApp.command is based

gibmacos那个makeinstall需要win7以上系统，也就是说需要版本号9600，即win8，win10 64位为佳。win764位我试过，不行，提示需要更高版本系统。
“小偏方”：
1. 编辑Makeinstall.py 的行12 9600 改成win7 64bit 的7601（我直接改成7600）
2. 偶尔会报这个ddrelease64 错误，直接http://www.chrysocome.net/downloads/ddrelease64.exe 下载下来安装
3. 拔掉U盘，再插上，按“D”重新识别U盘。
