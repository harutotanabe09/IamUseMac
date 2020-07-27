### :green_book: Mac Install

### Shell

```sh
# シェル確認
echo $SHELL
# 使えるシェル確認
cat /etc/shells
# シェル変更
chsh -s /bin/bash
```

### iTerm

```sh
▼　色設定
iTerm2 -> Performance -> Profile -> Colors -> Color Presets でインストールしたテーマ適用

▼　画面設定
iTerm2 -> Preferences -> Profiles -> Window -> Settings for New Windows -> Style, Screen, Space
Style：FullScreen
Screen：Screen with Cursor
Space: All Space

▼　ホットキー
iTerm2 > Preferences > Keys > HotKey > Show/hide iTerm2 with a system-wide hotkeyにチェック
HotKey: のテキストボックスを選択しRecording状態になったら任意のショートカットを入力

▼　ショットカートキー
https://qiita.com/0084ken/items/8aefabef4fd3cfdf8fce

```

### zsh

```sh
# 設定ファイル
vi ~/.zshrc

### 設定後
harutotanabe@HarutonoMacBook-Air [~/Desktop/git] % ls

以下を追加し、一度プロンプトを落として、再度立ち上げる
------------------------------------------
# 色を使用
autoload -Uz colors ; colors

# パスを追加したい場合
export PATH="$HOME/bin:$PATH"

# cdした際のディレクトリをディレクトリスタックへ自動追加
setopt auto_pushd

# ディレクトリスタックへの追加の際に重複させない
setopt pushd_ignore_dups

# cdコマンドを省略して、ディレクトリ名のみの入力で移動
setopt auto_cd

# コマンドのスペルチェックをする
setopt correct

# 基本設定
HISTFILE=$HOME/.zsh-history
HISTSIZE=100000
SAVEHIST=1000000

# ヒストリーに重複を表示しない
setopt histignorealldups

# すでにhistoryにあるコマンドは残さない
setopt hist_ignore_all_dups

# コマンドプロンプトの表示形式変える
PROMPT='%F{magenta}%B%n%b%f@%F{blue}%U%m%u%f %F{green}[%~]%f %# '

```

### Git

```sh
# 鍵作成
ssh-keygen -t rsa
※　鍵ファイルを保存するフォルダの名前を１回目で聞かれるので変える

# 備考
id_rsaファイルが秘密鍵
id_rsa.pubファイルが公開鍵

# 鍵登録
ssh-add -K ~/.ssh/github
```

### アプリ

```sh
# スクリーンショット
MonoSnap

# IDE
googleIDE

# Remote Desktop
Remote Desktop Windows

# SQL Editor
dbeaver

### 便利ショートカート
control + Shift + F

```
