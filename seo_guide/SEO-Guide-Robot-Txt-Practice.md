# robot.txt做法

## 對敏感的內容使用更為安全的方法

您或許對使用 robots.txt 來封鎖敏感或機密資料感覺不是特別放心。其中一個原因是，如果網際網路上碰巧存在連至您封鎖網址的連結 (例如參照記錄)，則搜尋引擎仍然可以參照該網址 (只是顯示網址，而不顯示標題或摘要)。

此外，一些不符合條件的搜尋引擎或惡意搜尋引擎並不遵守「漫遊器排除標準」，可能會違背您的 robots.txt 指示。最後，好奇的使用者可能會查看您 robots.txt 檔案中的目錄或子目錄，並猜中您不想曝光的內容網址。對內容加密或使用 .htaccess 對內容進行密碼保護是更安全的選擇。

***請避免 :***

> 允許檢索類似搜尋結果的網頁(使用者不喜歡從一個搜尋結果網頁進入另一個搜尋結果網頁，這對他們而言沒有多大價值)

> 允許檢索大量自動產生的且內容相同或稍有不同的網頁:「難道這100,000個近乎相同的網頁真的應該在搜尋引擎的索引中出現嗎？」

> 允許檢索因Proxy服務而建立的網址

## 參考資料

* [Google 搜尋引擎最佳化 初學者指南](http://static.googleusercontent.com/external_content/untrusted_dlcp/www.google.com.hk/zh-TW/hk/intl/zh-TW/webmasters/docs/search-engine-optimization-starter-guide-zh-tw.pdf)
* [robots.txt 產生器](http://googlewebmastercentral.blogspot.tw/2008/03/speaking-language-of-robots.html)
* [robots.txt 檔案](https://support.google.com/webmasters/answer/6062608?hl=zh-Hant&rd=1)
* [每種網址封鎖方法的注意事項](http://googlewebmastercentral.blogspot.tw/2008/01/remove-your-content-from-google.html)
