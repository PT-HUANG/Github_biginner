# git指令筆記都先放在這邊
#初始化 git init

#結束 rm -r .git (刪除.git檔案的意思)

#查看狀態 git status

#歷史紀錄 git log 或 git log --oneline (簡短呈現)

#要忽略的檔案(資料夾) vim .gitignore 輸入要忽略的檔名(檔案名稱底下要多一行空格)

#加入版本控制 git add <file> 或 git add . (全選的意思)

#取消加入版本控制 git rm --cached <file> 或 git reset -- <file>

#復原修改的檔案 git checkout -- <file> 或是 git restore <file>
  
#復原刪除的檔案 git checkout <file> 

#更新版本 
  

git commit (會跳到vim編輯器裡面，要新增關於版本的敘述) 
  

或是使用 git commit -m "關於版本的敘述內容"


或是使用 git commit -am "關於版本的敘述內容" 但不會把新增的檔案加入版本控制


如果要連新增的檔案也加入版本控制

git add .

git commit -am "關於版本的敘述內容"

#更改 commit message git commit --amend

#回到上一個commit的狀態 

git reset HEAD^ --hard (不保留更改的內容)

git reset HEAD^ --soft (保留commit前更改的內容，系統預設為soft可不加)

#回到之前的版本 git checkout <版本號>

#開新branch git branch <branch的名稱>

#修改branch的名稱 切換到要修改的branch  git branch -m <新的名稱>

#查看目前的branch狀況 git branch -v

#刪除branch git branch -d <branch的名稱>

#切換branch git checkout <branch的名稱> (會自動切換到最新版本)

#抓取遠端的branch git checkout <遠端的branch>

#創建分支，並切換過去 git checkout -b <new_branch>

#合併branch git merge <branch的名稱>   (將<branch的名稱>合併進來)

#當出現 conlict 提示時表示兩個相同檔案存在衝突，可以用 git status 查看是哪個檔案

使用vim 編輯檔案修正完成後再一次commit，將原本的branch刪除 git branch -d <branch的名稱> 即完成branch的合併

#上傳新版本至github git push origin main
  
#將github上的版本抓到電腦裡面 git pull origin main 

#將別人的repository抓到電腦裡面 git clone <複製的SSH網址> (但是更改後不能上傳)

#將別人的repository複製到自己的github頁面 在github上選擇 fork 接著 git clone <複製的SSH網址> (更改後可上傳)

#建立新的Branch後上傳 git push origin <新的Branch名稱>

#Github上可以直接使用Merge的功能，Merge後抓下來記得要刪除本機原來的新Branch









