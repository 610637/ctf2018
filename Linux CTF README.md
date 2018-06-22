linux 解題

你知道如何 安全連線到 遠端伺服器嗎?

```
使用ssh連線至120.114.62.48 Port:2200 ===> ssh lab@120.114.62.48 -p 2200

  列出當前目錄底下的檔案與子目錄 ===> ls

  檢視flag檔案內容 ===> cat flag
```


你知道如何在Linux上找到隱藏檔案嗎?

```
列出當前檔案與目錄==> ls

顯示檔案與目錄的詳細資訊==> ls -l

顯示所有檔案與目錄的詳細資訊==> ls -al
```

你知道如何 在Linux上做hex to string嗎

```
列出當前檔案與目錄==> ls

檢視hex.txt檔案內容==>cat hex.txt

使用xxd工具將hex.txt的16進位內容轉換為字串==>xxd -r -p hex.txt
```

你知道如何 在Linux上做base64 解碼嗎?
```
列出當前檔案與目錄==> ls

檢視base64.txt檔案內容 ==> cat base64.txt

使用base64工具將base64.txt的內容解碼==>base64 -d base64.txt
```

你知道如何 找到 secret秘密檔案嗎?
```
不知道
```

你知道如何找到Linux執行的服務嗎?
```
列出當前系統正在執行的Process ==> ps aux

解法一:執行flag程式 ==>/bin/flag

解法二: nc 127.0.0.1 2111

socat TCP-LISTEN:2111,reuseaddr,fork EXEC:/bin/fl
```
你知道如何找到Linux正在執行的網路服務嗎?
```
列出當前系統正在執行的網路服務 ==> netstat -ano

==> 取得http://127.0.0.1/的網頁內容
==> curl http://127.0.0.1/
```

你知道如何在Linux下載並解壓縮ForYou檔案嗎?
```
在tmp目錄下建立學號目錄 ==> mkdir /tmp/610637

==> cd /tmp/404050

下載遠端網站伺服器的ForYou.tar.gz壓縮檔  ==> wget http://120.114.62.39/ForYou.tar.gz

列出當前檔案與目錄 ==> ls
  
解壓縮ForYou.tar.gz檔案 ==> tar zxvf ForYou.tar.gz
    
查看ForYou檔案類型  ==> file ForYou
      
檢視ForYou檔案內容  ==> cat ForYou
```

你知道如何下載TobeExe檔案並讓他執行嗎?

```
進入tmp目錄下的學號目錄  ==> cd /tmp/610637

下載遠端網站伺服器的TobeExe檔案 ==> wget http://120.114.62.39/TobeExe

查看TobeExe檔案類型 ==> file TobeExe

賦予TobeExe檔案執行權限 ==> chmod +x TobeExe

執行TobeExe檔案 ==> ./TobeExe
```

只有執行檔你如何顯示重要資訊?

```
進入tmp目錄下的學號目錄 ==> cd /tmp/610637

下載遠端網站伺服器的reverse檔案 ==> wget http://120.114.62.39/reverse
 
查看reverse檔案類型 ==> file reverse
  
賦予reverse檔案執行權限  ==> chmod +x reverse

執行reverse檔案  ==> ./reverse

過濾reverse執行檔內的"flag"字串  ==> strings reverse | grep flag
  
過濾reverse執行檔內的"CTF"字串  ==> strings reverse | grep CTF
```
