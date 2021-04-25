# Keisan-Program
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>合計金額の計算</title>
</head>
<body>
    <h1>合計金額　計算</h1>

    <form method="post">
    <label for = "kakaku">価格</label>
        <input type="text" id = "kakaku" name = "kakaku"><br>
    <label for = "kosuu">個数</label>
        <input type="text" id = "kosuu" name ="kosuu"><br>

        <input type = "submit" id = "keisan" value="計算する">
    </form>

    <script>
        const keisan = document.getElementById('keisan');
        keisan.addEventListener("click",function(event){
            const kakaku = document.getElementById('kakaku').value;
            const kosuu = document.getElementById('kosuu').value;
            const total = kakaku * kosuu
            console.log(total)
            event.preventDefault();
        },false)

        
    </script>
</body>
</html>
