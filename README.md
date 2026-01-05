<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<title>Hack Menu Demo</title>
<style>
body {
    margin: 0;
    background: transparent;
    font-family: Arial, sans-serif;
}

/* Nút mở menu */
#openBtn {
    position: fixed;
    top: 20px;
    left: 20px;
    background: red;
    color: white;
    border: none;
    padding: 10px 15px;
    border-radius: 5px;
    font-weight: bold;
}

/* Menu chính */
#menu {
    position: fixed;
    top: 60px;
    left: 20px;
    width: 220px;
    background: #111;
    color: white;
    border-radius: 10px;
    display: none;
    padding: 10px;
    box-shadow: 0 0 10px red;
}

#menu h3 {
    text-align: center;
    margin: 5px 0 10px;
    color: red;
}

/* Nút chức năng */
.func {
    background: #222;
    margin: 6px 0;
    padding: 8px;
    border-radius: 5px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.func button {
    background: gray;
    color: white;
    border: none;
    padding: 5px 10px;
    border-radius: 4px;
}
</style>
</head>
<body>

<button id="openBtn" onclick="toggleMenu()">☰ HACK</button>

<div id="menu">
    <h3>HACK MENU</h3>

    <div class="func">God Mode <button onclick="toggle(this)">OFF</button></div>
    <div class="func">Speed Hack <button onclick="toggle(this)">OFF</button></div>
    <div class="func">No Cooldown <button onclick="toggle(this)">OFF</button></div>
    <div class="func">Auto Win <button onclick="toggle(this)">OFF</button></div>
    <div class="func">ESP <button onclick="toggle(this)">OFF</button></div>
</div>

<script>
function toggleMenu() {
    let m = document.getElementById("menu");
    m.style.display = (m.style.display === "none") ? "block" : "none";
}

function toggle(btn) {
    if (btn.innerText === "OFF") {
        btn.innerText = "ON";
        btn.style.background = "lime";
        btn.style.color = "black";
    } else {
        btn.innerText = "OFF";
        btn.style.background = "gray";
        btn.style.color = "white";
    }
}
</script>

</body>
</html>
