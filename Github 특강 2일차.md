# Github 특강 2일차

### Telegram 메신져

##### MSA : Micro Service Architecture

```cmd
-python --version  # 버젼 3.6이상
-python -m pip install --upgrade pip # python 업그레이드
-pip install flask
```
Python, flask 설치

Flask :  Python  Web Framework

```python
app = Flask(__name__) 
@app.route("/") 
def home():
    return 'hello'
```
loacalhost:5000로 접속하면된다
port번호 5000은 Flask의 기본 설정값이다.
```cmd
@app.route('/name')
def name():
    return "홍길동"
#localhost:5000/name
```
-flask run
http://gitignore.io

$ git tag -a v0.0.1 -m "version 0.0.1" ad591(커밋해시)



https://api.telegram.org/
bot<token>
/METHOD_NAME

https://api.telegram.org/
bot924818788:AAF5xDuBa7DUhi8zdSXhztsrxIBQlavdj1Q
/getMe

/getMe

/sendMessage?chat_id=1231231&text=하하

/getUpdates