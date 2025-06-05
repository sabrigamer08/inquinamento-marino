<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>#SALVIAMO GLI OCEANI</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Cambria', sans-serif;
      font-size: 2rem;
      margin-bottom: 0.50rem;
      background-color: #f4fefc;
      color: #013440;
    }

    header {
      background-image: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)),
      url("https://www.intotheblue.it/wp-content/uploads/2023/03/vlcsnap-2023-02-14-15h09m24s700-2048x1152.png");
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      color: white;
      padding: 8rem 2rem;
      text-align: center;
      animation: fadeIn 2s ease-in-out;
    }

    header h1 {
      font-size: 3rem;
      margin-bottom: 0.5rem;
    }

    header p {
      font-size: 1.2rem;
      font-style: italic;
    }

    .wave {
      display: block;
      width: 100%;
      height: 100px;
      background: url('https://www.transparenttextures.com/patterns/waves.png');
    }

    .section {
      padding: 4rem 2rem;
      max-width: 1100px;
      margin: auto;
      animation: fadeInUp 1s ease-in-out;
    }

    .section h2 {
      font-size: 2rem;
      margin-bottom: 1rem;
    }

    .section-content {
      display: flex;
      flex-wrap: wrap;
      gap: 2rem;
      align-items: center;
    }

    .section-content img {
      flex: 2;
      min-width: 300px;
      max-width: 100%;
      width: 100%;
      border-radius: 10px;
      transition: transform 0.3s ease;
    }

    .section-content img:hover {
      transform: scale(1.05);
    }

    .section-content div {
      flex: 1;
    }

    .stats {
      display: flex;
      justify-content: space-around;
      text-align: center;
      margin-top: 3rem;
      flex-wrap: wrap;
    }

    .stats div {
      flex: 1;
      min-width: 150px;
      padding: 1rem;
    }

    .stats h3 {
      font-size: 2rem;
      color: #0074D9;
      margin-bottom: 0.5rem;
    }

    .button {
      display: inline-block;
      margin-top: 2rem;
      padding: 1rem 2rem;
      background-color: #2ECC40;
      color: white;
      font-weight: bold;
      text-decoration: none;
      border-radius: 5px;
      transition: background-color 0.3s ease;
    }

    .button:hover {
      background-color: #28a745;
    }

    footer {
      background-color: #013440;
      color: white;
      text-align: center;
      padding: 1.5rem;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* 📱 Responsive design per mobile */
    @media (max-width: 768px) {
      .section-content {
        flex-direction: column;
        text-align: center;
      }

      .section-content img {
        max-width: 100%;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>SALVIAMO GLI OCEANI</h1>
    <p>Per un mondo dove il mare possa respirare</p>
  </header> 

  <section class="section">
    <h2>Il nostro obiettivo</h2>
    <div class="section-content">
      <div>
        <p>Raccogliere fondi per aumentare la consapevolezza e promuovere azioni concrete contro l'inquinamento marino, proteggendo la biodiversità e garantendo un ambiente più sano per le generazioni future.</p>
        <a class="button" href="#">Scopri come aiutare</a>
      </div>
      <img src="https://www.wwf.ch/sites/default/files/styles/facebook/public/2021-02/PlasticWasteinthePacificTaiwan_c_MagnusLundgrenWildWondersofChina_WW1119577.jpg?h=f6963184&itok=4lA71gko" alt="Barriera corallina"> 
    </div>
  </section>

  <section class="section">
    <h2>Oceano Atlantico e Pacifico</h2>
    <div class="section-content">
      <img src="https://www.wwf.ch/sites/default/files/styles/facebook/public/2021-02/PlasticWasteinthePacificTaiwan_c_MagnusLundgrenWildWondersofChina_WW1119577.jpg?h=f6963184&itok=4lA71gko" alt="Oceano Atlantico">
      <div>
        <p>L’Atlantico e il Pacifico sono due ecosistemi chiave per la vita sul nostro pianeta. Ma oggi sono minacciati dall'inquinamento, dalla pesca eccessiva e dal cambiamento climatico. Proteggerli significa proteggere anche noi stessi.</p>
      </div>
    </div>
  </section>

  <section class="section">
    <h2>Numeri significativi</h2>
    <div class="stats">
      <div>
        <h3>86mln</h3>
        <p>di tonnellate di plastica navigano nei nostri oceani</p>
      </div>
      <div>
        <h3>8mln</h3>
        <p>di tonnellate di rifiuti di plastica finiscono ogni anno negli oceani</p>
      </div>
      <div>
        <h3>700</h3>
        <p>specie sono state interessate da fenomeni di inquinamento di materie plastiche</p>
      </div>
    </div>
  </section>

  <section class="section">
    <h2>Partecipa anche tu</h2>
    <div class="section-content">
      <div>
        <p>Condividi la campagna, informati e dona. Ogni piccola azione conta: perché anche un piccolo gesto può salvare una grande vita.</p>
        <a class="button" href="javascript:void(0);" onclick="openModal()">Dona ora</a>
      </div>
      <img src="https://www.greenme.it/wp-content/uploads/2021/08/plastica-tartaruga-marina.jpg" alt="Tartaruga marina">
    </div>
  </section>
 
<!-- MODALE DONAZIONE -->
<div id="donation-modal" style="display:none; position:fixed; top:0; left:0; width:100%; height:100%; background:rgba(0,0,0,0.6); z-index:9999; justify-content:center; align-items:center;">
  <div style="background:white; padding:2rem; border-radius:10px; max-width:400px; width:90%; text-align:center; font-family:'Cambria',sans-serif; color:#013440;">
    <h2>Quanto vuoi donare?</h2>
   <button onclick="thankYou('5')" style="margin:1rem; padding:1rem 2rem; font-size:1rem; background:#2ECC40; color:white; border:none; border-radius:5px;">5 euro</button>
   <button onclick="thankYou('20')" style="margin:1rem; padding:1rem 2rem; font-size:1rem; background:#2ECC40; color:white; border:none; border-radius:5px;">20 euro</button>
   <button onclick="thankYou('50')" style="margin:1rem; padding:1rem 2rem; font-size:1rem; background:#2ECC40; color:white; border:none; border-radius:5px;">50 euro</button>
<div id="thank-you-msg" style="margin-top:1.5rem; font-weight:bold; color:#28a745; display:none;">
  Grazie per la donazione!
</div>
    <br><br>
    <button onclick="closeModal()" style="margin-top:1rem; background:#ccc; padding:0.5rem 1rem; border:none; border-radius:5px;">Chiudi</button>
  </div>
</div>

  <footer>
    <p>Campagna scolastica • Salviamo gli oceani • Tutti i diritti riservati</p>
  </footer>

<script>
  function openModal() {
    document.getElementById('donation-modal').style.display = 'flex';
    document.getElementById('thank-you-msg').style.display = 'none';
  }

  function closeModal() {
    document.getElementById('donation-modal').style.display = 'none';
  }

  function thankYou(amount) {
    document.getElementById('thank-you-msg').style.display = 'block';
  }
</script>
