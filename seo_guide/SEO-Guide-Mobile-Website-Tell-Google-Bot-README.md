# 行動網站 - 告知 Google 爬蟲

## 設定行動網站，讓Google為其正確製作索引

當今世界已進入行動時代，許多人每天使用行動電話，而且有大量使用者透過 [Google 的行動搜尋網頁](http://www.google.com.tw/mobile/) 進行搜尋。不過，身為網站管理員，經營行動網站並融入行動搜尋對象並非易事。行動網站不僅和一般電腦網站使用不同的格式，而且所需的管理方式和專業知識也大有不同。因此形成各式各樣的挑戰。雖然許多行動網站在設計時有考慮行動瀏覽的問題，但沒有打算設計成易於搜尋的網站。

![Google 行動搜尋與標準電腦搜尋差異](http://i.imgur.com/ukPPTfv.png)

以下提供一些疑難排解的秘訣，協助您確定網站是否受到適當地檢索和索引:

## 驗證Google是否替行動網站製作索引

如果您使用 [site: 運算子](https://support.google.com/webmasters/answer/35256)後，您的網站仍然沒有在Google行動搜尋的搜尋結果中出現，可能是因為您的網站發生下列兩個問題:

### 1.Googlebot 可能無法找到您的網站

Googlebot 必須先檢索您的網站才可以將您的網站納入我們的搜尋索引。如果您最近才建立網站，我們可能尚未注意到您的網站，如果是這樣的話，請建立[行動網頁 Sitemap](https://support.google.com/webmasters/topic/2370586?hl=zh-Hant&rd=1) 並提交至 Google，通知我們該網站早已建立。行動網頁 Sitemap 可以[使用 Google 網站管理員工具提交](https://support.google.com/webmasters/answer/156184)，一如提交標準的 Sitemap。

### 2.Googlebot 可能無法存取您的網站

部分行動網站只接受行動電話存取，這讓 Googlebot 無法存取該網站，也讓人無法搜尋該網站。我們的行動網站檢索器是「`Googlebot-Mobile`」。如果您想要檢索您的網站，請允許「`Googlebot-Mobile`」等任何使用者代理程式存取您的網站 (2)。您也要注意 Google 可能隨時變更使用者代理程式資訊，且不另行通知，因此我們不建議您檢查使用者代理程式是否和「`Googlebot-Mobile`」(目前的使用者代理程式) 完全相符，但建議您檢查使用者代理程式標頭是否含有「Googlebot-Mobile」字串。您也可以使用 [DNS 查詢以驗證 Googlebot](http://googlewebmastercentral.blogspot.tw/2006/09/how-to-verify-googlebot.html)。

![設定允許來自「Googlebot-Mobile」使用者代理程式存取](http://i.imgur.com/JzWcSHT.png)

## 驗證Google是否可辨識您的行動網址

只要 `Googlebot-Mobile` 檢索您的網址，我們即可檢查是否在行動裝置上，每一個網址都可以瀏覽。我們認為無法在行動電話上瀏覽的網頁不會包含在我們的行動網站索引中 (雖然這些網頁可能包含在一般網站索引中)，我們基於各種因素才決定這麼做，而「DTD (文件類型定義)」宣告便是因素之一。請檢查易於行動裝置使用的網址，其 DTD 宣告是否為適當的行動格式，例如 XHTML 行動網頁或 Compact HTML (3)。如果網址是相容格式，那麼網頁就能包含在行動搜尋索引中。如需詳細資訊，請參閱[行動網站管理員指南](https://support.google.com/webmasters/answer/72462)。

![行動裝置 DTD](http://i.imgur.com/Di3iUnC.png)


## 名詞解釋

### 行動網頁Sitemap

XML Sitemap 含有的網頁網址是特別為行動電話設計的。當您將行動電話網站內容的網址提交給 Google 時，即通知我們這些網頁的存在，可讓我們對這些網頁進行檢索。

### 使用者代理程式

使用者存取網站時使用的軟體和硬體。

### XHTML 行動網頁

XHTML 為一種先經過 HTML 改寫成 XML 進而重新定義的標記語言，然後進一步擴充供行動電話使用。

### Compact HTML

一種類似HTML的標記語言，通常用於建立可在行動電話、PHS、PDA 上顯示的網頁。


## 參考資料

* [Google 搜尋引擎最佳化 初學者指南](http://static.googleusercontent.com/external_content/untrusted_dlcp/www.google.com.hk/zh-TW/hk/intl/zh-TW/webmasters/docs/search-engine-optimization-starter-guide-zh-tw.pdf)
* [Google 的行動搜尋網頁](http://www.google.com.tw/mobile/)
* [site: 運算子](https://support.google.com/webmasters/answer/35256)
* [行動網頁 Sitemap](https://support.google.com/webmasters/topic/2370586?hl=zh-Hant&rd=1)
* [使用 Google 網站管理員工具提交](https://support.google.com/webmasters/answer/156184)
* [DNS 查詢以驗證 Googlebot](http://googlewebmastercentral.blogspot.tw/2006/09/how-to-verify-googlebot.html)
* [行動網站管理員指南](https://support.google.com/webmasters/answer/72462)
* [W3C mobileOK Checker](http://validator.w3.org/mobile/)
* [mobiReady - dotMobi compliance & mobileOK checker](http://ready.mobi/launch.jsp?locale=en_EN)
