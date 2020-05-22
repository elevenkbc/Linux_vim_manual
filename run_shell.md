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

