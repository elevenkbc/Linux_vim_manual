## **Linux (Ubuntu) 基本Shell指令**
使用快捷鍵 `Ctrl` + `Alt` + `T` 來開啟 Terminal

顯示當前所在目前路徑下的所有的檔案或資料夾

``` shell
ls
```

列出目前路徑下，所有檔案(包含隱藏文件與檔案)

```shell
ls -a
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

創建一個新的folder名稱為 **test**

```shell
mkdir test
```

刪除 **test** 資料夾

```shell
rmdir test/
```

刪除一個文件

```shell
rm data1.txt
```

刪除多個文件

```shell
rm data1.txt data2.txt
```

刪除 **test** 資料夾，並且刪除其中所有的文件

```shell
rm -r test/
```

移動 **data.txt** 到一個檔案到 **f** 資料夾中(相對路徑)，注意當下路徑需要有 **f** 資料夾

```shell
mv data.txt ./f/
```

檔案改名，**data.txt** 改成 **data2.txt**

```shell
mv data.txt data2.txt
```

安裝軟體，安裝 **vim** 文字編輯器

```shell
sudo apt－get install vim
```

查看 **kernel** 版本

```shell
uname -a
```



1. 

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
