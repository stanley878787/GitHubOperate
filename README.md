# GitHub 常用操作

## 創建新專案 
> {name}換成專案名稱
```
echo "# {name}" >> README.md
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/jiunjiun69/{name}.git
git push -u origin main
```

## 推送新版本專案
```
git add .
git commit -m "版本名稱"
git push
```

## 下載專案
git clone <專案HTTPS連結>

## 拉取新版本專案
要先cd進去專案目錄裡面下
`git pull`

## 拉取版本有合併問題時
1. 方法一：stash
```
git stash
git pull
git stash pop
```
2. 方法二：完全覆蓋本地修改
```
git reset --hard
git pull
```

## Git 指令回顧
```
單一檔案加入索引：git add <檔案名稱>
所有檔案加入索引：git add .
提交版本：git commit -m "填寫版本資訊"
觀看當前狀態：git status
瀏覽歷史紀錄：git log
```
[Git 實用操作：重寫 Commit 歷史](https://iter01.com/525732.html)