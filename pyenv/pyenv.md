# pyenv

## 備忘録
- Anaconda では インストールできる python のバージョンに制約がある
- pyenv も制約があるが、 Anaconda よりは 制約が緩い

# pyenv のインストール
- brew update
- brew install pyenv
- pyenv install 3.6.0
- pyenv global 3.6.0

# python のバージョンの表示
- ローカルにあるバージョン
    - pyenv versions
    - pyenv versions --bare
- インストールできるバージョン
    - pyenv install --list


# pyenvを使用してPython 3.6の仮想環境を作成する手順
- pyenv-virtualenvプラグインをインストール
    - brew install pyenv-virtualenv

- pyenvの初期化
    - echo 'eval "$(pyenv init --path)"' >> ~/.zshrc
    - echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.zshrc

- ターミナルを再起動するか、以下のコマンドを実行して初期化を反映させます。
    - source ~/.zshrc

- pyenv install 3.6.0

- 仮想環境を作成します。ターミナルで以下のコマンドを実行
    - pyenv virtualenv <Python version> <env name>
    - pyenv virtualenv 3.6.0 myenv36

- 仮想環境をアクティベートします。ターミナルで以下のコマンドを実行
    - pyenv activate myenv36


