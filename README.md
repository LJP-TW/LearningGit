此篇教你怎用 Git 與 Github

# 你需要做的事
  - 1. 創一個 Github 帳號
  - 2. 下載 Github 桌面 ( https://desktop.github.com/ )
  - 3. 搜尋你的電腦 現在應該會有 Github 和 Git shell
  - 4. 登入 Github 後，點擊右上角的頭貼，點擊 Your Profile
  - 5. 進入後，點擊 Repositories，點擊頁面中右上方的 New
  - 6. 給一個 Repository name 後 Create repository
  - 7. 在這個 repository 創造一個文件 README.md ( 副檔名不是 .txt 就是 .md) 並在裡面寫一點咚咚
  - 8. 在電腦中創造一個資料夾，創造好後開啟 Git shell 並進入此資料夾
  - 9. 在 Git shell 中輸入以下指令
```sh
git init
git add README.md
git commit -m 'first commit'
git remote add origin 頁面中的連結
git push -u origin master
```

# 基礎指令介紹

## 講在前頭 : Google hen 好用
遇到不懂的 git 指令，只要在 Google 搜尋 'git ...' (... 放你要查的指令)
都能查到這個指令的用法，所以以下介紹如果看完想了解更多，就Google + 練習吧

## 直接讀手冊也 hen 有用
你也可以使用
```sh
git help <你不懂的command>
```
來叫出那個command的使用手冊來看

### git init
這是要進行版本控制的第一個步驟，只要到你要版控的資料夾(專案)下這個指令
這個資料夾就開始使用版控了

### git add <Filename>
當你想要追蹤著你資料夾裡的某個新咚咚
或是你資料夾裡的某個咚咚更新了
都需要下這個指令

### git commit -m 'some message'
當你 git add 很多次後，終於你的專案告一個段落，一個版本完成了
此時就可以下此指令，-m 這個參數後面要緊接一些訊息，這個訊息最好是能一看就知道說這個版本對專案做了啥事
比如說 'Update Readme.md' 或是 'Adding myClass.cpp' 之類的

### git remote add origin <url>
這個指令是拿來設定遠端伺服器位置的，只要下一次後，之後 push 都會 push 到指定的 url 去
並且我們新增了一條分支叫做origin，用來代表遠端伺服器

### git push -u origin master
push 就是把我們本機當前版本更新到遠端伺服器
-u 是一個參數，詳情見手冊
後面兩個分別是遠端(push的目的地) 和 本機(push的來源地)
master 就是代表本機上的 '主幹'