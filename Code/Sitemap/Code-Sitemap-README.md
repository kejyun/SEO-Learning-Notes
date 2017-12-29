# Sitemap

## 去除 XML 特殊字元

### 正規表示式 PHP Code

```php
function utf8_for_xml($string)
{
    return preg_replace ('/[^\x{0009}\x{000a}\x{000d}\x{0020}-\x{D7FF}\x{E000}-\x{FFFD}]+/u', ' ', $string);
}
```



## 參考資料
* [character encoding - PHP generated XML shows invalid Char value 27 message - Stack Overflow](https://stackoverflow.com/questions/12229572/php-generated-xml-shows-invalid-char-value-27-message)