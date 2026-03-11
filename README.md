<!DOCTYPE html>
<html>
<head>
    <style>
        body { 
            background: #0a1a2a;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: Arial;
            margin: 0;
        }
        .hack-link {
            background: linear-gradient(45deg, #ffd700, #ffa500);
            color: #000;
            font-size: 4rem;
            font-weight: 900;
            padding: 2rem 4rem;
            border-radius: 80px 20px 80px 20px;
            text-decoration: none;
            border: 5px solid #fff;
            box-shadow: 0 20px 0 #8b0000;
            display: inline-block;
            transition: all 0.1s;
            cursor: pointer;
        }
        .hack-link:active {
            background: #8b0000;
            color: white;
            box-shadow: 0 5px 0 #4a0000;
            transform: translateY(15px);
            font-size: 3rem;
            content: "YOUR PHONE HAS BEEN HACKED";
        }
    </style>
</head>
<body>
    <a href="#" class="hack-link" onclick="this.innerHTML='⚠️ YOUR PHONE HAS BEEN HACKED ⚠️'; this.style.background='#8b0000'; this.style.color='white'; this.style.fontSize='2.5rem'; return false;">💰 EASY MONEY 💰</a>
</body>
</html>
