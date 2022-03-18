# 笔记

这个东西真的很难跑起来

1. 按照readme走，首先python版本不行，最新的3.10会下不了stt1.0，试了一下最后用的3.7。

2. 然后是运行main时from . import说不是什么parent。

3. 使用pycharm一顿操作后终于能运行了，就是用这个
run.sh
里面的

H:\Hworkspace\github\AutoSub\venv\Scripts\python.exe H:/Hworkspace/github/AutoSub/autosub/main.py --file tempSource/2022-03-17_22-05-12.mkv --engine=ds

4. 引擎不设ds的话它会找另一个格式的模型，不会用我下的pbmm或者scorer。设了ds就会用pbmm。

5. IDE里还要设运行文件夹为本层文件夹，否则会os.listFile的时候找不到模型。

6. 内部的文件也改了一点用来处理那个form . import
