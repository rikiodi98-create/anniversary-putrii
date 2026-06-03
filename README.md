# anniversary-putrii
Website anniversary 10 bulan untuk Putri ❤️
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy 10 Month Anniversary Putri ❤️</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

body{
    background: linear-gradient(135deg,#ff7eb3,#ff4f81);
    min-height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    overflow:hidden;
}

.card{
    background:white;
    width:90%;
    max-width:600px;
    padding:35px;
    border-radius:25px;
    text-align:center;
    box-shadow:0 10px 30px rgba(0,0,0,0.2);
    position:relative;
    z-index:2;
}

h1{
    color:#ff4f81;
    margin-bottom:15px;
}

p{
    color:#555;
    line-height:1.8;
    margin-bottom:15px;
}

button{
    background:#ff4f81;
    color:white;
    border:none;
    padding:12px 25px;
    border-radius:30px;
    cursor:pointer;
    font-size:16px;
    margin-top:10px;
}

button:hover{
    background:#ff2d68;
}

#pesan{
    margin-top:20px;
    color:#ff2d68;
    font-weight:bold;
    font-size:18px;
}

.heart{
    position:absolute;
    color:white;
    font-size:24px;
    animation:jatuh linear infinite;
}

@keyframes jatuh{
    from{
        transform:translateY(-100vh);
    }
    to{
        transform:translateY(100vh);
    }
}
</style>
</head>

<body>

<div class="card">
    <h1>💖 Happy 10 Month Anniversary Putri 💖</h1>

    <p>
        Hai Putri ❤️
    </p>

    <p>
        Tidak terasa ya, kita sudah bersama selama <b>10 bulan</b>.
        Rasanya baru kemarin kita mulai saling mengenal,
        tapi sekarang sudah banyak sekali cerita, tawa,
        dan kenangan yang kita lewati bersama.
    </p>

    <p>
        Terima kasih karena selalu ada, selalu sabar,
        dan selalu menjadi seseorang yang spesial di hidupku.
        Semoga hubungan kita semakin kuat, semakin bahagia,
        dan dipenuhi banyak momen indah ke depannya.
    </p>

    <button onclick="pesanCinta()">Klik Aku Sayang ❤️</button>

    <div id="pesan"></div>
</div>

<script>
function pesanCinta(){
    document.getElementById("pesan").innerHTML =
    "Putri ❤️ Terima kasih sudah menemani aku selama 10 bulan ini. Semoga kita selalu bersama dan bahagia. I Love You ❤️";
}

for(let i=0;i<50;i++){
    let heart=document.createElement("div");
    heart.className="heart";
    heart.innerHTML="❤";
    heart.style.left=Math.random()*100+"vw";
    heart.style.animationDuration=(4+Math.random()*5)+"s";
    heart.style.opacity=Math.random();
    document.body.appendChild(heart);
}
</script>

</body>
</html>
