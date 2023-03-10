# 純文字檔案的合併
這篇可以讓你知道如何使用Windows的CMD.exe合併大量的.txt、.md檔等[純文字檔案](https://zh.wikipedia.org/wiki/%E6%96%87%E6%9C%AC%E6%96%87%E4%BB%B6)。
> - 這個合併方式並不會導致原先的檔案被刪除。
> - 這個合併所另存的文件中會將不同文件間的文字首尾相連，請自行找方法將文件與文件相連的首尾換行。
> - 如果這個方法所另存的檔案效果不符合你的要求，可以嘗試使用python.exe自己客製化導出想要的樣子。


## 步驟
> [ ___ ]：指的是要照文字說明修改的地方，修改後不用加上中括號"[ ]"。

### 前置作業
1. 將欲合併的檔案堆放在一個資料夾中，並將此資料夾的路徑複製下來。
2. 打開CMD.exe，輸出`cd [剛才複製的資料夾路徑]`。

### 合併方法（一）
在CMD.exe中輸出`copy *.[欲合併檔案堆的副檔名] [另存後欲取的檔名].[另存後欲要取的副檔名]`。

### 合併方法（二）
在CMD.exe中輸出`type *.[欲合併檔案堆的副檔名] > [欲另存檔案的路徑]/[另存後欲取的檔名].[另存後欲要取的副檔名]`。
> 這方法中，[欲另存檔案的路徑]不能與原先存放檔案堆的資料夾路徑相同，不然會進入複製迴圈。


## 參考資料
1. https://a102302301.pixnet.net/blog/post/4404099-%E5%88%A9%E7%94%A8%E5%91%BD%E4%BB%A4%E6%8F%90%E7%A4%BA%E5%AD%97%E5%85%83%E5%90%88%E4%BD%B5%E5%A4%9A%E5%80%8Bcsv.%E6%AA%94
2. https://juejin.cn/post/7103422838572318757
