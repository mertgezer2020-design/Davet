[index 4.html](https://github.com/user-attachments/files/25222720/index.4.html)
<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<title>Düğün Davetiyesi</title>

<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500&family=Playfair+Display:wght@500;600&display=swap" rel="stylesheet">

<style>
body{
  margin:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  background:#f6f2ec;
  font-family:'Montserrat', sans-serif;
}

.cover{
  width:100%;
  max-width:360px;
  height:540px;
  background:#fdfbf7;
  border-radius:22px;
  box-shadow:0 20px 50px rgba(0,0,0,.15);
  display:flex;
  justify-content:center;
  align-items:center;
  text-align:center;
  padding:30px;
  cursor:pointer;
}

.cover-inner{
  padding:42px 26px;
  border:1px solid #d6c48f;
  border-radius:18px;
}

.cover-text{
  font-family:'Playfair Display', serif;
  font-size:16px;
  line-height:1.8;
  color:#2c2c2c;
}

.cover-spoiler{
  margin-top:16px;
  font-size:14px;
  font-style:italic;
  color:#555;
}

.cover-highlight{
  margin-top:10px;
  font-family:'Playfair Display', serif;
  font-size:18px;
  color:#1f1f1f;
}

.cover-sub{
  margin-top:30px;
  font-size:12px;
  letter-spacing:1px;
  color:#8a8a8a;
}

.invite{
  display:none;
  background:#ffffff;
  padding:40px 32px;
  border-radius:22px;
  box-shadow:0 20px 50px rgba(0,0,0,.15);
  text-align:center;
  max-width:360px;
}

.animate{
  opacity:0;
  transform:translateY(18px);
  animation:fadeUp 0.9s ease forwards;
}

.delay1{animation-delay:.2s}
.delay2{animation-delay:.4s}
.delay3{animation-delay:.6s}
.delay4{animation-delay:.8s}
.delay5{animation-delay:1s}
.delay6{animation-delay:1.2s}

@keyframes fadeUp{
  to{opacity:1; transform:translateY(0);}
}

.names{
  font-family:'Playfair Display', serif;
  font-size:26px;
  letter-spacing:1px;
  color:#2c2c2c;
}

.text{
  font-size:14px;
  line-height:1.7;
  color:#555;
}

.highlight{
  font-family:'Playfair Display', serif;
  font-size:18px;
  margin-top:12px;
  letter-spacing:.8px;
  color:#1f1f1f;
}

button{
  margin-top:26px;
  padding:12px 28px;
  border:none;
  border-radius:999px;
  background:#b89b4f;
  color:white;
  font-size:14px;
  letter-spacing:.6px;
}
</style>
</head>

<body>

<div class="cover" onclick="openInvite()">
  <div class="cover-inner">
    <div class="cover-text">
      Bir ömür boyu sürecek “biz”e ilk adımı atıyoruz.<br>
      Bu mutluluğa ortak olmanız dileğiyle…
    </div>

    <div class="cover-spoiler">
      Spoiler: Mutlu son!
    </div>

    <div class="cover-highlight">
      Biz evleniyoruz 💍
    </div>

    <div class="cover-sub">
      DAVETİYEYİ AÇMAK İÇİN DOKUNUN
    </div>
  </div>
</div>

<div class="invite" id="invite">

  <div class="animate delay1 highlight">
    BİZ EVLENİYORUZ 💍
  </div>

  <h3 class="animate delay2 names" style="margin-top:26px;">
    Günser Karamez<br>&<br>Mert Gezer
  </h3>

  <p class="animate delay3 text" style="margin-top:22px;">
    <b>Gelinin Anne ve Babası</b><br>
    Gülsün – Ural Karamez
  </p>

  <p class="animate delay4 text" style="margin-top:16px;">
    <b>Damadın Anne ve Babası</b><br>
    Gezer Ailesi
  </p>

  <p class="animate delay5 text" style="margin-top:18px;">
    20 Haziran 2026<br>
    Nikâh Saati: 19:45<br>
    Fuar Premier Hall
  </p>

  <button class="animate delay6"
    onclick="window.open('https://www.google.com/maps/search/Fuar+Premier+Hall')">
    Konuma Git
  </button>

</div>

<script>
function openInvite(){
  document.querySelector('.cover').style.display="none";
  document.getElementById('invite').style.display="block";
}
</script>

</body>
</html>
