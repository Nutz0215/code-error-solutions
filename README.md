# gitのコマンド

最新のmainブランチの状態を取り込み
```
git pull origin main
```
コミットした差分をgithubに反映
```
git push
```
ブランチ一覧と現在いるブランチの名前
```
git branch
```
ブランチの移動
```
git checkout ブランチ名
```
github上での変更の取り込み
```
git fetch
```
gitでリモートに追加されたブランチを確認する時
```
git branch -r
```
既存のリポジトリをクローンする
```
git clone <リポジトリのHTTPS URL>
```
pushするときのめも
```
git init

git add .

git commit -m "XXXXXXX"

git remote add origin https://github.com/YYYYYYY/test.git

git push origin master (git push origin main)
```
mainにmerge出来ないとき

[Errors:fatal: refusing to merge unrelated histories]
```
git merge <任意のbranch> --allow-unrelated-histories
```
pull request出来なかったとき
[Errors:There isn't anything to compare]
```
https://qiita.com/mikumikumikumiku/items/3353018c72a1bf306f21
```
## vueでのエラーについて
templateタグを用いた時の【Component template should contain exactly one root element. 】エラーの解消　
```
<div>で全体を囲む
```
## nuxtを立ち上げる際のエラー解消
"digital envelope routines"のエラーはNode.jsのバージョンに影響されたエラー
```
export NODE_OPTIONS=--openssl-legacy-provider