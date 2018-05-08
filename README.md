此篇教你怎用 Git 與 Github

# 你需要做的事
  - 1. 創一個 Github 帳號
  - 2. 下載 Github 桌面 ( https://desktop.github.com/ )
  - 3. 搜尋你的電腦 現在應該會有 Github 和 Git shell
  - 4. 登入 Github 後，點擊右上角的頭貼，點擊 Your Profile
  - 5. 進入後，點擊 Repositories，點擊頁面中右上方的 New
  - 6. 給一個 Repository name 後 Create repository
  - 7. 點擊一下頁面裡的連結旁邊的 SSH
  - 8. 在電腦中創造一個資料夾，創造好後開啟 Git shell 並進入此資料夾
  - 9. 輸入以下指令
```sh
git init
git commit -m 'first commit'
git remote add origin 頁面中的連結
git push -u origin master
```

