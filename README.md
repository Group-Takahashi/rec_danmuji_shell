哔哩哔哩录播姬运行脚本<br>
文件在Windows编辑过 Windows每一行结尾是\n\r Linux是\n<br>
文件中行尾的\r替换为空白<br>
```
sed -i 's/\r$//' rec
sed -i 's/\r$//' rec_run
```
rec -> 手动设定房间号，不读取配置文件，文件保存位置由脚本决定（注：因为未知原因，在ubuntu desktop中录播文件无法保存在录播姬工作目录外，所以无论脚本所设定的目录是什么，都会在工作目录按照脚本设定新建文件夹 例：脚本设定的目录为/opt/bili/files，文件保存路径为：工作目录/opt/bili/files）<br>
rec_run -> 读取配置文件运行，文件将保存在config.json所在目录，脚本中指定的路径为配置文件所在目录

## 路径

rec-> /
rec_run-> /

## 运行

任意目录<br>
```
/rec
or
/rec_run
```
