<h1> 程式介紹 </h1>
本程式會從 src/quotation.txt 內讀取資料 (請按照提供之格式並注意不要有多餘的空白或換行，沒寫防呆QQ) <br>
接著會自動生成 output/{報價單號}_{抬頭} 之 .doc 檔案和 .json 檔案 <br>

<h1>quotation.txt 之固定格式</h1>
<hr>
傳給消費者之內容格式，以訊息方式傳送 <br>
```
抬頭：（有報帳需求才需填寫） <br>
統編：（有報帳需求才需填寫） <br>
聯絡人： <br>
電話： <br>
信箱： <br>
活動日期： <br>
地址： <br>
--------分隔線--------- <br>
餐廳名稱： <br>
日期： <br>
送達時間： <br>
回收時間： <br>
訂餐內容： <br>
--------分隔線--------- <br>
<br>

拿到消費者回傳的訊息後，請手動新增前四行，完成後之 quotation.txt 如下，類別內容填（訂餐/租餐具）。 <br>

報價單號：B108 <br>
報價日期：8/18 <br>
運費：0 <br>
類別：訂餐  <br>
抬頭：aaa <br>
統編：12345678 <br>
聯絡人：曾ㄚㄚ <br>
電話：099999999 <br>
信箱：aaaa@gmail.com <br>
活動日期：8/21 <br>
地址：台北市中山區xx路3號 <br>
--------分隔線--------- <br>
餐廳名稱：好吃的便當 <br>
日期：08/21 <br>
送達時間：11:45 <br>
回收時間：14:00 <br>
滷肉便當：*110 80 <br>
素食便當：*2 80 <br>
--------分隔線--------- <br>
<br>

<h1>生成的檔案形式</h1>
<hr>
共會生成三個檔案，分別為docx、csv、json檔<br>
![image](https://github.com/chenyc1126/Auto_Quotation/assets/137832751/7b1c3194-4c5c-4c7e-94fa-3dec50a7310d)
報價單格式<br>
![image](https://github.com/chenyc1126/Auto_Quotation/assets/137832751/26494619-574a-4d96-ba85-bac9cec167a4)



<h1> 用法 </h1>
1.<br>
pip3 install -r requirement.txt<br>
py auto_quotation.py #windows<br>
python3 auto_quotation.py #linux or mac<br>
<br>
2.<br>
填寫完 src/quotation.txt 後，雙擊 auto_quotation.exe

