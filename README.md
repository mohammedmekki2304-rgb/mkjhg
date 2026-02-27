<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=!
    , initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>

<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <title>صفحتي الأولى</title>
</head>
<body>
    <h1>مرحباً بك في عالم البرمجة!</h1>
    <p>هذه أول صفحة ويب أقوم بإنشائها باستخدام HTML.</p>
</body>
</html>
import sys
from PyQt5.QtCore import *
from PyQt5.QtWidgets import *
from PyQt5.QtWebEngineWidgets import *

class MyBrowser(QMainWindow):
    def __init__(self):
        super(MyBrowser, self).__init__()
        # إعداد محرك المتصفح
        self.browser = QWebEngineView()
        self.browser.setUrl(QUrl('http://google.com'))
        self.setCentralWidget(self.browser)
        self.showMaximized()

        # شريط الأدوات (Navigation Bar)
        navbar = QToolBar()
        self.addToolBar(navbar)

        # زر العودة للخلف
        back_btn = QAction('Back', self)
        back_btn.triggered.connect(self.browser.back)
        navbar.addAction(back_btn)

        # زر التحديث
        reload_btn = QAction('Reload', self)
        reload_btn.triggered.connect(self.browser.reload)
        navbar.addAction(reload_btn)

        # شريط العنوان (URL Bar)
        self.url_bar = QLineEdit()
        self.url_bar.returnPressed.connect(self.navigate_to_url)
        navbar.addWidget(self.url_bar)

    def navigate_to_url(self):
        url = self.url_bar.text()
        self.browser.setUrl(QUrl(url))

app = QApplication(sys.argv)
QApplication.setApplicationName('My Custom Browser')
window = MyBrowser()
app.exec_()
pip install PyQt5 PyQtWebEngine
<!DOCTYPE html>
<html>
<head>
    <title>صفحة تجريبية</title>
</head>
<body style="background-color: #f0f0f0; text-align: center;">
    <h1>تم تشغيل المتصفح بنجاح!</h1>
    <p>هذا النص يظهر لأن المتصفح قام بترجمة كود HTML.</p>
</body>
</html>








<table>
    /
    /
</table>

Content unavailable. Resource was not cached





