**Ubuntu 基本Shell指令**

使用快捷鍵 `Ctrl` + `Alt` + `T` 來開啟 Terminal

顯示當前所在目前路徑下的所有的檔案或資料夾

``` shell
ls
```

列出目前路徑下的所有檔案與資料夾的詳細資訊，時間、容量等等

``` shell
ls -l
```

清除當前所有的command 紀錄

``` shell
clear
```

關閉Terminal 

``` shell
exit
```

移動到使用者目錄

``` shell
cd 
```

移動到另一資料夾

``` shell
cd /要移動到的資料夾
```

移動到目前目錄的上一層

``` shell
cd ..
```

移動到根目錄

``` shell
cd /
```

移動到 HOME 目錄

 ```shell
cd ~
 ```

列出目前所在的目錄

``` shell
pwd
```



**Vim 指令教學 **

vim 總共有三種模式

1. 命令模式(常規模式，一進入vim預設就在命令模式)

   i  在游標處插入內容

   o 在當前行的下一行插入內容

   dd 刪除目前所在的整行內容

   yy 複製當前行的內容到緩衝區

   n+yy 複製從游標處開始n行的內容到緩衝區

   p 將緩衝區的內容貼到游標處

   / 尋找關鍵字，n鍵可找出下一個關鍵字

   : 進入EX模式

2. 插入模式(編輯內容)

   就像word一樣，隨意編輯內容，所見就是所得

   esc 返回命令模式

3. EX模式(存檔、離開等等)

   :w 保存當前的修改

   :w + example.txt  將當前的修改另存為 example.txt

   :q 退出vim，如果尚未保存vim會提示您需要保存

   :q!  不保存直接退出

   :sh 回到termintal

   :!  執行系統命令，在termintal 上執行單行的shell指令，輸入ctril+d 可回到vim

   : set number 顯示行號(coding 好用)

   

**在Ubuntu 上編譯 C++ 程式的方法**

使用快捷鍵 `Ctrl` + `Alt` + `T` 來開啟 Terminal

1. 安裝g++編譯器

   ``` sh
   sudo apt-get install g++ build-essential
   ```

2. 假設我們的C++檔案檔名為 example.cpp，執行以下命令可以編譯example.cpp檔，並且產生一個能被執行的example.out檔案

   ``` shell
   g++ /home/......../example.cpp -o /home/......./example.out -Wall
   ```

3. 接著移動到 example.out 的資料夾路徑下，輸入以下語法來觀察程式結果

   ```shell
   ./example.out
   ```
