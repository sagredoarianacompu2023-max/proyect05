<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nuestro Espacio ❤️</title>
    <style>
        body { background-image: url('https://i.postimg.cc/9fshvVKK/descargar-(3).jpg'); background-size: cover; background-position: center; background-attachment: fixed; font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; padding: 20px; display: flex; justify-content: center; }
        h1 { color: #3366ff; background-color: #ccffff; display: inline-block; padding: 10px; border-radius: 15px; font-size: 1.6rem; }
        .tabs { margin: 20px 0; display: flex; flex-wrap: wrap; justify-content: center; }
        .btn-tab { background: #0288d1; color: white; border: none; padding: 10px 15px; margin: 5px; border-radius: 20px; cursor: pointer; font-weight: bold; font-size: 0.85rem; transition: 0.3s; }
        .btn-tab:hover { background: #01579b; transform: scale(1.1); }
        .ventana { display: none; background: white; padding: 25px; border-radius: 25px; box-shadow: 0 10px 30px rgba(0,0,0,0.1); margin-top: 15px; animation: fadeIn 0.4s ease-in-out; }
        .visible { display: block !important; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }
        .frasco-wrapper { background: #ffffff99; border: 4px solid #0288d1; border-radius: 20px 20px 80px 80px; width: 260px; min-height: 220px; margin: 20px auto; padding: 20px; display: flex; flex-wrap: wrap; justify-content: center; align-content: center; }
        .emoji-click { font-size: 1.8rem; cursor: pointer; margin: 6px; transition: transform 0.2s; user-select: none; }
        .emoji-click:hover { transform: scale(1.4) rotate(15deg); }
        .mensaje-display { font-weight: bold; color: #d81b60; margin-top: 20px; min-height: 60px; padding: 15px; border-top: 1px dashed #0288d1; display: flex; align-items: center; justify-content: center; }
        .polaroid { background: white; padding: 15px; box-shadow: 0 5px 15px rgba(0,0,0,0.15); margin-bottom: 25px; transition: 0.3s; }
        .polaroid img { width: 100%; height: auto; border: 1px solid #eee; }
        .polaroid p { font-family: 'Courier New', monospace; font-weight: bold; margin-top: 15px; color: #555; font-size: 0.9rem; }
        ol { text-align: left; background: #f1f8ff; padding: 25px 40px; border-radius: 20px; }

/* Estilos para el Álbum Interactivo */
        .controles-album { margin-top: 15px; display: flex; flex-wrap: wrap; justify-content: center; gap: 8px; }
        .btn-foto { background: #f1f8ff; color: #0288d1; border: 2px solid #0288d1; padding: 8px 12px; border-radius: 50%; cursor: pointer; font-weight: bold; transition: 0.2s; }
        .btn-foto:hover, .btn-foto.activo { background: #0288d1; color: white; transform: scale(1.1); }
        #visor-album { max-width: 350px; margin: 20px auto; opacity: 1; transition: opacity 0.3s ease-in-out; }
    </style>
</head>
<body>

<div class="interfaz-regalo">
    <h1>Nuestro Espacio ❤️</h1>
    <div class="tabs">
        <button class="btn-tab" onclick="abrir('inicio')">Inicio</button>
        <button class="btn-tab" onclick="abrir('recordatorio')">Lo que vales</button>
        <button class="btn-tab" onclick="abrir('frasco-amor')">Frasco de Amor</button>
        <button class="btn-tab" onclick="abrir('por-nosotros')">Por nosotros</button>
        <button class="btn-tab" onclick="abrir('galeria')">Galería</button>
        <button class="btn-tab" onclick="abrir('album')">Nuestro Álbum 📸</button>
    </div>
<div id="inicio" class="ventana visible">
        <h4><u><em>¡Hola, mi palito bombón!</em></u></h4>
        <p style="color: #000080;">He creado este lugar digital para que siempre tengas un rinconcito donde refugiarte cuando me extrañes. 😊</p>
        <p style="color: #000080;">Explora las pestañas de arriba para descubrir las sorpresas.</p>
        <p style="color: #000080;">También por si quieres leer todas las chucherías que hago por vos y algunos recuerdos que tengo cada tanto.</p>
        <p style="color: #000080;">La verdad es que amo mucho y me cuesta no pensarte y me gusta darte detalles, aunque pequeños para mi requiere tiempo, paciencia y aprendizajes. 💋</p>
    </div>
<div id="recordatorio" class="ventana">
        <h3>Pequeño recordatorio de lo que vales</h3>
        <ol type="I">
            <li>Extraño como me besas de noche</li>
            <li>Me gustan tus abrazos</li>
            <li>Todo tus intentos para verme bien</li>
            <li>Lo dulce y cargoso que Sos</li>
            <li>Y como te interesan mis pasatiempos</li>
        </ol>
    </div>
<div id="frasco-amor" class="ventana">
        <h3>Frasco de Mensajes</h3>
        <p>Toca un corazón para sacar un pensamiento:</p>
        <div class="frasco-wrapper">
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💖</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💝</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💗</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💓</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💘</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💕</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💖</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💝</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💗</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💓</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💘</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💕</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💖</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💝</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💗</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💓</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-amor', frasesAmor)">💘</span>
        </div>
        <div id="msg-amor" class="mensaje-display">¿Qué dirá hoy?</div>
    </div>
<div id="por-nosotros" class="ventana">
        <h3>Por nosotros ✨</h3>
        <p>Toca un emoji para ver un deseo:</p>
        <div class="frasco-wrapper">
            <span class="emoji-click" onclick="mostrarMensaje('msg-nos', frasesNosotros)">🌟</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-nos', frasesNosotros)">🍭</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-nos', frasesNosotros)">🎬</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-nos', frasesNosotros)">🍯</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-nos', frasesNosotros)">🎨</span>
            <span class="emoji-click" onclick="mostrarMensaje('msg-nos', frasesNosotros)">🎤</span>
        </div>
        <div id="msg-nos" class="mensaje-display">¿Qué saldrá?</div>
    </div>

<div id="galeria" class="ventana">

<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Te Amo ❤️</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background-color: #000;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            touch-action: none;
        }
        canvas {
            display: block;
        }
        #instrucciones {
            position: absolute;
            bottom: 30px;
            color: rgba(255, 105, 180, 0.6);
            font-family: 'Segoe UI', Tahoma, sans-serif;
            font-size: 14px;
            pointer-events: none;
            text-align: center;
            width: 100%;
        }
    </style>
</head>
<body>
    <script>
        const canvas = document.getElementById('heartCanvas');
        const ctx = canvas.getContext('2d');
        const texto = "te amo";
        const color = "#FF69B4"; // Rosa fuerte
        const cantidad = 360; // Densidad de palabras  
        let width, height;
        let mouseX = 0, mouseY = 0, pMouseX = 0, pMouseY = 0;
        let rotX = 0, rotY = 0;
        let isMoving = false;
        function resize() {
            width = canvas.width = window.innerWidth;
            height = canvas.height = window.innerHeight;
            ctx.font = "bold 15px Arial";
            ctx.textAlign = 'center';
            ctx.textBaseline = 'middle';
        }
        window.addEventListener('resize', resize);
        resize();
        // Generar los puntos del corazón 3D
        const puntos = [];
        for (let i = 0; i < cantidad; i++) {
            const t = Math.PI * 2 * (i / cantidad);
            const phi = Math.acos(2 * Math.random() - 1);
             // Fórmula matemática del corazón
            const x2d = 16 * Math.pow(Math.sin(t), 3);
            const y2d = 13 * Math.cos(t) - 5 * Math.cos(2*t) - 2 * Math.cos(3*t) - Math.cos(4*t);// Distribución 3D
            const x = x2d * Math.sin(phi);
            const y = y2d * Math.sin(phi);
            const z = x2d * Math.cos(phi) * 1.5;
  puntos.push({ x, y, z });
        }
function draw() {
            ctx.fillStyle = 'black';
            ctx.fillRect(0, 0, width, height);
if (!isMoving) {
                rotY += 0.05; // Giro automático suave
            } else {
                rotY += (mouseX - pMouseX) * 0.05;
                rotX += (mouseY - pMouseY) * 0.05;
            }
    pMouseX = mouseX;
            pMouseY = mouseY;
// Ordenar puntos por profundidad (Z) para que se vea bien el 3D
            const renderList = puntos.map(p => {
                let x1 = p.x * Math.cos(rotY) + p.z * Math.sin(rotY);
                let z1 = -p.x * Math.sin(rotY) + p.z * Math.cos(rotY);
                let y1 = p.y * Math.cos(rotX) - z1 * Math.sin(rotX);
                let z2 = p.y * Math.sin(rotX) + z1 * Math.cos(rotX);
const perspective = 500;
                const scale = perspective / (perspective + z2 + 30);
                const screenX = x1 * scale * 12 + width / 2;
                const screenY = -y1 * scale * 12 + height / 2;
                return { x: screenX, y: screenY, z: z2 };
            });
renderList.sort((a, b) => b.z - a.z);
renderList.forEach(p => {
                const alpha = Math.max(0.1, 1 - (p.z + 15) / 40);
                ctx.fillStyle = color;
                ctx.globalAlpha = alpha;
                ctx.fillText(texto, p.x, p.y);
            });
requestAnimationFrame(draw);
        }
   // Interacción
        const updatePos = (e) => {
            const pos = e.touches ? e.touches[0] : e;
            mouseX = pos.clientX;
            mouseY = pos.clientY;
        };
window.addEventListener('mousedown', e => { isMoving = true; updatePos(e); pMouseX = mouseX; pMouseY = mouseY; });
        window.addEventListener('mousemove', updatePos);
        window.addEventListener('mouseup', () => isMoving = false);
        window.addEventListener('touchstart', e => { isMoving = true; updatePos(e); pMouseX = mouseX; pMouseY = mouseY; }, {passive: false});
        window.addEventListener('touchmove', e => { updatePos(e); e.preventDefault(); }, {passive: false});
        window.addEventListener('touchend', () => isMoving = false);

</body>
</html>    
    </div>
 <div id="album" class="ventana">
        <h3>Nuestro Álbum Interactivo 📸</h3>
        <p>Toca los números para ver nuestras fotos:</p>
        
<div id="visor-album" class="polaroid">
            <img id="foto-actual" src="https://i.postimg.cc/7ZnRD4cG/IMG-20251010-WA0052.jpg" alt="Nuestra foto">
            <p id="texto-actual"> me encanta pensar que pronto sere tu esposa ✨</p>
        </div>

<div class="controles-album">
            <button class="btn-foto activo" onclick="cambiarFoto(0, this)">1</button>
            <button class="btn-foto" onclick="cambiarFoto(1, this)">2</button>
            <button class="btn-foto" onclick="cambiarFoto(2, this)">3</button>
            <button class="btn-foto" onclick="cambiarFoto(3, this)">4</button>
            <button class="btn-foto" onclick="cambiarFoto(4, this)">5</button>
            <button class="btn-foto" onclick="cambiarFoto(5, this)">6</button>
            <button class="btn-foto" onclick="cambiarFoto(6, this)">7</button>
        </div>
    </div>

</div>

<script>
    function abrir(id) {
        document.querySelectorAll('.ventana').forEach(v => v.classList.remove('visible'));
        document.getElementById(id).classList.add('visible');
    }

    const frasesAmor = [
        "Vale por un beso interminable. 💋", "Gracias por hacerme tan feliz cada día. ✨",
        "Eres mi persona favorita en el mundo entero. 🌎", "Amo cada pequeño detalle de ti. ❤️",
        "¡Eres el mejor regalo que me dio la vida! 🎁", "Sos la personita más dulce que conozco. 🍭",
        "Amo cuando me miras y sonreís. 😊", "Vale por una tarde de mimos sin fin. 🐾",
        "Sos mi refugio favorito. 🏠", "Gracias por tenerme tanta paciencia. 💕",
        "Me encanta cómo me hacés sentir. 💖", "Sos mucho más de lo que alguna vez soñé. ✨",
        "Amo compartir mis días con vos. ☀️", "Vale por tu comida favorita hecha por mí. 🍕",
        "Tu felicidad es la mía también. 🥰", "Sos increíble, nunca lo olvides. 💎",
        "Te amo hoy, mañana y siempre. 🌹"
    ];

    const frasesNosotros = [
        "vale por un secreto", "vale por unos masajes", "me gustan tus ojitos",
        "amo tus destalles", "gracias por hacerme sentir amada cada dia", "hacemos postrecito",
        "me gusta rascarme con tu bigote", "dibujar juntos", "cantar solos",
        "ver una peli", "te extraño todos los dias", "me haces muuuuuuuy feliz"
    ];

    function mostrarMensaje(id, lista) {
        const display = document.getElementById(id);
        display.style.opacity = 0;
        setTimeout(() => {
            display.innerText = lista[Math.floor(Math.random() * lista.length)];
            display.style.opacity = 1;
        }, 150);
    }

    // --- LÓGICA DEL ÁLBUM INTERACTIVO CON TUS 7 FOTOS ---

    const fotosAlbum = [
        {
            url: "https://i.postimg.cc/7ZnRD4cG/IMG-20251010-WA0052.jpg", 
            texto: "¡me encanta pensar que pronto sere tu esposa! ✨"
        },
        {
            url: "https://i.postimg.cc/k40sKYzJ/IMG_20251022_WA0036.jpg", 
            texto: "me gusta esta foto con nuestra hija 🤗"
        },
        {
            url: "https://i.postimg.cc/DwwrJK0G/IMG_20260110_WA0017.jpg", 
            texto: "tus abrazos lo son todoo... 7w7 💋"
        },
        {
            url: "https://i.postimg.cc/Y2GmwT1s/Captura-de-pantalla-2026-03-18-141804.png",
            texto: "Te extraño todos los días, mi vida. 💖"
        },
        {
            url: "https://i.postimg.cc/Vkkqrcvb/IMG_20251212_WA0107.jpg",
            texto: "Gracias por cada paseo.💎"
        },
        {
            url: "https://i.postimg.cc/cLLRgNCv/IMG_20251002_WA0074.jpg",
            texto: "los dias son mas lindos con vos.☀️"
        },
        {
            url: "https://i.postimg.cc/Ghh8zxRw/IMG-20260312-WA0167(1).jpg",
            texto: "jaja como me miras es tan dulce.🥞🍰"
        }
    ];

    function cambiarFoto(indice, boton) {
        const visor = document.getElementById('visor-album');
        const imgActual = document.getElementById('foto-actual');
        const txtActual = document.getElementById('texto-actual');

        visor.style.opacity = 0;

        setTimeout(() => {
            imgActual.src = fotosAlbum[indice].url;
            txtActual.innerText = fotosAlbum[indice].texto;
            visor.style.opacity = 1;

            document.querySelectorAll('.btn-foto').forEach(b => b.classList.remove('activo'));
            boton.classList.add('activo');
        }, 300);
    }

</script>
</body>
</html>
