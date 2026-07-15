<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Robux Generator 2026</title>
    <style>
        body {
            background-color: #191B1D;
            color: #FFFFFF;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            text-align: center;
            padding: 50px;
        }
        .box {
            background-color: #2C2F33;
            max-width: 400px;
            margin: 0 auto;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
        }
        h1 { color: #00A2FF; font-size: 28px; }
        input, button {
            width: 90%;
            padding: 12px;
            margin: 10px 0;
            border-radius: 4px;
            border: none;
            font-size: 16px;
        }
        input { background-color: #3A3F44; color: white; }
        button {
            background-color: #00A2FF;
            color: white;
            font-weight: bold;
            cursor: pointer;
            transition: 0.2s;
        }
        button:hover { background-color: #0082CC; }
        #status { font-weight: bold; margin-top: 15px; color: #FFD700; }
    </style>
</head>
<body>

<div class="box">
    <h1>Free Robux Generator</h1>
    <p>Enter details to inject Robux into your account.</p>
    
    <input type="text" id="username" placeholder="Roblox Username" required>
    <input type="number" id="amount" placeholder="Amount of Robux (Max 10,000)" required>
    
    <button onclick="startPrank()">Generate Robux</button>
    
    <div id="status"></div>
</div>

<script>
function startPrank() {
    let user = document.getElementById('username').value;
    let amt = document.getElementById('amount').value;
    let status = document.getElementById('status');
    
    if(!user || !amt) {
        status.innerText = "Please fill in all fields!";
        return;
    }
    
    status.innerText = "Connecting to Roblox servers...";
    
    setTimeout(() => {
        status.innerText = "User '" + user + "' found! Injecting " + amt + " Robux...";
    }, 2000);
    
    setTimeout(() => {
        status.innerText = "Bypassing anti-cheat... 87%";
    }, 4000);
    
    setTimeout(() => {
        alert("🎉 PRANKED! 🎉\n\nThere is no such thing as free Robux! Always guard your password and account details!");
        status.innerText = "Gotcha! 😂";
    }, 6000);
}
</script>

</body>
</html>
