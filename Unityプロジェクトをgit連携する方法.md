.gitignoreを配置

https://github.com/spoiledcat/git-for-unity を参考にgitをパッケージに追加

git for Unity の Repository Configration にリポジトリを指定する
git@github.com:LawrenceTurnerW/~~~.git

ローカルにmainブランチを作成して--set-upstream-to でつなげる
git branch --set-upstream-to=origin/main main

initした際にできるgitignoreがコンフリクトしないようにローカルのgitignoreを消してcommit
git rm .gitignore
git commit -m "gitignoreを削除"

ローカルにマージする
git merge --allow-unrelated-histories origin/main
