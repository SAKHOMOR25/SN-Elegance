<!doctype html>
<html lang="fr">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>SN-Élégance 221 — Boutique</title>
<meta name="description" content="SN-Élégance 221 — Tissus Getzner premium. Achetez au mètre : Magnum, Brocade, Wifi, Focus. Paiement Wave & Orange Money. Commande via WhatsApp."/>
<style>
  /* =========================
     Palette moderne (clair & doré)
     ========================= */
  :root{
    --ivory:#F8F6F1;
    --champagne:#C9A227;
    --sand:#E5D9C5;
    --dark:#2C2C2C;
    --accent:#006C67;
    --muted:#7a7872;
    --card:#ffffff;
    --radius:14px;
    --shadow: 0 10px 30px rgba(15,15,15,0.08);
    font-family: "Inter", "Segoe UI", Roboto, Arial, sans-serif;
    color-scheme: light;
  }
  *{box-sizing:border-box}
  html,body{height:100%;margin:0;background:linear-gradient(180deg,var(--ivory) 0%, #f3efe8 100%);color:var(--dark);-webkit-font-smoothing:antialiased}
  a{color:inherit}
  /* Header */
  header{background:transparent;padding:28px 16px;text-align:center}
  .logo{max-width:140px;margin:0 auto 6px;display:block}
  .site-title{font-size:28px;color:var(--dark);font-weight:800;letter-spacing:0.2px;margin:4px 0}
  .site-sub{color:var(--muted);margin-bottom:10px}
  .banner{
    background:linear-gradient(90deg, rgba(201,162,39,0.08), rgba(0,108,103,0.02));
    border-radius:12px;padding:10px 14px;display:inline-block;margin-top:10px;color:var(--dark);font-weight:600;
    box-shadow:var(--shadow);
  }

  main.container{max-width:1200px;margin:22px auto;padding:16px}
  .hero{display:flex;gap:18px;align-items:center;margin-bottom:20px}
  .hero .left{flex:1}
  .hero h2{margin:0;font-size:22px;color:var(--dark)}
  .hero p{color:var(--muted);margin-top:8px}
  .hero .cta{margin-top:12px;display:flex;gap:10px;flex-wrap:wrap}
  .btn{background:var(--champagne);Color:#111;padding:10px 14px;border-radius:10px;border:none;font-weight:800;cursor:pointer;box-shadow:0 8px 20px rgba(201,162,39,0.12)}
  .btn.secondary{background:transparent;border:1px solid rgba(44,44,44,0.06);color:var(--dark)}
  .btn.whatsapp{background:#25D366;color:#042b16}
  .btn.pay-wave{background:#0dbc5f;color:#042b16}
  .btn.pay-orange{background:#ff7a00;color:#fff}

  /* Grid products */
  .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:18px}
  .card{background:var(--card);border-radius:var(--radius);padding:14px;border:1px solid rgba(44,44,44,0.04);box-shadow:var(--shadow);display:flex;flex-direction:column;min-height:420px}
  .thumbs{display:flex;gap:8px;justify-content:center;margin-bottom:12px}
  .thumbs img{width:86px;height:86px;object-fit:cover;border-radius:10px;cursor:pointer;border:2px solid var(--champagne);transition:transform .12s, box-shadow .12s}
  .thumbs img:hover{transform:scale(1.04);box-shadow:0 8px 20px rgba(0,0,0,0.08)}
  .title{font-weight:800;color:var(--dark);text-align:center;margin:6px 0}
  .desc{color:var(--muted);font-size:14px;text-align:center;margin-bottom:8px}
  .price{font-weight:900;color:var(--champagne);font-size:18px;text-align:center;margin-bottom:10px}
  .card .controls{display:flex;gap:8px;align-items:center;justify-content:center;margin-top:auto}
  input[type="number"]{width:90px;padding:8px;border-radius:8px;border:1px solid rgba(44,44,44,0.06);text-align:center}

  /* Cart floating */
  aside.cart{position:fixed;right:18px;bottom:18px;width:360px;background:var(--card);border-radius:12px;padding:14px;border:1px solid rgba(44,44,44,0.06);box-shadow:0 24px 60px rgba(15,15,15,0.08);z-index:60}
  aside.cart h4{margin:0 0 8px 0;color:var(--dark)}
  .cart-list{max-height:260px;overflow:auto;margin-bottom:10px}
  .cart-row{display:flex;gap:10px;align-items:center;padding:8px;border-radius:8px;border:1px solid rgba(44,44,44,0.03);margin-bottom:8px}
  .cart-row img{width:60px;height:60px;object-fit:cover;border-radius:8px}
  .cart-row .meta{flex:1}
  .cart-row .meta .name{font-weight:800;color:var(--dark)}
  .cart-row .meta .small{color:var(--muted);font-size:13px}
  .cart-actions{display:flex;gap:6px;margin-top:8px}
  .small{font-size:13px;color:var(--muted)}
  .cart-footer{display:flex;gap:8px;margin-top:12px;flex-direction:column}

  /* Modal styles */
  .modal-back{position:fixed;inset:0;background:rgba(0,0,0,0.55);display:flex;align-items:center;justify-content:center;z-index:200}
  .modal{background:var(--card);border-radius:12px;padding:16px;max-width:920px;width:94%;display:flex;gap:14px;box-shadow:0 30px 90px rgba(0,0,0,0.12)}
  .modal .left{flex:1}
  .modal .right{width:320px}
  .modal img{width:100%;border-radius:8px}
  .modal h3{margin:0;color:var(--champagne)}
  .modal label{display:block;margin-top:8px;color:var(--muted);font-size:13px}

  /* FAQ & footer */
  .faq{margin-top:26px;background:var(--sand);padding:16px;border-radius:12px;border:1px solid rgba(44,44,44,0.04)}
  footer{margin-top:30px;padding:18px;text-align:center;color:var(--muted)}

  /* Responsive */
  @media(max-width:980px){ .grid{grid-template-columns:repeat(2,1fr)} aside.cart{width:320px} }
  @media(max-width:700px){ .grid{grid-template-columns:1fr} aside.cart{position:static;margin:16px auto;width:calc(100% - 32px)} .modal{flex-direction:column} .modal .right{width:100%} }
</style>
</head>
<body>

<header>
  <!-- Logo mis à jour -->
  <img class="logo" src="https://i.postimg.cc/fWJvXsJ4/SN-Elegange.png" alt="SN-Élégance 221">
  <div class="site-title">SN-Élégance 221</div>
  <div class="site-sub">Des tissus de prestige pour donner vie à votre élégance unique.</div>
  <div class="banner">Paiement sécurisé • Livraison locale • Commande facile via WhatsApp</div>
</header>

<main class="container">
  <section class="hero">
    <div class="left">
      <h2>Collections Getzner — Qualité & élégance</h2>
      <p>Choisissez votre tissu, sélectionnez la quantité en mètres et confirmez votre commande en quelques clics. Paiement disponible via Wave & Orange Money.</p>
      <div class="cta">
        <button class="btn" onclick="document.querySelector('.grid').scrollIntoView({behavior:'smooth'})">Voir la boutique</button>
        <button class="btn secondary" onclick="document.getElementById('cartBox').scrollIntoView({behavior:'smooth'})">Voir le panier</button>
      </div>
    </div>
    <div style="width:260px;text-align:right">
      <div style="background:var(--sand);padding:12px;border-radius:12px;border:1px solid rgba(44,44,44,0.04)">
        <div style="font-size:13px;color:var(--muted)">Sélection premium</div>
        <div style="font-weight:800;font-size:18px;color:var(--champagne);margin-top:6px">Getzner — Brocade, Magnum, Wifi, Focus</div>
      </div>
    </div>
  </section>

  <!-- Products grid -->
  <div class="grid" id="productsGrid">
    <!-- Product cards (data attributes used for modal) -->
    <!-- Magnum -->
    <article class="card product" data-name="Getzner Magnum Gold" data-price="11000" data-desc="Le tissu Getzner Magnum Gold est reconnu pour sa qualité exceptionnelle et son éclat raffiné. Idéal pour boubous et tenues de fête.">
      <div class="thumbs">
        <img src="https://i.postimg.cc/rpVfPpbQ/IMG-20250927-WA0068.jpg" alt="Magnum" data-src="https://i.postimg.cc/rpVfPpbQ/IMG-20250927-WA0068.jpg">
        <img src="https://i.postimg.cc/B6tLy5M9/IMG-20250927-WA0065.jpg" alt="Magnum" data-src="https://i.postimg.cc/B6tLy5M9/IMG-20250927-WA0065.jpg">
        <img src="https://i.postimg.cc/rFRGzTGL/IMG-20250917-WA0011.jpg" alt="Magnum" data-src="https://i.postimg.cc/rFRGzTGL/IMG-20250917-WA0011.jpg">
      </div>
      <div class="title">Getzner Magnum Gold</div>
      <div class="desc">Brillance durable • Confort premium • Tombé parfait</div>
      <div class="price">11 000 CFA / mètre</div>
      <div class="controls">
        <input type="number" min="1" value="1" class="quick-qty">
        <button class="btn" onclick="addFromCard(this)">Ajouter</button>
      </div>
    </article>

    <!-- Brocade -->
    <article class="card product" data-name="Getzner Brocade" data-price="13000" data-desc="Le Brocade est un tissu élégant aux motifs tissés, parfait pour des tenues traditionnelles et cérémonies.">
      <div class="thumbs">
        <img src="https://i.postimg.cc/RZ6SnMGb/IMG-20250927-WA0101.jpg" alt="Brocade" data-src="https://i.postimg.cc/RZ6SnMGb/IMG-20250927-WA0101.jpg">
        <img src="https://i.postimg.cc/XJ0YbTfm/IMG-20250927-WA0088.jpg" alt="Brocade" data-src="https://i.postimg.cc/XJ0YbTfm/IMG-20250927-WA0088.jpg">
        <img src="https://i.postimg.cc/7h96Xm2q/IMG-20250927-WA0087.jpg" alt="Brocade" data-src="https://i.postimg.cc/7h96Xm2q/IMG-20250927-WA0087.jpg">
      </div>
      <div class="title">Getzner Brocade</div>
      <div class="desc">Aspect raffiné • Motifs intégrés • Résistant</div>
      <div class="price">13 000 CFA / mètre</div>
      <div class="controls">
        <input type="number" min="1" value="1" class="quick-qty">
        <button class="btn" onclick="addFromCard(this)">Ajouter</button>
      </div>
    </article>

    <!-- Wifi -->
    <article class="card product" data-name="Getzner Wifi" data-price="13000" data-desc="Le tissu Wifi séduit par ses motifs originaux et sa souplesse, idéal pour un usage quotidien ou événementiel.">
      <div class="thumbs">
        <img src="https://i.postimg.cc/6QbFVR3b/IMG-20250917-WA0029-1.jpg" alt="Wifi" data-src="https://i.postimg.cc/6QbFVR3b/IMG-20250917-WA0029-1.jpg">
        <img src="https://i.postimg.cc/Wbrj293k/IMG-20250917-WA0042.jpg" alt="Wifi" data-src="https://i.postimg.cc/Wbrj293k/IMG-20250917-WA0042.jpg">
        <img src="https://i.postimg.cc/zGnQQ6fB/IMG-20250917-WA0034.jpg" alt="Wifi" data-src="https://i.postimg.cc/zGnQQ6fB/IMG-20250917-WA0034.jpg">
      </div>
      <div class="title">Getzner Wifi</div>
      <div class="desc">Motifs modernes • Léger & respirant • Polyvalent</div>
      <div class="price">13 000 CFA / mètre</div>
      <div class="controls">
        <input type="number" min="1" value="1" class="quick-qty">
        <button class="btn" onclick="addFromCard(this)">Ajouter</button>
      </div>
    </article>

    <!-- Focus -->
    <article class="card product" data-name="Getzner Focus" data-price="14000" data-desc="Le Focus se distingue par sa texture soyeuse et son tombé fluide, parfait pour des tenues modernes et élégantes.">
      <div class="thumbs">
        <img src="https://i.postimg.cc/prsjy2kW/IMG-20250927-WA0035.jpg" alt="Focus" data-src="https://i.postimg.cc/prsjy2kW/IMG-20250927-WA0035.jpg">
        <img src="https://i.postimg.cc/4dzb4krF/IMG-20250927-WA0044.jpg" alt="Focus" data-src="https://i.postimg.cc/4dzb4krF/IMG-20250927-WA0044.jpg">
        <img src="https://i.postimg.cc/Qt5SBWW9/IMG-20250927-WA0038.jpg" alt="Focus" data-src="https://i.postimg.cc/Qt5SBWW9/IMG-20250927-WA0038.jpg">
      </div>
      <div class="title">Getzner Focus</div>
      <div class="desc">Texture douce • Durable • Polyvalent</div>
      <div class="price">14 000 CFA / mètre</div>
      <div class="controls">
        <input type="number" min="1" value="1" class="quick-qty">
        <button class="btn" onclick="addFromCard(this)">Ajouter</button>
      </div>
    </article>
  </div>

  <!-- FAQ -->
  <section class="faq">
    <h3>FAQ — Livraison & Paiement</h3>
    <p><strong>Livraison locale :</strong> Nous livrons à Dakar et environs via moto/transporteur. Le tarif dépend de la distance.</p>
    <p><strong>Livraison internationale :</strong> Sur demande — contactez-nous par WhatsApp pour un devis.</p>
    <p><strong>Paiement :</strong> Wave (Promobile) et Orange Money acceptés. Vous pouvez payer via QR ou manuellement, puis confirmer via WhatsApp.</p>
    <p><strong>Annulation / Réclamation :</strong> Contactez-nous immédiatement sur WhatsApp avec la référence et le reçu.</p>
  </section>
</main>

<!-- Cart (floating) -->
<aside class="cart" id="cartBox">
  <h4>🛒 Votre Panier</h4>
  <div class="cart-list" id="cartList">Le panier est vide</div>

  <div class="cart-total" style="margin-top:8px;display:flex;justify-content:space-between;align-items:center">
    <div class="small">Total</div>
    <div id="cartTotal" style="font-weight:900;color:var(--champagne)">0 CFA</div>
  </div>

  <div class="cart-footer">
    <button class="btn whatsapp" onclick="openWhatsApp()">Commander via WhatsApp</button>
    <div class="cart-actions" style="margin-top:8px">
      <button class="btn pay-wave" onclick="openPayModal('wave')">Payer Wave</button>
      <button class="btn pay-orange" onclick="openPayModal('orange')">Payer Orange</button>
    </div>
    <div style="margin-top:8px" class="small">Après paiement, cliquez sur "J'ai payé" dans la popup et confirmez via WhatsApp.</div>
  </div>
</aside>

<!-- Modal container -->
<div id="modals"></div>

<footer>
  <div>© 2025 SN-Élégance 221</div>
  <div class="small">Téléphone : +221 75 443 7491 • +221 78 432 4745</div>
</footer>

<script>
/* =========================
   Config / Numéros
   ========================= */
const WHATSAPP_NUMBER = "221754437491"; // numéro pour recevoir confirmation (WhatsApp)
const WAVE_NUMBER = "+221754437491";    // Wave (Promobile)
const ORANGE_NUMBER = "+221784324745";  // Orange Money

/* =========================
   Cart state (persisted)
   ========================= */
let CART = JSON.parse(localStorage.getItem('sn_cart_sn221') || '[]');
function saveCart(){ localStorage.setItem('sn_cart_sn221', JSON.stringify(CART)); }

/* Helpers */
const money = n => n.toLocaleString() + " CFA";

/* Render cart */
function renderCart(){
  const list = document.getElementById('cartList');
  const totalEl = document.getElementById('cartTotal');
  list.innerHTML = '';
  if(CART.length===0){ list.textContent = "Le panier est vide"; totalEl.textContent = "0 CFA"; return; }
  let total = 0;
  CART.forEach((it, idx)=>{
    total += it.price * it.qty;
    const row = document.createElement('div');
    row.className = 'cart-row';
    row.innerHTML = `
      <img src="${it.img}" alt="${it.name}">
      <div class="meta">
        <div class="name">${it.name}</div>
        <div class="small">${it.qty} m • ${money(it.price)} / m</div>
      </div>
      <div style="text-align:right">
        <div style="font-weight:900">${money(it.price * it.qty)}</div>
        <div style="display:flex;gap:6px;margin-top:6px;justify-content:flex-end">
          <button class="btn secondary" onclick="changeQty(${idx},1)">+</button>
          <button class="btn secondary" onclick="changeQty(${idx},-1)">−</button>
          <button class="btn secondary" onclick="removeItem(${idx})">Suppr</button>
        </div>
      </div>
    `;
    list.appendChild(row);
  });
  totalEl.textContent = total.toLocaleString() + " CFA";
}

/* Add to cart helper */
function addToCart(item){
  // item: {name, price, qty, img}
  const existing = CART.find(i => i.name === item.name);
  if(existing){ existing.qty += item.qty; }
  else CART.push({...item});
  saveCart();
  renderCart();
}

/* Remove / change qty */
function removeItem(idx){ CART.splice(idx,1); saveCart(); renderCart(); }
function changeQty(idx, delta){
  if(!CART[idx]) return;
  CART[idx].qty = Math.max(0, CART[idx].qty + delta);
  if(CART[idx].qty === 0) CART.splice(idx,1);
  saveCart();
  renderCart();
}

/* Quick add from card controls */
function addFromCard(buttonEl){
  const card = buttonEl.closest('.product');
  const name = card.dataset.name;
  const price = parseInt(card.dataset.price,10);
  const qty = Math.max(1, parseInt(card.querySelector('.quick-qty').value || 1,10));
  const img = card.querySelector('.thumbs img').getAttribute('data-src');
  addToCart({name, price, qty, img});
}

/* Open Buy Modal when clicking a thumbnail */
document.querySelectorAll('.thumbs img').forEach(img=>{
  img.addEventListener('click', (e)=>{
    openBuyModal(img);
  });
});

/* Buy modal (image click) */
function openBuyModal(imgEl){
  const card = imgEl.closest('.product');
  const name = card.dataset.name;
  const price = parseInt(card.dataset.price,10);
  const desc = card.dataset.desc;
  const imgSrc = imgEl.dataset.src || imgEl.src;

  const modalBack = document.createElement('div');
  modalBack.className = 'modal-back';
  modalBack.innerHTML = `
    <div class="modal" role="dialog" aria-modal="true">
      <div class="left">
        <img src="${imgSrc}" alt="${name}">
      </div>
      <div class="right">
        <h3>${name}</h3>
        <div class="small">${desc}</div>
        <div style="margin-top:8px" class="small">Prix : <strong>${money(price)}</strong> / mètre</div>

        <label>Quantité (mètres)</label>
        <input type="number" id="modalQty" min="1" value="1">

        <label>Nom (optionnel)</label>
        <input type="text" id="modalName" placeholder="Votre nom">

        <label>Téléphone (optionnel)</label>
        <input type="text" id="modalPhone" placeholder="+221 ...">

        <label>Remarques (optionnel)</label>
        <input type="text" id="modalNotes" placeholder="Ex: tissu pour robe, livraison demain">

        <div style="margin-top:10px" class="small">Total : <strong id="modalTotal">${money(price)}</strong></div>

        <div style="margin-top:12px;display:flex;gap:8px">
          <button class="btn" id="modalAddBtn">Ajouter au panier</button>
          <button class="btn secondary" id="modalCloseBtn">Fermer</button>
        </div>
      </div>
    </div>
  `;
  document.getElementById('modals').appendChild(modalBack);

  const qtyInput = modalBack.querySelector('#modalQty');
  const totalEl = modalBack.querySelector('#modalTotal');
  const nameInput = modalBack.querySelector('#modalName');
  const phoneInput = modalBack.querySelector('#modalPhone');
  const notesInput = modalBack.querySelector('#modalNotes');

  const update = ()=> {
    const q = Math.max(1, parseInt(qtyInput.value||1,10));
    totalEl.textContent = money(q * price);
  };
  qtyInput.addEventListener('input', update);

  modalBack.querySelector('#modalCloseBtn').addEventListener('click', ()=> modalBack.remove());
  modalBack.querySelector('#modalAddBtn').addEventListener('click', ()=>{
    const q = Math.max(1, parseInt(qtyInput.value||1,10));
    const nameVal = nameInput.value.trim();
    const phoneVal = phoneInput.value.trim();
    const notesVal = notesInput.value.trim();
    addToCart({name, price, qty: q, img: imgSrc, buyerName: nameVal, buyerPhone: phoneVal, notes: notesVal});
    modalBack.remove();
  });
}

/* WhatsApp order (pre-fill) */
function openWhatsApp(){
  if(CART.length===0){ alert("Le panier est vide."); return; }
  let msg = "Bonjour,%0AJ'aimerais commander :%0A";
  let total = 0;
  CART.forEach(it=>{
    msg += `- ${it.qty} m de ${it.name} -> ${money(it.price * it.qty)}%0A`;
    if(it.notes) msg += `  Remarque: ${encodeURIComponent(it.notes)}%0A`;
    total += it.price * it.qty;
  });
  msg += `Total : ${total.toLocaleString()} CFA%0A%0ANom : %0ATéléphone : %0AAdresse :`;
  const url = `https://wa.me/${WHATSAPP_NUMBER}?text=${encodeURIComponent(decodeURIComponent(msg))}`;
  window.open(url, '_blank');
}

/* Payment modal for Wave / Orange */
function openPayModal(method){
  if(CART.length===0){ alert("Le panier est vide."); return; }
  const total = CART.reduce((s,it)=> s + it.price * it.qty, 0);
  const number = method === 'wave' ? WAVE_NUMBER : ORANGE_NUMBER;
  const label = method === 'wave' ? 'Wave (Promobile)' : 'Orange Money';
  const qrText = `${label} ${number} Montant:${total}CFA`;
  const qrUrl = `https://chart.googleapis.com/chart?chs=260x260&cht=qr&chl=${encodeURIComponent(qrText)}`;

  const modalBack = document.createElement('div');
  modalBack.className = 'modal-back';
  modalBack.innerHTML = `
    <div class="modal" role="dialog">
      <div style="flex:1">
        <h3>${label}</h3>
        <div class="small">Numéro : <strong>${number}</strong></div>
        <div class="small">Montant : <strong>${total.toLocaleString()} CFA</strong></div>
        <div style="margin-top:10px" class="small">Scannez le QR pour effectuer le paiement ou payez manuellement puis cliquez sur "J'ai payé" pour confirmer.</div>
        <div style="margin-top:12px"><img src="${qrUrl}" alt="QR Code" style="max-width:220px;border:6px solid #fff;border-radius:10px"></div>
        <label>Référence paiement (ex: transaction ID)</label>
        <input type="text" id="payRef" placeholder="Ex: REF12345">
      </div>
      <div style="width:200px;display:flex;flex-direction:column;gap:8px;align-items:center">
        <button class="btn" id="paidConfirm">J'ai payé — Confirmer</button>
        <button class="btn secondary" id="payClose">Fermer</button>
      </div>
    </div>
  `;
  document.getElementById('modals').appendChild(modalBack);

  modalBack.querySelector('#payClose').addEventListener('click', ()=> modalBack.remove());
  modalBack.querySelector('#paidConfirm').addEventListener('click', ()=>{
    const ref = modalBack.querySelector('#payRef').value.trim();
    // send confirmation via WhatsApp with order details + ref
    let msg = `Bonjour, j'ai effectué un paiement de ${total.toLocaleString()} CFA via ${label} (${number}).%0ARéférence: ${encodeURIComponent(ref)}%0ACommande:%0A`;
    CART.forEach(it => msg += `- ${it.qty} m de ${it.name} -> ${money(it.price * it.qty)}%0A`);
    msg += `Total : ${total.toLocaleString()} CFA%0A%0ANom :%0ATéléphone :%0AAdresse :`;
    const wa = `https://wa.me/${WHATSAPP_NUMBER}?text=${encodeURIComponent(decodeURIComponent(msg))}`;
    window.open(wa, '_blank');
    modalBack.remove();
  });
}

/* Init render */
renderCart();

/* Save on unload */
window.addEventListener('beforeunload', saveCart);
</script>
</body>
</html>
