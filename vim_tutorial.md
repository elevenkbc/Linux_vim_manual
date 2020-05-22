## **Vim 指令教學 **

```shell
sudo apt-get install vim
```



**Vim** 總共有三種模式

* **command mode** (常規模式，一進入vim預設就在命令模式)

  輸入指令 vim test.txt 後就直接進入這個模式

  i  在游標處插入內容

  o 在當前行的下一行插入內容

  dd 刪除目前所在的整行內容

  yy 複製當前行的內容到緩衝區

  n+yy 複製從游標處開始n行的內容到緩衝區

  p 將緩衝區的內容貼到游標處

  / 尋找關鍵字，n鍵可找出下一個關鍵字

  : 進入EX模式

* **insert mode** (編輯模式)

  就像word一樣，隨意編輯內容，所見就是所得

  esc 返回 command mode

* **command-line mode** (存檔、離開等等)

  :w 保存當前的修改

  :w + example.txt  將當前的修改另存為 example.txt

  :q 退出vim，如果尚未保存vim會提示您需要保存

  :q!  不保存直接退出

  :sh 回到termintal

  :!  執行系統命令，在termintal 上執行單行的shell指令，輸入ctril+d 可回到vim

  : set number 顯示行號(coding 好用)

