# flask-bootstrap-deployment
A practice project to learn Flask web development and deployment using PythonAnywhere.

## 網站連結  

[https://你的用戶名.pythonanywhere.com  ](https://mark1116.pythonanywhere.com/)

## 專案結構
my_flask_app/

├── flask_app.py # Flask 主程式

├── templates/

│   └── index.html # HTML 模板，使用 Jinja2 語法

├── static/

│   └── assets/ # CSS、JS、圖片等靜態資源（Bootstrap 模板）

## 使用技術

- Python 3.10
- Flask
- Bootstrap 5（iPortfolio 模板)
- HTML / CSS / JavaScript
- PythonAnywhere 免費空間部署

## 製作過程

- 解壓縮並整理 Bootstrap 模板  
- 修改 HTML 中所有靜態檔案路徑，使用 `{{ url_for('static', filename='...') }}`  
- 替換個人照片與文字內容，客製化網站風格  
- 在 PythonAnywhere 平台設定並部署 Flask 應用

## 遇到問題與解決方法

| 問題                           | 解決方式                              |
|------------------------------|-----------------------------------|
| 靜態檔案無法正常顯示             | 將 HTML 內所有靜態資源路徑改用 `url_for('static', filename='...')` |
| WSGI 配置錯誤                  | 修改 `wsgi.py`，正確設定專案路徑與 Flask app 名稱            |
| 圖片不顯示                     | 確認圖片路徑正確，並調整圖片格式（如 jpg, png）                |
| 模板修改後網頁未更新             | 清除瀏覽器快取或強制重新整理（Ctrl + F5）                     |
