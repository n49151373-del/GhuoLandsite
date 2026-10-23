[Ghuo_Land_site_improved.html](https://github.com/user-attachments/files/33884837/Ghuo_Land_site_improved.html)
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#10091d">
  <meta name="description" content="GHUO LAND — Minecraft-анархия. Новости, сообщество и магазин привилегий.">
  <title>GHUO LAND — Твой мир. Твои правила.</title>
  <style>
    :root{
      --bg:#0b0712;--panel:#151020;--panel2:#1c142a;--purple:#a855f7;
      --purple2:#7c3aed;--pink:#e879f9;--text:#faf7ff;--muted:#b2a5c2;
      --line:#38264d;--green:#6ee7a0;--max:1160px
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth;scroll-padding-top:88px}
    body{margin:0;background:var(--bg);color:var(--text);font:16px/1.65 Inter,Segoe UI,Arial,sans-serif}
    body:before{content:"";position:fixed;inset:0;z-index:-2;pointer-events:none;background:radial-gradient(ellipse at 50% -15%,#542078 0,transparent 42%),radial-gradient(ellipse at 100% 55%,#27123c 0,transparent 35%)}
    a{color:inherit;text-decoration:none}button,input{font:inherit}
    .container{width:min(var(--max),92%);margin:auto}
    .topbar{position:sticky;top:0;z-index:20;background:#0b0712eF;border-bottom:1px solid #ffffff12;backdrop-filter:blur(18px)}
    .nav{min-height:76px;display:flex;align-items:center;justify-content:space-between;gap:22px}
    .brand{display:flex;align-items:center;gap:11px;font-size:19px;font-weight:950;letter-spacing:.8px}
    .brand-mark{width:38px;height:38px;display:grid;place-items:center;border-radius:12px;background:linear-gradient(145deg,#d8a4ff,#792ce0);box-shadow:0 5px 24px #a855f733;color:#170925;font-weight:1000}
    .brand span:last-child{color:#c084fc}
    .navlinks{display:flex;align-items:center;gap:27px;color:var(--muted);font-size:13px;font-weight:700}
    .navlinks a:hover,.footer-links a:hover{color:white}
    .btn{display:inline-flex;align-items:center;justify-content:center;gap:9px;min-height:46px;padding:12px 19px;border:1px solid transparent;border-radius:13px;background:linear-gradient(135deg,#bd76ff,#7c3aed);color:white;font-weight:850;cursor:pointer;transition:transform .2s,box-shadow .2s,border-color .2s}
    .btn:hover{transform:translateY(-2px);box-shadow:0 10px 30px #9333ea35}
    .btn-ghost{background:#ffffff06;border-color:var(--line)}
    .btn-ghost:hover{border-color:#9860c5}
    .btn-small{min-height:39px;padding:9px 14px;font-size:12px}
    .hero{position:relative;text-align:center;padding:104px 0 70px}
    .hero:before{content:"";position:absolute;z-index:-1;left:50%;top:90px;width:360px;height:300px;transform:translateX(-50%);background:#9333ea;filter:blur(150px);opacity:.2}
    .pill{display:inline-flex;align-items:center;gap:9px;border:1px solid #74449a;border-radius:999px;padding:7px 13px;background:#a855f714;color:#e9d5ff;font-size:11px;font-weight:900;letter-spacing:1.7px}
    .dot{width:8px;height:8px;border-radius:50%;background:#fbbf24;box-shadow:0 0 12px #fbbf24}
    h1{margin:27px 0 20px;font-size:clamp(58px,11vw,116px);line-height:.88;letter-spacing:-5px;font-weight:1000}
    .gradient{background:linear-gradient(100deg,#fff,#d8b4fe 42%,#a855f7 78%,#e879f9);background-clip:text;-webkit-background-clip:text;color:transparent}
    .hero-copy{max-width:680px;margin:26px auto;color:var(--muted);font-size:17px;line-height:1.85}
    .actions{display:flex;justify-content:center;gap:12px;flex-wrap:wrap;margin-top:28px}
    .stats{display:grid;grid-template-columns:repeat(3,1fr);max-width:780px;margin:58px auto 0;gap:13px}
    .stat{padding:20px 12px;border:1px solid #ffffff12;border-radius:17px;background:#ffffff05}
    .stat strong{display:block;color:#ead7ff;font-size:23px;line-height:1.3}
    .stat span{color:var(--muted);font-size:12px}
    .note{font-size:12px;color:#9586a6;margin-top:16px}
    section{padding:66px 0}
    .section-head{margin-bottom:28px}
    .eyebrow{color:#c084fc;font-size:11px;font-weight:950;letter-spacing:3px}
    h2{font-size:clamp(29px,5vw,43px);line-height:1.15;letter-spacing:-1.3px;margin:10px 0}
    .section-head p{color:var(--muted);margin:10px 0 0}
    .community{display:flex;align-items:center;gap:22px;padding:29px;border:1px solid #75439b;border-radius:24px;background:linear-gradient(115deg,#2a1640,#171022 72%);overflow:hidden}
    .telegram-icon{flex-shrink:0;width:70px;height:70px;display:grid;place-items:center;border-radius:21px;background:linear-gradient(135deg,#38bdf8,#7c3aed);font-size:32px}
    .community-info{flex:1}.community h3{font-size:22px;margin:0 0 4px}.community p{color:var(--muted);margin:0;font-size:14px}
    .grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:16px}
    .card{min-width:0;padding:25px;border:1px solid var(--line);border-radius:20px;background:linear-gradient(145deg,#1c142a,#120d1c);transition:transform .2s,border-color .2s}
    .card:hover{transform:translateY(-4px);border-color:#8752b1}
    .card-icon{width:49px;height:49px;display:grid;place-items:center;border-radius:15px;background:#a855f71b;font-size:24px}
    .card h3{margin:17px 0 7px;font-size:19px}.card p{color:var(--muted);font-size:14px;margin:0}
    .donate-intro{display:flex;justify-content:space-between;align-items:end;gap:20px;margin-bottom:28px}
    .donate-intro .section-head{margin:0}
    .rank{position:relative;display:flex;flex-direction:column}
    .rank-label{color:#c084fc;font-size:10px;font-weight:950;letter-spacing:2px}
    .rank h3{font-size:25px;margin:10px 0 0}
    .price{font-size:38px;line-height:1.2;font-weight:1000;margin:14px 0}
    .price small{font-size:12px;color:var(--muted);font-weight:600}
    .rank p{min-height:45px}
    .rank .btn{width:100%;margin-top:20px}
    .rank.featured{border-color:#a855f7;box-shadow:0 0 0 1px #a855f71c,0 18px 50px #6b21a81a}
    .featured-tag{position:absolute;top:14px;right:14px;padding:4px 8px;border-radius:99px;background:#a855f722;color:#e9d5ff;font-size:9px;font-weight:900}
    .info-grid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:16px}
    .info-card{padding:24px;border:1px solid var(--line);border-radius:18px;background:var(--panel)}
    .info-card p{font-size:14px;color:var(--muted)}
    .faq{max-width:850px}.faq-item{border-bottom:1px solid var(--line);padding:19px 0}
    .faq-item summary{cursor:pointer;font-weight:850;list-style:none;display:flex;justify-content:space-between;gap:16px}
    .faq-item summary:after{content:"+";color:#c084fc;font-size:22px;line-height:1}
    .faq-item[open] summary:after{content:"−"}
    .faq-item p{color:var(--muted);font-size:14px}
    footer{margin-top:35px;padding:30px 0;border-top:1px solid #ffffff12;color:var(--muted);font-size:13px}
    .footer-inner{display:flex;align-items:center;justify-content:space-between;gap:18px;flex-wrap:wrap}
    .footer-links{display:flex;gap:18px;flex-wrap:wrap}.footer-links a{color:#e9d5ff}
    .modal{position:fixed;inset:0;z-index:50;display:none;align-items:center;justify-content:center;padding:18px;background:#000b}
    .modal.open{display:flex}
    .modal-box{width:min(450px,100%);padding:27px;border:1px solid #75439b;border-radius:23px;background:#171022;box-shadow:0 20px 80px #0009}
    .modal-box h2{font-size:27px}.close{float:right;border:0;border-radius:9px;padding:7px 10px;background:#ffffff12;color:white;cursor:pointer}
    label{display:block;margin:16px 0 7px;color:var(--muted);font-size:13px}
    input{width:100%;padding:14px;border:1px solid var(--line);border-radius:12px;outline:none;background:#0b0714;color:white}
    input:focus{border-color:var(--purple)}.modal-box form .btn{width:100%;margin-top:15px}
    .notice{font-size:12px;color:var(--muted);line-height:1.7}
    @media(max-width:800px){.navlinks{gap:13px}.grid{grid-template-columns:repeat(2,minmax(0,1fr))}.community{flex-wrap:wrap}.community .btn{width:100%}.donate-intro{display:block}}
    @media(max-width:540px){.nav{min-height:66px;gap:8px}.brand{font-size:15px;gap:7px}.brand-mark{width:32px;height:32px}.navlinks{gap:10px;font-size:11px}.navlinks a:nth-child(1){display:none}.nav>.btn{padding:8px 10px;min-height:36px;font-size:10px}.hero{padding:78px 0 48px}h1{letter-spacing:-2px}.hero-copy{font-size:14px}.stats{gap:7px;margin-top:40px}.stat{padding:15px 5px}.stat strong{font-size:17px}.stat span{font-size:10px}.grid,.info-grid{grid-template-columns:1fr}.community{padding:21px}.community h3{font-size:19px}section{padding:47px 0}.card{padding:22px}.rank p{min-height:0}}
    @media(prefers-reduced-motion:reduce){html{scroll-behavior:auto}*,*:before,*:after{transition:none!important}}
  </style>
</head>
<body>
<header class="topbar">
  <div class="container nav">
    <a class="brand" href="#home" aria-label="Ghuo Land — главная"><span class="brand-mark">G</span><span>GHUO<span>LAND</span></span></a>
    <nav class="navlinks" aria-label="Главная навигация">
      <a href="#about">Сервер</a><a href="#donate">Привилегии</a><a href="#community">Сообщество</a>
    </nav>
    <a class="btn btn-small" href="https://t.me/ghuolandservera" target="_blank" rel="noopener noreferrer">Telegram ↗</a>
  </div>
</header>

<main>
  <section class="hero container" id="home">
    <div class="pill"><span class="dot"></span> ПРОЕКТ ГОТОВИТСЯ К ОТКРЫТИЮ</div>
    <h1>GHUO<br><span class="gradient">LAND</span></h1>
    <p class="hero-copy">Твой мир. Твои правила. Твоя история.<br>Погрузись в Minecraft-анархию, исследуй мир и создай собственную легенду вместе с Ghuo Land.</p>
    <div class="actions">
      <a class="btn" href="https://t.me/ghuolandservera" target="_blank" rel="noopener noreferrer">✈ Следить за запуском</a>
      <a class="btn btn-ghost" href="#about">Исследовать сервер ↓</a>
    </div>
    <div class="stats">
      <div class="stat"><strong>1.21.11</strong><span>Планируемая версия</span></div>
      <div class="stat"><strong>SOON</strong><span>Открытие сервера</span></div>
      <div class="stat"><strong>ANARCHY</strong><span>Игровой режим</span></div>
    </div>
    <p class="note">IP-адрес появится здесь и в Telegram после запуска сервера.</p>
  </section>

  <section class="container" id="community">
    <div class="section-head"><span class="eyebrow">НАШЕ СООБЩЕСТВО</span><h2>Будь среди первых</h2><p>Следи за новостями, разработкой и датой открытия Ghuo Land.</p></div>
    <div class="community">
      <div class="telegram-icon">✈</div>
      <div class="community-info"><h3>Ghuo Land · Minecraft</h3><p>Объявления, обновления проекта и новости о запуске — в официальном канале.</p></div>
      <a class="btn" href="https://t.me/ghuolandservera" target="_blank" rel="noopener noreferrer">Открыть канал ↗</a>
    </div>
  </section>

  <section class="container" id="about">
    <div class="section-head"><span class="eyebrow">О ПРОЕКТЕ</span><h2>Больше, чем просто выживание</h2><p>Ghuo Land создаётся для игроков, которым нравится свобода и собственные истории.</p></div>
    <div class="grid">
      <article class="card"><div class="card-icon">⚔️</div><h3>Анархия</h3><p>Исследуй мир, добывай ресурсы, сражайся и выбирай собственный путь.</p></article>
      <article class="card"><div class="card-icon">🌌</div><h3>Фиолетовый стиль</h3><p>Узнаваемая атмосфера Ghuo Land и свой визуальный характер проекта.</p></article>
      <article class="card"><div class="card-icon">🎁</div><h3>Награды</h3><p>Планируем игровые награды и дополнительные возможности для сообщества.</p></article>
    </div>
  </section>

  <section class="container" id="donate">
    <div class="donate-intro"><div class="section-head"><span class="eyebrow">МАГАЗИН GHUO LAND</span><h2>Выбери привилегию</h2><p>Поддержи развитие сервера и выбери свой ранг.</p></div></div>
    <div class="grid">
      <article class="card rank"><span class="rank-label">STARTER</span><h3>START</h3><div class="price">8 ₽</div><p>Первый шаг в линейке привилегий.</p><button class="btn" onclick="buy('START',8)">Выбрать ранг</button></article>
      <article class="card rank"><span class="rank-label">UPGRADE</span><h3>SUPER</h3><div class="price">13 ₽</div><p>Для тех, кто хочет поддержать проект.</p><button class="btn" onclick="buy('SUPER',13)">Выбрать ранг</button></article>
      <article class="card rank featured"><span class="featured-tag">РЕКОМЕНДУЕМ</span><span class="rank-label">POPULAR</span><h3>MEGA</h3><div class="price">15 ₽</div><p>Ещё один уровень поддержки Ghuo Land.</p><button class="btn" onclick="buy('MEGA',15)">Выбрать ранг</button></article>
      <article class="card rank"><span class="rank-label">ADVANCED</span><h3>HERO</h3><div class="price">24 ₽</div><p>Для настоящих героев сообщества.</p><button class="btn" onclick="buy('HERO',24)">Выбрать ранг</button></article>
      <article class="card rank"><span class="rank-label">SPECIAL</span><h3>DEATH</h3><div class="price">40 ₽</div><p>Особый ранг в линейке привилегий.</p><button class="btn" onclick="buy('DEATH',40)">Выбрать ранг</button></article>
      <article class="card"><div class="card-icon">✨</div><h3>Новые предложения</h3><p>Следи за обновлениями магазина и новыми возможностями.</p><a class="btn btn-ghost" style="width:100%;margin-top:20px" href="https://t.me/ghuolandservera" target="_blank" rel="noopener noreferrer">Новости магазина ↗</a></article>
    </div>
    <p class="notice">Важно: платёжная система и автоматическая выдача рангов пока не подключены. Перед оплатой уточни условия у администрации. Не отправляй никому пароль от аккаунта.</p>
  </section>

  <section class="container">
    <div class="section-head"><span class="eyebrow">ПЕРЕД СТАРТОМ</span><h2>Всё, что нужно знать</h2></div>
    <div class="info-grid">
      <article class="info-card"><h3>🖥️ Как подключиться?</h3><p>Планируется Minecraft Java Edition 1.21.11. IP-адрес будет опубликован после запуска сервера.</p></article>
      <article class="info-card"><h3>📢 Где новости?</h3><p>Все важные объявления будут выходить в официальном Telegram-канале.</p><a class="btn btn-ghost btn-small" href="https://t.me/ghuolandservera" target="_blank" rel="noopener noreferrer">Открыть Telegram ↗</a></article>
    </div>
  </section>

  <section class="container">
    <div class="section-head"><span class="eyebrow">FAQ</span><h2>Частые вопросы</h2></div>
    <div class="faq">
      <details class="faq-item"><summary>Когда откроется сервер?</summary><p>Дата пока не объявлена. Следи за Telegram-каналом — там появятся новости о запуске.</p></details>
      <details class="faq-item"><summary>Какая версия Minecraft нужна?</summary><p>Планируется Minecraft Java Edition 1.21.11. Совместимость клиента будет уточнена перед запуском.</p></details>
      <details class="faq-item"><summary>Как заказать привилегию?</summary><p>Нажми «Выбрать ранг», введи игровой ник и отправь сообщение администрации в Telegram. Дождись подтверждения условий и способа оплаты.</p></details>
      <details class="faq-item"><summary>Можно ли уже играть?</summary><p>Сервер ещё готовится к открытию. IP появится после запуска.</p></details>
    </div>
  </section>
</main>

<footer><div class="container footer-inner"><div><strong>GHUO<span style="color:#a855f7">LAND</span></strong><div>© 2026 Ghuo Land · Minecraft community</div></div><div class="footer-links"><a href="#home">Наверх ↑</a><a href="https://t.me/ghuolandservera" target="_blank" rel="noopener noreferrer">Telegram ↗</a><a href="https://t.me/ME_ghuo" target="_blank" rel="noopener noreferrer">Связаться с админом ↗</a></div></div></footer>

<div class="modal" id="buyModal" role="dialog" aria-modal="true" aria-labelledby="modalTitle">
  <div class="modal-box">
    <button class="close" type="button" onclick="closeModal()" aria-label="Закрыть окно">✕</button>
    <span class="eyebrow">МАГАЗИН GHUO LAND</span><h2 id="modalTitle">Твой заказ</h2><p id="selectedRank"></p>
    <form id="orderForm"><label for="nickname">Minecraft Java ник</label><input id="nickname" name="nickname" type="text" minlength="3" maxlength="16" pattern="[A-Za-z0-9_]{3,16}" placeholder="Например, GhuoPlayer" autocomplete="off" required><button class="btn" type="submit">Отправить заявку ↗</button></form>
    <p class="notice">Откроется Telegram с готовым сообщением администрации. Заказ не означает, что оплата произведена. Никогда не указывай пароль.</p>
  </div>
</div>
<script>
  const ADMIN = "https://t.me/ME_ghuo";
  let selected = {name:"",price:0};
  const modal = document.getElementById("buyModal");
  function buy(name,price){
    selected={name,price};
    document.getElementById("selectedRank").textContent=`Привилегия ${name} — ${price} ₽`;
    modal.classList.add("open");
    document.getElementById("nickname").focus();
  }
  function closeModal(){modal.classList.remove("open")}
  document.getElementById("orderForm").addEventListener("submit",function(event){
    event.preventDefault();
    const nickname=document.getElementById("nickname").value.trim();
    if(!/^[A-Za-z0-9_]{3,16}$/.test(nickname)){alert("Ник должен содержать 3–16 английских букв, цифр или символов _.");return}
    const message=`Здравствуйте! Хочу заказать привилегию ${selected.name} на Ghuo Land.\nMinecraft ник: ${nickname}\nЦена: ${selected.price} ₽\nПожалуйста, подтвердите условия и способ оплаты.`;
    window.open(ADMIN+"?text="+encodeURIComponent(message),"_blank","noopener,noreferrer");
  });
  modal.addEventListener("click",event=>{if(event.target===modal)closeModal()});
  document.addEventListener("keydown",event=>{if(event.key==="Escape")closeModal()});
</script>
</body>
</html>
