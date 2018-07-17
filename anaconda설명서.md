# Anaconda2

가상환경 셋팅
```
$ conda create -n simvenv_1.0.0 python=2.7
```
가상환경 활성화
```
$ source activate simvenv_1.0.0
```
가상환경 비활성화
```
$ source deactivate simvenv_1.0.0
```
현제 활성화된 가상환경 보기
```
$ conda info --envs
```
```shell
sim@MacSoon : ~ $ source activate simenv_1.0.0 && conda info --envs
# conda environments:
#
base                     /Users/sim/anaconda2
simenv_1.0.0          *  /Users/sim/anaconda2/envs/simenv_1.0.0

(simenv_1.0.0) sim@MacSoon : ~ $
```

Install package from specific source
```
$ conda install --channel $URL $PACKAGE_NAME
$ pip install --index-url $URL $PACKAGE_NAME
```
```shell
(simenv_1.0.0) sim@MacSoon : ~ $ conda install --channel https://conda.anaconda.org/menpo opencv3
```
Search available packages
```
$ conda search pygame
$ pip search pygame
```
Install a package
```
$ conda install pygame
$ pip install pygame
```
Update a package
```
$ conda update --name pygame
$ pip install --upgrade pygame
```
Uninstall a package
```
$ conda remove --name pygame
$ pip uninstall pygame
```

가상환경 패키지목록을 파일로 저장
```
$ conda env export -f myvenv.txt
```
패키지목록 파일로부터 환경 셋팅
```
$ conda env create -f myvenv.txt
```
파일안에는 가상환경이름까지 저장되어있음.
