# ubuntu 中執行 .sh 檔案的幾種方法
首先寫一個簡單的 test.sh 檔案

```shell
#!/bin/bash
read -p "Please input your first name:" firstname
read -p "Please input your last name:" lastname
echo -e "\nYour full name is: $firstname $lastname"
```



### 1. 使用 sh 執行 test.sh

強制使用 sh 這種 shell 來執行 **test.sh**

```shell
sh test.sh
```

### 2. 使用 bash 執行 test.sh

用 **/bin/bash** 來執行 **test.sh** 這個檔案

```shell
bash test.sh
```

### 3. 使用 . 來執行

這種方式執行 .sh檔案，需要先新增可執行的許可權，ls 觀看檔名變成綠色(可執行)

```shell
chmod +x test.sh
```

取消可執行權限

```shell
chmod -x test.sh
```

### 4. 使用 source 執行 (python 虛擬環境常用)

使用 source 指令也能夠執行 .sh檔案

```shell
source test.sh
```
