# git指令筆記都先放在這邊
git 指令筆記

初始化 git init

結束   rm -r .git 刪除.git檔案的意思

查看狀態 git status

要忽略的檔案(資料夾)
vim .gitignore 將要忽略的檔案名稱輸入進去即可完成

加入版本控制 git add <file> or git add . (全選的意思)

取消加入版本控制 git rm --cached <file>

將檔案回復到存檔之前的狀態 git resotre <file>

更新版本 git commit (會跳到vim編輯器裡面，要新增關於版本的敘述)

或是使用 git commit -m "關於版本的敘述內容"

或是使用 git commit -am "關於版本的敘述內容" 但不會把新增的檔案加入版本控制

如果要連新增的檔案也加入版本控制

git add .

git commit -am "關於版本的敘述內容"

歷史紀錄 git log  git log --oneline 簡短呈現

回到之前的版本 git checkout <版本號>

回到這個Branch的最新版本 git checkout master

開新branch git branch <branch的名稱>

查看目前的branch狀況 git branch -v

刪除branch git branch -d <branch的名稱>

切換branch git checkout <branch的名稱>

合併branch git merge <branch的名稱>   **將<branch的名稱>合併進來**

當出現 conlict 提示時表示兩個相同檔案存在衝突，可以用 git status 查看是哪個檔案

使用vim 編輯檔案修正完成後再一次commit，將原本的branch刪除 git branch -d <branch的名稱> 即完成branch的合併













