# Dcoker についてまとめる

## 備忘録
- 23/07 mps は gpus で現在指定できない 
    - macOS の場合, anaconda や pyenv で環境構築して gpu を指定するのが現状ベスト


# docker run 例 (mps は gpus で現在指定できない error を出す 23/07)
- latest 
    - docker run  -v $(pwd):$(pwd) -w $(pwd) -it -d --gpus all --name container_name python:latest /bin/bash
    - docker run  -v $(pwd):/workspace -it -d --gpus all --name container_name python:latest /bin/bash


# knowledge
- python version
    - https://hub.docker.com/_/python


# 参考
- https://qiita.com/satotka/items/e1851799bcaf44a11763
    - $ docker run -it --rm --name console --user `id -u`:`id -g` --volume `pwd`:`pwd` --workdir `pwd` <image> bash



