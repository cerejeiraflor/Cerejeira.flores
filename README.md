[cerejeira-flores-codigo.html](https://github.com/user-attachments/files/34319175/cerejeira-flores-codigo.html)
<!DOCTYPE html>
<html lang="pt-BR"><head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Cerejeira.Flores – Catálogo</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:wght@600;800&amp;family=Figtree:wght@400;500;600&amp;display=swap" rel="stylesheet">
<style>
:root{--bg:#FFF6F8;--surface:#FFFFFF;--ink:#2B2230;--muted:#6E6277;--accent:#B02A5B;--accent-ink:#FFFFFF;--leaf:#2E6B4A;--line:#EBD9E0;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#1E1722;--surface:#2A2130;--ink:#F6ECF1;--muted:#B8A9C0;--accent:#F08AB0;--accent-ink:#2B1020;--leaf:#7FCB9F;--line:#45384D;color-scheme:dark}}
:root[data-theme="dark"]{--bg:#1E1722;--surface:#2A2130;--ink:#F6ECF1;--muted:#B8A9C0;--accent:#F08AB0;--accent-ink:#2B1020;--leaf:#7FCB9F;--line:#45384D;color-scheme:dark}
*,*::before,*::after{box-sizing:border-box}
[hidden]{display:none!important}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--ink);font-family:Figtree,system-ui,sans-serif;font-size:16px;line-height:1.5;padding-bottom:96px}
h1,h2,h3{font-family:'Bricolage Grotesque',Georgia,serif;margin:0;line-height:1.1}
header{padding:40px 20px 20px;max-width:960px;margin:0 auto}
header h1{font-size:clamp(2.2rem,9vw,3.8rem);font-weight:800;letter-spacing:-.02em}
header p{color:var(--muted);max-width:46ch;margin:12px 0 0}
.edit{margin-top:14px;background:var(--surface);color:var(--ink);border:1.5px solid var(--line);border-radius:10px;padding:8px 14px;font-weight:600}
.chips{display:flex;gap:8px;overflow-x:auto;padding:8px 20px 16px;max-width:960px;margin:0 auto}
.chip{flex:none;border:1.5px solid var(--line);background:var(--surface);color:var(--ink);border-radius:999px;padding:8px 16px;font:inherit;font-weight:500;cursor:pointer}
.chip[aria-pressed="true"]{background:var(--leaf);border-color:var(--leaf);color:var(--bg)}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(230px,1fr));gap:16px;padding:0 20px;max-width:960px;margin:0 auto}
.card{background:var(--surface);border:1px solid var(--line);border-radius:18px;overflow:hidden;display:flex;flex-direction:column}
.art{height:150px;display:grid;place-items:center;font-size:76px}
img.art{display:block;width:100%;object-fit:cover}
.pic{position:relative}
.gal{display:flex;align-items:center;background:var(--surface);overflow-x:auto;scroll-snap-type:x mandatory}
.gal img{flex:none;width:100%;height:auto;max-height:340px;object-fit:contain;scroll-snap-align:center}
.badge{position:absolute;right:8px;bottom:8px;background:rgba(0,0,0,.65);color:#fff;border-radius:999px;padding:2px 10px;font-size:.8rem}
.thumbs{display:flex;gap:10px;flex-wrap:wrap;margin-top:8px}
.th{position:relative}
.th img{width:64px;height:64px;object-fit:contain;background:var(--line);border-radius:8px;display:block}
.th button{position:absolute;top:-6px;right:-6px;width:22px;height:22px;border-radius:50%;border:0;background:var(--accent);color:var(--accent-ink);line-height:1;padding:0}
.body{padding:14px 16px 16px;display:flex;flex-direction:column;gap:6px;flex:1}
.body h3{font-size:1.15rem}
.body p{margin:0;color:var(--muted);font-size:.92rem;flex:1}
.row{display:flex;align-items:center;justify-content:space-between;gap:8px;margin-top:8px}
.price{font-weight:600;font-size:1.1rem}
button{font:inherit;cursor:pointer}
button:focus-visible,input:focus-visible,select:focus-visible,textarea:focus-visible{outline:3px solid var(--accent);outline-offset:2px}
.add{background:var(--accent);color:var(--accent-ink);border:0;border-radius:12px;padding:9px 16px;font-weight:600}
.qty{display:flex;align-items:center;gap:4px}
.qty button{width:36px;height:36px;border-radius:10px;border:1.5px solid var(--line);background:var(--surface);color:var(--ink);font-size:1.2rem}
.qty span{min-width:26px;text-align:center;font-weight:600}
.bar{position:fixed;left:0;right:0;bottom:0;background:var(--surface);border-top:1px solid var(--line);padding:12px 20px calc(12px + env(safe-area-inset-bottom,0px));display:flex;align-items:center;justify-content:space-between;gap:12px;z-index:5}
.bar b{font-size:1.1rem}
.bar small{display:block;color:var(--muted)}
.bar button{background:var(--accent);color:var(--accent-ink);border:0;border-radius:12px;padding:12px 20px;font-weight:600}
.bar button:disabled{opacity:.45;cursor:not-allowed}
.sheet{position:fixed;inset:0;background:rgba(20,10,25,.55);display:none;align-items:flex-end;justify-content:center;z-index:10}
.sheet.open{display:flex}
.panel{background:var(--bg);width:100%;max-width:560px;max-height:92%;overflow-y:auto;border-radius:22px 22px 0 0;padding:20px 20px calc(20px + env(safe-area-inset-bottom,0px))}
.panel h2{font-size:1.5rem;margin-bottom:12px}
.panel h3{font-size:1.1rem;margin-top:22px}
.item{display:flex;justify-content:space-between;gap:10px;padding:8px 0;border-bottom:1px solid var(--line)}
label{display:block;font-weight:500;margin-top:14px;margin-bottom:4px}
input,select,textarea{width:100%;font:inherit;padding:10px 12px;border-radius:10px;border:1.5px solid var(--line);background:var(--surface);color:var(--ink)}
.total{display:flex;justify-content:space-between;font-size:1.2rem;font-weight:600;margin-top:16px}
.send{width:100%;margin-top:16px;background:var(--leaf);color:var(--bg);border:0;border-radius:12px;padding:14px;font-weight:600;font-size:1rem;display:block;text-align:center;text-decoration:none}
.ghost{width:100%;margin-top:8px;background:none;border:0;color:var(--muted);padding:10px}
.hint{color:var(--muted);font-size:.88rem;margin:4px 0 0}
.two{display:grid;grid-template-columns:1fr 1fr;gap:8px}
.adm{border:1px solid var(--line);border-radius:14px;padding:4px 12px 12px;margin-top:12px;background:var(--surface)}
.mini{background:none;border:1.5px solid var(--line);color:var(--ink);border-radius:8px;padding:6px 10px;margin-top:10px}
.danger{color:var(--accent)}
.low{color:var(--accent)}
.stk{display:flex;gap:8px;align-items:center}
.stk .mini{margin-top:0;flex:none;min-width:48px}
.add:disabled{opacity:.45;cursor:not-allowed}
.closedMsg{max-width:920px;width:calc(100% - 40px);margin:20px auto;padding:28px 20px;text-align:center;background:var(--surface);border:1px solid var(--line);border-radius:18px}
.closedMsg p{color:var(--muted);margin:8px 0 0}
.chk{display:flex;align-items:center;gap:10px;font-weight:600;margin:14px 0 4px}
.chk input{width:auto}
@media (prefers-reduced-motion:no-preference){.card{transition:transform .15s}.card:hover{transform:translateY(-3px)}}
</style>
</head>
<body data-closed="0">
<header>
  <h1 id="shop">Cerejeira.Flores</h1>
  <p>Escolha seus maços, preencha seus dados e envie o pedido direto no WhatsApp da loja.</p>
  <button class="edit" id="adminBtn" hidden="">Editar loja</button>
</header>
<div class="chips" id="chips" role="group" aria-label="Filtrar por ocasião"></div>
<div class="closedMsg" id="closedMsg" hidden=""><h2>Pedidos pausados no momento</h2><p>Volte em breve para fazer seu pedido de flores.</p></div>
<main class="grid" id="grid"></main>

<div class="bar">
  <div><b id="total">R$&nbsp;0,00</b><small id="count">Nenhum maço escolhido</small></div>
  <button id="open" disabled="">Ver pedido</button>
</div>

<div class="sheet" id="sheet" role="dialog" aria-modal="true" aria-labelledby="ptitle">
  <div class="panel">
    <h2 id="ptitle">Seu pedido</h2>
    <div id="items"></div>
    <div class="total"><span>Total</span><span id="sum">R$&nbsp;0,00</span></div>
    <h3>Seus dados</h3>
    <label for="name">Nome</label>
    <input id="name" autocomplete="name">
    <label for="kind">Você é</label>
    <select id="kind"><option>Pessoa física</option><option>Pessoa jurídica</option></select>
    <label for="phone">Telefone</label>
    <input id="phone" type="tel" autocomplete="tel" placeholder="(11) 90000-0000">
    <p class="hint">Seus dados ficam salvos neste aparelho para o próximo pedido.</p>
    <h3>Recebimento</h3>
    <label for="mode">Como quer receber?</label>
    <select id="mode"><option value="Retirar pessoalmente">Retirar pessoalmente</option><option value="Entrega">Entregador</option></select>
    <label for="day">Dia desejado</label>
    <select id="day"><option>Segunda-feira</option><option>Sexta-feira</option></select>
    <label for="time">Horário desejado</label>
    <select id="time"><option>22h</option><option>23h</option><option>00h (meia-noite)</option><option>01h (madrugada)</option><option>02h (madrugada)</option></select>
    <p class="hint">Atendemos às segundas e sextas, das 22h às 2h da manhã.</p>
    <label for="msg">Observação (opcional)</label>
    <textarea id="msg" rows="3" placeholder="Escreva aqui uma mensagem ou observação para o pedido"></textarea>
    <p class="hint">O endereço e o valor da entrega são combinados com a loja pelo WhatsApp.</p>
    <a class="send" id="send" href="#" target="_blank" rel="noopener">Enviar pedido pelo WhatsApp</a>
    <div id="fb" hidden=""><p class="hint">Se o WhatsApp não abriu, copie o pedido abaixo e envie para a loja: <b>(11) 96639-5690</b>.</p><textarea id="fbText" rows="6" readonly=""></textarea><button class="mini" id="fbCopy" type="button">Copiar pedido</button></div>
    <button class="ghost" id="close">Voltar ao catálogo</button>
  </div>
</div>

<div class="sheet" id="admin" role="dialog" aria-modal="true" aria-labelledby="atitle">
  <div class="panel">
    <h2 id="atitle">Editar maços</h2>
    <p class="hint">Mude nomes, preços e fotos. Nada muda para os clientes até você tocar em Salvar e publicar.</p>
    <label class="chk"><input type="checkbox" id="admOpen"> Loja aberta para pedidos</label>
    <p class="hint">Desmarque para pausar: os clientes veem "Pedidos pausados no momento" e não conseguem pedir.</p>
    <div id="adminList"></div>
    <button class="mini" id="admAdd" type="button">+ Adicionar maço</button>
    <p class="hint" id="admMsg" role="status">Publicando…</p>
    <button class="send" id="admSave">Salvar e publicar</button>
    <button class="ghost" id="admClose">Fechar</button>
  </div>
</div>

<script id="data" type="application/json">[{"id":1,"n":"Rosas vermelhas","d":"Maço com 12 rosas de talo longo.","p":89.9,"o":"Amor","e":"🌹","c":"#F7C6D0","imgs":["/_blob/43807e976c7deb619b874dc832dc4958","/_blob/e4630d3dde0afaa9c7dfb86ace4b91d0","/_blob/20e711ff33abe5cfa442e0ff52ae399a"],"s":2},{"id":2,"n":"Tulipas mistas","d":"10 tulipas em cores variadas.","p":79.9,"o":"Agradecer","e":"🌷","c":"#F9D3E3"},{"id":3,"n":"Girassóis do campo","d":"6 girassóis grandes e alegres.","p":59.9,"o":"Aniversário","e":"🌻","c":"#FBE29A"},{"id":4,"n":"Lavanda perfumada","d":"Maço de lavanda para perfumar a casa.","p":49.9,"o":"Agradecer","e":"🪻","c":"#D9CCF2"},{"id":5,"n":"Buquê romântico","d":"Rosas e lisianthus com folhagem.","p":129.9,"o":"Amor","e":"💐","c":"#F5B9C9"},{"id":6,"n":"Margaridas frescas","d":"15 margaridas para o dia a dia.","p":39.9,"o":"Aniversário","e":"🌼","c":"#FFF0B3"},{"id":7,"n":"Cravos rosa","d":"Maço com 12 cravos que duram muito.","p":44.9,"o":"Agradecer","e":"🌸","c":"#FAD1DC"},{"id":8,"n":"Buquê de noiva branco","d":"Flores brancas, sob encomenda.","p":189.9,"o":"Casamento","e":"🪷","c":"#E6E9F5"}]</script>
<script>
const SHOP="Cerejeira.Flores",WHATSAPP="5511966395690";
const $=id=>document.getElementById(id);
const esc=s=>String(s==null?'':s).replace(/[&<>"']/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]));
const brl=v=>Number(v||0).toLocaleString('pt-BR',{style:'currency',currency:'BRL'});
let products=JSON.parse($('data').textContent);
const cart={};let filter="Todos",art=null,assets=null;
document.title=SHOP+" – Catálogo";

function chips(){
  const cats=["Todos",...new Set(products.map(p=>p.o).filter(Boolean))];
  if(!cats.includes(filter))filter="Todos";
  $('chips').innerHTML=cats.map(c=>`<button class="chip" aria-pressed="${c===filter}" data-c="${esc(c)}">${esc(c)}</button>`).join('');
}
function grid(){
  chips();
  $('grid').innerHTML=products.filter(p=>filter==="Todos"||p.o===filter).map(p=>{
    const q=cart[p.id]||0;const hasS=p.s!==undefined&&p.s!==null&&p.s!=="";const out=hasS&&+p.s<=0;
    const ctl=q?`<div class="qty"><button data-m="${p.id}" aria-label="Diminuir">−</button><span>${q}</span><button data-a="${p.id}" aria-label="Aumentar"${hasS&&q>=+p.s?' disabled':''}>+</button></div>`
                :(out?`<button class="add" disabled>Esgotado</button>`:`<button class="add" data-a="${p.id}">Adicionar</button>`);
    const im=p.imgs||(p.img?[p.img]:[]);
    const pic=im.length?`<div class="pic"><div class="gal">${im.map(u=>`<img src="${esc(u)}" alt="${esc(p.n)}" loading="lazy">`).join('')}</div>${im.length>1?`<span class="badge">📷 ${im.length} · deslize</span>`:''}</div>`:`<div class="art" style="background:${esc(p.c)}" aria-hidden="true">${esc(p.e)}</div>`;
    return `<article class="card">${pic}<div class="body"><h3>${esc(p.n)}</h3><p>${esc(p.d)}${hasS&&!out&&+p.s<=5?`<br><b class="low">Restam só ${+p.s}</b>`:''}</p><div class="row"><span class="price">${brl(p.p)}</span>${ctl}</div></div></article>`;
  }).join('');
}
function totals(){
  let n=0,s=0;products.forEach(p=>{const q=cart[p.id]||0;n+=q;s+=q*p.p});
  $('total').textContent=brl(s);$('sum').textContent=brl(s);
  $('count').textContent=n?`${n} ${n===1?'maço':'maços'} no pedido`:'Nenhum maço escolhido';
  $('open').disabled=!n;
  $('items').innerHTML=products.filter(p=>cart[p.id]).map(p=>`<div class="item"><span>${cart[p.id]}× ${esc(p.n)}</span><span>${brl(cart[p.id]*p.p)}</span></div>`).join('');
  return {n,s};
}
function change(id,d){const pr=products.find(x=>x.id===id);let v=Math.max(0,(cart[id]||0)+d);if(pr&&pr.s!==undefined&&pr.s!==null&&pr.s!==""&&v>+pr.s)v=Math.max(0,+pr.s);cart[id]=v;if(!cart[id])delete cart[id];grid();if(!totals().n)$('sheet').classList.remove('open')}
$('chips').onclick=e=>{const c=e.target.dataset.c;if(c){filter=c;grid()}};
$('grid').onclick=e=>{const b=e.target.closest('button');if(!b)return;if(b.dataset.a)change(+b.dataset.a,1);if(b.dataset.m)change(+b.dataset.m,-1)};
$('open').onclick=()=>$('sheet').classList.add('open');
$('close').onclick=()=>$('sheet').classList.remove('open');

// Dados do comprador, salvos só neste aparelho
const KEYS=['name','kind','phone'];
try{const d=JSON.parse(localStorage.getItem('cf_cliente')||'{}');KEYS.forEach(k=>{if(d[k])$(k).value=d[k]})}catch(e){}
function saveClient(){try{const d={};KEYS.forEach(k=>d[k]=$(k).value.trim());localStorage.setItem('cf_cliente',JSON.stringify(d))}catch(e){}}
const need=id=>{if(!$(id).value.trim()){$(id).focus();return true}return false};
$('send').onclick=e=>{
  const {n,s}=totals();if(!n){e.preventDefault();return}
  const delivery=$('mode').value==="Entrega";
  if(need('name')||need('phone')){e.preventDefault();return}
  saveClient();
  const lines=products.filter(p=>cart[p.id]).map(p=>`• ${cart[p.id]}× ${p.n} – ${brl(cart[p.id]*p.p)}`);
  let t=`Olá! Quero fazer um pedido:\n${lines.join('\n')}\nTotal: ${brl(s)}\n\nNome: ${$('name').value.trim()} (${$('kind').value})\nTelefone: ${$('phone').value.trim()}\n${$('mode').value}`;
  t+=`\nQuando: ${$('day').value}, às ${$('time').value}`;
  if($('msg').value.trim())t+=`\nObservação: ${$('msg').value.trim()}`;
  $('send').href=`https://wa.me/${WHATSAPP}?text=${encodeURIComponent(t)}`;
  $('fbText').value=t;$('fb').hidden=false;
};

$('fbCopy').onclick=async()=>{const t=$('fbText');try{await navigator.clipboard.writeText(t.value);$('fbCopy').textContent='Copiado!'}catch(e){t.select();$('fbCopy').textContent='Selecione e copie o texto'}};
// Área da dona: só aparece para quem é dona desta página
(async()=>{try{
  if(!window.claude||!claude.use)return;
  const u=await claude.use('user');
  if(u&&u.isOwner()){art=await claude.use('artifact');assets=await claude.use('assets');if(art)$('adminBtn').hidden=false}
}catch(e){}})();
const prodOf=el=>products.find(p=>p.id===+el.closest('.adm').dataset.id);
function adminRender(){
  $('adminList').innerHTML=products.map(p=>`<div class="adm" data-id="${p.id}">
    <label>Nome</label><input data-k="n" value="${esc(p.n)}">
    <div class="two"><div><label>Preço (R$)</label><input data-k="p" type="number" step="0.01" min="0" value="${p.p}"></div>
    <div><label>Ocasião</label><input data-k="o" value="${esc(p.o)}"></div></div>
    <label>Descrição</label><input data-k="d" value="${esc(p.d)}">
    <label>Estoque (deixe vazio para não controlar)</label><div class="stk"><button type="button" class="mini" data-st="-1" aria-label="Tirar 1 do estoque">−1</button><input data-k="s" type="number" min="0" step="1" value="${p.s===undefined||p.s===null?'':p.s}"><button type="button" class="mini" data-st="1" aria-label="Somar 1 ao estoque">+1</button></div>
    <label>Fotos (pode escolher várias)</label><input type="file" accept="image/*" multiple data-f="1">
    <div class="thumbs">${(p.imgs||(p.img?[p.img]:[])).map((u,i)=>`<span class="th"><img src="${esc(u)}" alt=""><button type="button" data-rm="${i}" aria-label="Tirar foto">×</button></span>`).join('')}</div>
    <button type="button" class="mini danger" data-del="1">Remover maço</button></div>`).join('');
}
$('adminBtn').onclick=()=>{$('admOpen').checked=!closed;adminRender();$('admMsg').textContent='';$('admin').classList.add('open')};
$('admClose').onclick=()=>$('admin').classList.remove('open');
$('admAdd').onclick=()=>{products.push({id:Math.max(0,...products.map(p=>p.id))+1,n:"Novo maço",d:"",p:0,o:"Outros",e:"🌸",c:"#F9D3E3"});adminRender();grid();totals()};
$('adminList').oninput=e=>{const k=e.target.dataset.k;if(!k)return;const p=prodOf(e.target);p[k]=k==='p'?(parseFloat(e.target.value)||0):k==='s'?(e.target.value===''?'':Math.max(0,parseInt(e.target.value,10)||0)):e.target.value;grid();totals()};
$('adminList').onclick=e=>{
  const b=e.target.closest('button');if(!b)return;const p=prodOf(b);
  if(b.dataset.del){products=products.filter(x=>x.id!==p.id);delete cart[p.id];adminRender();grid();totals()}
  if(b.dataset.st){if(p.s===undefined||p.s===null||p.s==='')return;p.s=Math.max(0,+p.s+(+b.dataset.st));adminRender();grid();totals();return}
  if(b.dataset.rm!==undefined){const l=p.imgs||(p.img?[p.img]:[]);l.splice(+b.dataset.rm,1);p.imgs=l;delete p.img;adminRender();grid()}
};
$('adminList').onchange=async e=>{
  if(!e.target.dataset.f)return;const fs=[...(e.target.files||[])];if(!fs.length)return;
  if(!assets){$('admMsg').textContent='Envio de fotos indisponível agora.';return}
  const p=prodOf(e.target);$('admMsg').textContent='Enviando foto…';
  try{const l=(p.imgs||(p.img?[p.img]:[])).slice();for(const f of fs){const r=await assets.upload(f);l.push(r.url)}p.imgs=l;delete p.img;$('admMsg').textContent='Fotos enviadas.';adminRender();grid()}
  catch(err){$('admMsg').textContent='Não foi possível enviar a foto. Tente uma imagem menor.'}
};
$('admSave').onclick=async()=>{
  $('admMsg').textContent='Publicando…';
  try{
    const c=document.documentElement.cloneNode(true);
    ['grid','chips','items','adminList'].forEach(i=>c.querySelector('#'+i).replaceChildren());
    c.querySelector('#data').textContent=JSON.stringify(products).replace(/</g,'\\u003c');
    c.querySelectorAll('.sheet').forEach(s=>s.classList.remove('open'));
    c.querySelector('#adminBtn').setAttribute('hidden','');
    c.querySelector('#fb').setAttribute('hidden','');
    c.querySelector('body').setAttribute('data-closed',closed?'1':'0');
    c.querySelector('#send').setAttribute('href','#');
    await art.publish('<!DOCTYPE html>\n'+c.outerHTML);
  }catch(err){$('admMsg').textContent='Não foi possível salvar ('+((err&&err.code)||'erro')+'). Tente de novo.'}
};
let closed=document.body.dataset.closed==="1";
function applyClosed(){$('closedMsg').hidden=!closed;$('chips').hidden=closed;$('grid').hidden=closed;document.querySelector('.bar').hidden=closed;if(closed)$('sheet').classList.remove('open')}
$('admOpen').onchange=()=>{closed=!$('admOpen').checked;applyClosed()};
applyClosed();
grid();totals();
</script>


</body></html>
