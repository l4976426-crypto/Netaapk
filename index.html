<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <style>
        body { 
            font-family: sans-serif; background: #fff; margin: 0; 
            height: 100vh; overflow: hidden; touch-action: none; 
        }
        
        /* Painel */
        #painel {
            width: 260px; background: rgba(20, 20, 20, 0.95);
            border: 2px solid #ff0033; border-radius: 10px;
            padding: 15px; color: white; position: absolute;
            top: 50px; left: 120px; z-index: 1000;
        }

        .header { text-align: center; color: #ff0033; font-weight: bold; margin-bottom: 10px; }
        .row { display: flex; justify-content: space-between; align-items: center; margin: 10px 0; }

        /* Botões Flutuantes */
        .btn-float {
            width: 60px; height: 60px; border-radius: 50%;
            display: flex; align-items: center; justify-content: center;
            position: absolute; font-size: 10px; font-weight: bold;
            color: white; border: 2px solid white; z-index: 1001;
            box-shadow: 0 4px 10px rgba(0,0,0,0.5);
            transition: opacity 0.3s, background 0.3s; /* Transição suave para a invisibilidade */
        }
        
        #btn-freeze { background: #550000; top: 100px; left: 20px; }
        #btn-ghost { background: #330055; top: 180px; left: 20px; }
        #btn-menu { background: #004400; top: 260px; left: 20px; }

        /* Estilo quando invisível: esconde mas continua clicável */
        .esta-invisivel {
            opacity: 0 !important;
        }

        #btn-exit {
            width: 25px; height: 25px; background: #ff0033;
            color: white; border-radius: 50%; position: absolute;
            top: -10px; right: -10px; border: none; font-weight: bold;
        }

        .on-freeze { background: red !important; box-shadow: 0 0 15px red !important; }
        .on-ghost { background: #a020f0 !important; box-shadow: 0 0 15px #a020f0 !important; }
        
        .close-btn { 
            background: #333; border: 1px solid #ff0033; color: white;
            width: 100%; padding: 8px; margin-top: 10px; border-radius: 5px;
        }

        input[type=range] { width: 100%; accent-color: #ff0033; }
    </style>
</head>
<body>

<div id="painel" class="draggable">
    <button id="btn-exit" onclick="location.reload()">X</button>
    <div class="header">KM INJECTOR CLONE</div>
    
    <div class="row">
        <span>VPN</span>
        <input type="checkbox" id="vpn-check">
    </div>

    <hr style="border: 0; border-top: 1px solid #444;">

    <label id="lbl-freeze">FREEZE (0 - 100MB)</label>
    <input type="range" min="0" max="100" value="0" id="range-freeze">
    
    <label id="lbl-ghost">GHOST (0 - 100MB)</label>
    <input type="range" min="0" max="100" value="0" id="range-ghost">

    <label>TAMANHO DOS BOTÕES</label>
    <input type="range" min="40" max="120" value="60" id="range-size" oninput="mudarTamanho(this.value)">

    <div class="row">
        <span>Botões Invisíveis</span>
        <input type="checkbox" id="check-invisible" onchange="toggleVisibility()">
    </div>

    <button class="close-btn" onclick="document.getElementById('painel').style.display='none'">FECHAR PAINEL</button>
</div>

<button id="btn-freeze" class="btn-float draggable" onclick="toggleStatus('freeze')">FREEZE</button>
<button id="btn-ghost" class="btn-float draggable" onclick="toggleStatus('ghost')">GHOST</button>
<button id="btn-menu" class="btn-float draggable" onclick="document.getElementById('painel').style.display='block'">MENU</button>

<script>
    // CORREÇÃO: Função para deixar invisível mas funcional
    function toggleVisibility() {
        const check = document.getElementById('check-invisible').checked;
        const botoes = document.querySelectorAll('.btn-float');
        
        botoes.forEach(btn => {
            if (check) {
                btn.classList.add('esta-invisivel');
            } else {
                btn.classList.remove('esta-invisivel');
            }
        });
    }

    function mudarTamanho(valor) {
        const botoes = document.querySelectorAll('.btn-float');
        botoes.forEach(btn => {
            btn.style.width = valor + 'px';
            btn.style.height = valor + 'px';
            btn.style.fontSize = (valor / 6) + 'px';
        });
    }

    function toggleStatus(tipo) {
        const btn = document.getElementById('btn-' + tipo);
        const range = document.getElementById('range-' + tipo).value;
        btn.classList.toggle('on-' + tipo);
        
        let estaAtivo = btn.classList.contains('on-' + tipo);
        let statusTexto = estaAtivo ? "ON" : "OFF";
        
        document.getElementById('lbl-' + tipo).innerText = tipo.toUpperCase() + " (" + statusTexto + ") - " + range + "MB";
    }

    // Arrastar (Draggable) para Mobile
    function makeDraggable(element) {
        let posX = 0, posY = 0, mouseX = 0, mouseY = 0;
        element.addEventListener('touchstart', (e) => {
            mouseX = e.touches[0].clientX;
            mouseY = e.touches[0].clientY;
            document.addEventListener('touchmove', dragMove, {passive: false});
        });

        function dragMove(e) {
            posX = mouseX - e.touches[0].clientX;
            posY = mouseY - e.touches[0].clientY;
            mouseX = e.touches[0].clientX;
            mouseY = e.touches[0].clientY;
            element.style.top = (element.offsetTop - posY) + "px";
            element.style.left = (element.offsetLeft - posX) + "px";
        }

        element.addEventListener('touchend', () => {
            document.removeEventListener('touchmove', dragMove);
        });
    }

    makeDraggable(document.getElementById("painel"));
    makeDraggable(document.getElementById("btn-freeze"));
    makeDraggable(document.getElementById("btn-ghost"));
    makeDraggable(document.getElementById("btn-menu"));
</script>

</body>
</html>
