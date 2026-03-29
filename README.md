# php-

# 開發環境
```
VS Code
VS Code環境插件: PHP Intelephense


[伺服器]
XAMPP


```
## XAMPP

### XAMPP 故障解決方案
```
1. 管理員運行
2. 關閉本地的齊發Web服務，或佔用80/443端口的服務，例如vmware-host 服務;
3. 進入[config]文件,修改apache的默認80/443,例如80修改82, 重啟XAMPP
並管理員運行，之後訪問本地站點時，都需要加上端口號，例如
http"//localhost:82/index.pxp ;
4. 卸載之前自己安裝的apache/mysql等版本;





```






### 引入 include "sysHeader.php"

```
常見用途：

設定共用變數

連線資料庫

設定 session

HTML <head>、權限設定等
```
### 引入 require_once("fnc.php");

```
一定要成功

檔案不存在 → Fatal Error，程式直接中止

只載入一次

避免 function 重複定義錯誤

```

### isLoginFnc()
呼叫「登入檢查函式」
- 打開 fnc.php > 查看 function isLoginFnc()


## style

```
divMap {} K7-7F 地圖
divMap2 {} K5-1F 地圖
divMap3 {} K7_5FMAP
divPoint {} （異常 / 斷線）

```



### <header class="topbar">：上方導覽列（Top Bar）
```
上方黑色（或深色）導覽列

skin5：主題配色

navbar-expand-md：中尺寸以上才展開
```



### navbar-brand 左上角：Logo + 系統名稱
```
系統名稱：B3 eRack
點 Logo 會回首頁 index.php
這整套就是 B3 廠 eRack Map 監控系統
```


### nav-toggler Mobile 專用按鈕（RWD）

``` php
<a class="nav-toggler d-block d-md-none">
<a class="topbartoggler d-block d-md-none">
```

```
👉 只有在手機 / 平板才會出現
👉 用來：

展開側邊欄

展開右上選單

```

### echo sprintf 右上角：登入者資訊
``` php
<?PHP
    echo sprintf("Hi, %s", $_SESSION["idno"]);
?>
```

### dropdown-item 登出功能


```
登出不是直接跳頁

而是 JS function



通常內容會是：

function userLogout(){
    location.href = "logout.php";
}

或 AJAX 清 session。

```



