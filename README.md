<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>भक्ति लॉकर - अपना वर्चुअल लॉकर खोलें</title>
    <style>
        body {
            background-color: #ff9933;
            font-family: Arial, sans-serif;
            text-align: center;
            color: white;
        }
        .container {
            margin-top: 50px;
        }
        .locker-input {
            padding: 10px;
            font-size: 18px;
            border-radius: 5px;
            border: none;
            text-align: center;
        }
        .locker-button {
            background-color: #cc3300;
            color: white;
            padding: 15px 30px;
            border: none;
            font-size: 20px;
            cursor: pointer;
            border-radius: 10px;
            margin-top: 10px;
        }
        .locker-button:hover {
            background-color: #992600;
        }
        .locker-message {
            font-size: 22px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>भक्ति लॉकर</h1>
        <p>अपने आराध्य भगवान का नाम लिखें और लॉकर खोलें!</p>
        <input type="text" id="godName" class="locker-input" placeholder="भगवान का नाम दर्ज करें">
        <br>
        <button class="locker-button" onclick="openLocker()">लॉकर खोलें</button>
        <p id="message" class="locker-message"></p>
    </div>

    <script>
        function openLocker() {
            var name = document.getElementById("godName").value;
            if(name.trim() === "") {
                document.getElementById("message").innerText = "कृपया भगवान का नाम दर्ज करें।";
            } else {
                document.getElementById("message").innerText = name + " का लॉकर खुल गया!";
            }
        }
    </script>
</body>
</html>
# Bhakti-Bank-locker-
