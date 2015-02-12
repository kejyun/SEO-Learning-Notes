# robot.txt 說明

## 使用robots.txt限制搜尋引擎對無需檢索的部分進行檢索

「robots.txt」檔案可告知搜尋引擎是否可以存取您網站的某些部分，進而對這些部分進行檢索 (1)。

![robots.txt 資料內容](http://i.imgur.com/5QcYKZV.png)

這個檔案必須命名為「robots.txt」，並放置在您網站的根目錄中(2)。

![robots.txt 檔案位置](http://i.imgur.com/olgY5dE.png)


您可能不希望搜尋引擎檢索網站中的某些網頁，因為這些出現在搜尋結果中的網頁，對使用者而言並無益處。如果您確實想阻止搜尋引擎檢索您的網頁，「Google網站管理員工具」中有一個很好用的 [robots.txt 產生器](http://googlewebmastercentral.blogspot.tw/2008/03/speaking-language-of-robots.html)，可協助您建立這個檔案。請注意，如果您的網站使用了子網域，且您不希望搜尋引擎檢索特定子網域中的某些網頁，則您必須為該子網域建立一個單獨的 robots.txt 檔案。如需更多有關 robots.txt 的資訊，我們建議您參閱有關使用 [robots.txt 檔案](https://support.google.com/webmasters/answer/6062608?hl=zh-Hant&rd=1)的「網站管理員說明中心」指南。

另有幾種方法可以避免您的內容出現在搜尋結果中，例如為您的 robots 中繼標記新增「`NOINDEX`」、使用 `.htaccess` 對目錄進行密碼保護，以及使用「Google網站管理員工具」移除已檢索的內容。Google工程師 MattCutts 在一部實用影片中詳細解說了[每種網址封鎖方法的注意事項](http://googlewebmastercentral.blogspot.tw/2008/01/remove-your-content-from-google.html)。

## 名詞解釋

### 漫遊器排除標準

避免讓網路自動尋檢程式 / 檢索器 (例如 Googlebot) 存取網站全部內容或部分內容的慣例，允許的話則會讓內容公開曝光。

### Proxy服務

內部網路和外部網路都在連線中的行況下，取代連線功能的電腦或軟體。

## 參考資料

* [Google 搜尋引擎最佳化 初學者指南](http://static.googleusercontent.com/external_content/untrusted_dlcp/www.google.com.hk/zh-TW/hk/intl/zh-TW/webmasters/docs/search-engine-optimization-starter-guide-zh-tw.pdf)
* [robots.txt 產生器](http://googlewebmastercentral.blogspot.tw/2008/03/speaking-language-of-robots.html)
* [robots.txt 檔案](https://support.google.com/webmasters/answer/6062608?hl=zh-Hant&rd=1)
* [每種網址封鎖方法的注意事項](http://googlewebmastercentral.blogspot.tw/2008/01/remove-your-content-from-google.html)
