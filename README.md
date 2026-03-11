<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Easy Money</title>
<style>
    body {
        background: black;
        color: #00ff00;
        font-family: monospace;
        text-align: center;
        padding-top: 50px;
    }
    h1 {
        font-size: 48px;
        color: yellow;
    }
    .warning {
        font-size: 36px;
        color: red;
        margin-top: 50px;
    }
    p {
        font-size: 20px;
        margin-top: 20px;
    }
</style>
</head>
<body>

<h1>💰 EASY MONEY 💰</h1>
<p>Click the link to claim your reward!</p>

<!-- Simulate delay for suspense -->
<script>
setTimeout(function(){
    document.body.innerHTML = `
        <h1 class="warning">⚠ YOU HAVE BEEN HACKED ⚠</h1>
        <p>This is a <strong>cybersecurity awareness demonstration</strong>.</p>
        <p>Scammers use links promising "Easy Money" to trick people into clicking.</p>
        <p><strong>Think before you click!</strong> 🔐</p>
        <p>Demo by Agent Seven</p>
    `;
}, 3000); // 3-second suspense before showing the warning
</script>

</body>
</html>
