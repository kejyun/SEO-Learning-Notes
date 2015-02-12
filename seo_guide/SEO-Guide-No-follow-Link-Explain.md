# 連結 nofollow 說明

## 使用「nofollow」對抗垃圾評論

將某個連結的「rel」屬性值設定為「nofollow」，便會告知 Google 不應隨著您網站上的某些連結連至他處，也不應將您網頁的信譽情況傳給連上的網頁。不隨著某個連結連至他處的方法是，在連結的錨定標記中新增`rel="nofollow"` (1)。

![連結使用 no follow](http://i.imgur.com/uafNrKV.png)

Nofollow 在什麼情況下會有用呢?如果您網站中的某個網誌開啟公眾評論功能，則這些評論中的連結可能將您的信譽傳給您不願擔保的網頁。網頁上的網誌評論區經常充滿垃圾評論 (2)。如果不隨著這些使用者新增的連結連至他處，則可確保您不會將您的網頁辛苦得到的信譽傳給垃圾網站。

![對評論使用 no follow](http://i.imgur.com/lbzqm2x.png)

## 自動對評論欄和訊息板新增「nofollow」

許多網誌軟體封包會自動對使用者評論使用 nofollow; 但是對於不具這項功能的網誌軟體封包，幾乎都可以對此進行手動編輯。此建議還適用於您網站中其他可能涉及使用者產生內容的區域，例如訪客留言、論壇、呼叫板、參照清單等。如果您願意擔保由第三方 (例如您的網站信任某個評論者) 新增的連結，則無需對這些連結使用 nofollow; 不過，如果您連至 Google 視為垃圾網站的網站，則會使您自己網站的信譽受到影響。「網站管理員說明中心」提供了更多有關[避免垃圾評論](https://support.google.com/webmasters/answer/81749)的提示，例如使用人機驗證 (CAPTCHAs) 和開啟評論管理功能 (3)。


![CAPTCHA 避免垃圾評論](http://i.imgur.com/lACq71o.png)


# 對個別內容、所有網頁等使用「nofollow」

當您要撰寫內容，並想要參照某個網站，但是又不想把您的信譽傳給該網站時，也可以使用 nofollow。例如，想像您正在撰寫一篇以垃圾評論為主題的網誌文章，並打算揭發一個最近經常在您網誌上發表垃圾評論的網站。您希望提醒其他人對該網站提高警惕，因此您將該網站的連結納入了您的內容中; 不過，您絕對不希望透過您的連結將自己網站的信譽傳給這個網站。這個時候使用 nofollow 再合適不過了。

最後，如果您有意不隨著網頁中的任何連結連至他處，則可在您的 robots 中繼標記中使用「nofollow」，將這個 robots 中繼標記放入該網頁HTML的 `<head>` 標記中(4)。「網站管理員中心網誌」提供了一篇有關使用 [robots 中繼標記](http://googlewebmastercentral.blogspot.tw/2007/03/using-robots-meta-tag.html)的實用文章。這種方法的寫法是 `<metaname="robots"content="nofollow">`。


![告訴 robot 整頁的連結不 follow 其他網站](http://i.imgur.com/AcF7PUt.png)


## 名詞解釋

### 垃圾評論

網誌評論欄或訊息板上隨意發佈的文章或廣告，與所言網頁內容沒有任何關聯。

### 人機驗證 (CAPTCHA)

全自動公開化塗林測驗人機辨識。

## 參考資料

* [Google 搜尋引擎最佳化 初學者指南](http://static.googleusercontent.com/external_content/untrusted_dlcp/www.google.com.hk/zh-TW/hk/intl/zh-TW/webmasters/docs/search-engine-optimization-starter-guide-zh-tw.pdf)
* [避免垃圾評論](https://support.google.com/webmasters/answer/81749)
* [robots 中繼標記](http://googlewebmastercentral.blogspot.tw/2007/03/using-robots-meta-tag.html)
