[EcoPuntos_EJECUTABLE_FINAL_PEDIDOS_CORREGIDO.html](https://github.com/user-attachments/files/31088814/EcoPuntos_EJECUTABLE_FINAL_PEDIDOS_CORREGIDO.html)
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>EcoPuntos - Sistema Unificado</title>
<style>


*{
    box-sizing:border-box;
    margin:0;
    padding:0;
    font-family:Arial,sans-serif;
}

body{
    background:#f1f8f4;
    color:#263238;
    min-height:100vh;
}

/* =========================
   ENCABEZADO
========================= */

header{
    background:
    linear-gradient(
        135deg,
        #1b5e20,
        #43a047
    );

    color:white;
    padding:25px 20px;
    text-align:center;
}

.logo{
    font-size:32px;
    font-weight:bold;
}

header p{
    margin-top:7px;
    opacity:.95;
}

/* =========================
   CONTENEDOR
========================= */

.container{
    width:92%;
    max-width:1000px;
    margin:25px auto;
}

.card{
    background:white;
    padding:25px;
    border-radius:18px;
    margin-bottom:20px;

    box-shadow:
    0 5px 20px rgba(0,0,0,.10);
}

/* =========================
   LOGIN
========================= */

.login{
    max-width:430px;
    margin:40px auto;
}

.login h2{
    margin-bottom:10px;
}

input,
select{
    width:100%;
    padding:14px;

    margin:8px 0;

    border:
    1px solid #cfd8dc;

    border-radius:10px;

    font-size:16px;

    outline:none;
}

input:focus,
select:focus{
    border-color:#43a047;
}

button{
    border:0;

    border-radius:10px;

    padding:13px 18px;

    cursor:pointer;

    font-size:15px;

    transition:.2s;
}

button:hover{
    transform:translateY(-1px);
}

.btn-verde{
    background:#43a047;
    color:white;
}

.btn-verde:hover{
    background:#2e7d32;
}

.btn-azul{
    background:#1976d2;
    color:white;
}

.btn-rojo{
    background:#e53935;
    color:white;
}

.btn-gris{
    background:#78909c;
    color:white;
}

.btn-naranja{
    background:#ef6c00;
    color:white;
}

.btn-completo{
    width:100%;
}

/* =========================
   OCULTO
========================= */

.oculto{
    display:none;
}

/* =========================
   PERFIL
========================= */

.perfil{

    display:flex;

    justify-content:
    space-between;

    align-items:center;

    gap:15px;

    margin-bottom:20px;
}

.usuario-info h2{
    color:#1b5e20;
}

.usuario-info p{
    color:#607d8b;
    margin-top:5px;
}

.btn-salir{
    background:#e53935;
    color:white;
}

/* =========================
   SALDO
========================= */

.saldo{

    background:
    linear-gradient(
        135deg,
        #2e7d32,
        #66bb6a
    );

    color:white;

    padding:30px;

    border-radius:20px;

    margin-bottom:20px;

    position:relative;

    overflow:hidden;
}

.saldo::after{

    content:"♻️";

    position:absolute;

    right:20px;

    bottom:-15px;

    font-size:90px;

    opacity:.15;
}

.saldo-titulo{
    font-size:15px;
}

.saldo-monto{

    font-size:42px;

    font-weight:bold;

    margin-top:8px;
}

.saldo-puntos{
    margin-top:7px;
    opacity:.9;
}

/* =========================
   GRID
========================= */

.grid{

    display:grid;

    grid-template-columns:
    repeat(2,1fr);

    gap:20px;
}

/* =========================
   TITULOS
========================= */

h2{
    color:#263238;
    margin-bottom:12px;
}

h3{
    color:#2e7d32;
    margin-bottom:10px;
}

.descripcion{
    color:#607d8b;
    line-height:1.5;
    margin-bottom:15px;
}

/* =========================
   RECICLAJE
========================= */

.residuos{

    display:grid;

    grid-template-columns:
    repeat(2,1fr);

    gap:10px;

    margin:15px 0;
}

.residuo{

    border:
    2px solid #e0e0e0;

    padding:15px;

    border-radius:12px;

    cursor:pointer;

    text-align:center;

    background:white;
}

.residuo:hover{
    border-color:#43a047;
}

.residuo.seleccionado{

    border-color:#43a047;

    background:#e8f5e9;

    color:#1b5e20;

    font-weight:bold;
}

.residuo .icono{
    font-size:30px;
    display:block;
    margin-bottom:5px;
}

.puntos-preview{

    background:#e8f5e9;

    padding:15px;

    border-radius:10px;

    margin:15px 0;

    color:#2e7d32;

    font-weight:bold;
}

/* =========================
   RETIRO
========================= */

.limite{

    background:#fff3e0;

    color:#e65100;

    padding:13px;

    border-radius:10px;

    margin:12px 0;

    font-size:14px;
}

.monto-input{
    position:relative;
}

.monto-input span{

    position:absolute;

    left:13px;

    top:22px;

    font-weight:bold;

    color:#546e7a;
}

.monto-input input{
    padding-left:38px;
}

/* =========================
   CODIGO
========================= */

.codigo-box{

    background:#263238;

    color:white;

    padding:20px;

    border-radius:15px;

    text-align:center;

    margin-top:15px;
}

.codigo{

    display:inline-block;

    background:#111;

    padding:10px 16px;

    border-radius:8px;

    margin-top:10px;

    font-size:24px;

    font-weight:bold;

    letter-spacing:3px;

    font-family:monospace;

}

/* =========================
   HISTORIAL
========================= */

.historial-item{

    display:flex;

    justify-content:space-between;

    align-items:center;

    padding:15px 0;

    border-bottom:
    1px solid #eeeeee;

}

.historial-item:last-child{
    border-bottom:0;
}

.historial-info strong{
    display:block;
}

.historial-info small{
    color:#78909c;
}

.positivo{
    color:#2e7d32;
    font-weight:bold;
}

.negativo{
    color:#e53935;
    font-weight:bold;
}

/* =========================
   ESTADOS
========================= */

.estado{

    display:inline-block;

    padding:6px 10px;

    border-radius:20px;

    font-size:12px;

    font-weight:bold;

    margin-top:5px;
}

.estado-pendiente{
    background:#fff3cd;
    color:#856404;
}

.estado-aprobado{
    background:#d4edda;
    color:#155724;
}

.estado-rechazado{
    background:#f8d7da;
    color:#721c24;
}

/* =========================
   MENSAJES
========================= */

.mensaje{

    padding:14px;

    border-radius:10px;

    margin-top:10px;

    line-height:1.4;
}

.exito{
    background:#e8f5e9;
    color:#2e7d32;
}

.error{
    background:#ffebee;
    color:#c62828;
}

.info{
    background:#e3f2fd;
    color:#1565c0;
}

/* =========================
   FIRMA
========================= */

.firma-creador{

    position:fixed;

    right:14px;

    bottom:12px;

    background:
    rgba(255,255,255,.96);

    color:#546e7a;

    padding:
    7px 11px;

    border-radius:10px;

    box-shadow:
    0 3px 12px
    rgba(0,0,0,.15);

    border-left:
    3px solid #43a047;

    z-index:9999;

    text-align:right;

    font-size:10px;
}

.firma-creador span{

    display:block;

    font-size:8px;

    color:#78909c;

}

.firma-creador strong{

    display:block;

    color:#263238;

    font-size:10px;

}

/* =========================
   FOOTER
========================= */

footer{

    background:#263238;

    color:white;

    text-align:center;

    padding:25px;

    margin-top:30px;

    padding-bottom:55px;
}

/* =========================
   RESPONSIVE
========================= */

@media(max-width:700px){

    .grid{
        grid-template-columns:1fr;
    }

    .perfil{
        display:block;
    }

    .btn-salir{
        margin-top:12px;
    }

    .residuos{
        grid-template-columns:1fr 1fr;
    }

    .saldo-monto{
        font-size:36px;
    }

}

@media(max-width:450px){

    .container{
        width:95%;
    }

    .card{
        padding:18px;
    }

    .residuos{
        grid-template-columns:1fr;
    }

    .firma-creador{
        right:8px;
        bottom:8px;
    }

}




*{
    box-sizing:border-box;
    margin:0;
    padding:0;
    font-family:Arial,sans-serif;
}

body{
    background:#eef3f5;
    color:#263238;
}

header{
    background:
    linear-gradient(
        135deg,
        #263238,
        #455a64
    );

    color:white;
    padding:25px;
    text-align:center;
}

.logo{
    font-size:34px;
    font-weight:bold;
}

header p{
    margin-top:7px;
}

.container{
    width:92%;
    max-width:1150px;
    margin:25px auto;
}

.card{
    background:white;
    padding:25px;
    border-radius:18px;
    margin-bottom:20px;
    box-shadow:0 5px 18px #0002;
}

h2{
    color:#263238;
    margin-bottom:15px;
}

.oculto{
    display:none;
}


/* LOGIN */

.login{
    max-width:430px;
    margin:50px auto;
}

input{
    width:100%;
    padding:14px;
    margin:8px 0;
    border:1px solid #ccc;
    border-radius:10px;
    font-size:16px;
}

button{
    border:0;
    border-radius:10px;
    padding:13px 18px;
    cursor:pointer;
    font-size:15px;
}

.btn-entrar{
    width:100%;
    background:#455a64;
    color:white;
    margin-top:10px;
}

.btn-salir{
    background:#e53935;
    color:white;
}

.btn-buscar{
    background:#455a64;
    color:white;
}

.btn-aprobar{
    background:#43a047;
    color:white;
}

.btn-rechazar{
    background:#e53935;
    color:white;
}

.btn-gris{
    background:#78909c;
    color:white;
}


/* ADMIN */

.admin-header{
    display:flex;
    justify-content:space-between;
    align-items:center;
    margin-bottom:20px;
}


/* ESTADISTICAS */

.estadisticas{

    display:grid;

    grid-template-columns:
    repeat(5,1fr);

    gap:15px;

}

.stat{

    color:white;

    padding:20px;

    border-radius:16px;

}

.stat h3{

    font-size:30px;

    margin-top:8px;

}

.stat-pendiente{
    background:#f9a825;
}

.stat-aprobado{
    background:#43a047;
}

.stat-rechazado{
    background:#e53935;
}

.stat-puntos{
    background:#1976d2;
}

.stat-retiros{
    background:#ef6c00;
}


/* BUSCAR */

.buscador{

    display:flex;

    gap:10px;

}

.buscador input{

    margin:0;

    flex:1;

}


/* SOLICITUD */

.solicitud{

    border:
    2px solid #e0e0e0;

    border-radius:16px;

    padding:20px;

    margin-bottom:15px;

}

.solicitud-header{

    display:flex;

    justify-content:space-between;

    align-items:center;

    margin-bottom:15px;

}

.codigo{

    background:#263238;

    color:white;

    padding:8px 12px;

    border-radius:8px;

    font-family:monospace;

    font-weight:bold;

    letter-spacing:1px;

}

.estado{

    padding:7px 12px;

    border-radius:20px;

    font-weight:bold;

    font-size:14px;

}

.pendiente{

    background:#fff3cd;

    color:#856404;

}

.aprobado{

    background:#d4edda;

    color:#155724;

}

.rechazado{

    background:#f8d7da;

    color:#721c24;

}


/* INFO */

.info-grid{

    display:grid;

    grid-template-columns:
    repeat(2,1fr);

    gap:10px;

    margin-bottom:15px;

}

.info{

    background:#f5f7f8;

    padding:13px;

    border-radius:10px;

}

.info strong{

    display:block;

    color:#546e7a;

    margin-bottom:5px;

}


/* ACCIONES */

.acciones{

    display:flex;

    gap:10px;

    margin-top:18px;

}


/* FILTROS */

.filtros{

    display:flex;

    gap:10px;

    margin:15px 0;

    flex-wrap:wrap;

}

.filtros button{

    background:#eceff1;

}

.filtros button.activo{

    background:#455a64;

    color:white;

}


/* MONTO */

.monto{

    font-size:28px;

    font-weight:bold;

    color:#e65100;

}


/* MENSAJES */

.mensaje{

    padding:15px;

    border-radius:10px;

    margin-top:10px;

}

.error{

    background:#ffebee;

    color:#c62828;

}

.exito{

    background:#e8f5e9;

    color:#2e7d32;

}


/* VACIO */

.vacio{

    text-align:center;

    padding:35px;

    color:#78909c;

}


/* FOOTER */

footer{

    background:#263238;

    color:white;

    text-align:center;

    padding:25px;

    margin-top:30px;

}


/* RESPONSIVE */

@media(max-width:900px){

    .estadisticas{

        grid-template-columns:
        repeat(2,1fr);

    }

}

@media(max-width:600px){

    .admin-header{

        display:block;

    }

    .admin-header button{

        margin-top:12px;

    }

    .estadisticas{

        grid-template-columns:1fr;

    }

    .buscador{

        display:block;

    }

    .buscador button{

        width:100%;

        margin-top:8px;

    }

    .info-grid{

        grid-template-columns:1fr;

    }

    .acciones{

        display:block;

    }

    .acciones button{

        width:100%;

        margin-top:7px;

    }

}



/* ESTILOS DE LA APLICACION UNIFICADA */
header{background:linear-gradient(135deg,#1b5e20,#43a047)!important;}
.acceso-tabs{display:flex;gap:10px;}
#tabUsuario,#tabAdmin{flex:1;background:#eceff1;}
#tabUsuario.activo,#tabAdmin.activo{background:#455a64;color:white;}
#panelAdmin{max-width:1150px;}

</style>
</head>
<body>
<header>
<div class="logo">♻️ EcoPuntos</div>
<p>Recicla, gana puntos y conviértelos en soles</p>
</header>
<div id="pantallaAcceso" class="container">
<div class="card login">
  <h2>♻️ Bienvenido a EcoPuntos</h2>
  <p class="descripcion">Selecciona tu tipo de acceso para continuar.</p>
  <div class="filtros" style="margin-top:15px;">
    <button id="tabUsuario" class="activo" onclick="mostrarAccesoTipo('usuario')">👤 Usuario</button>
    <button id="tabAdmin" onclick="mostrarAccesoTipo('admin')">🛠️ Administrador</button>
  </div>

  <div id="accesoUsuario">
    <h3>Crear cuenta</h3>
    <input id="nombreRegistro" type="text" placeholder="Nombre completo">
    <input id="correoRegistro" type="email" placeholder="Correo electrónico">
    <input id="claveRegistro" type="password" placeholder="Contraseña">
    <button class="btn-verde btn-completo" onclick="registrar()">Crear cuenta</button>
    <br><br><hr><br>
    <h3>Ya tengo una cuenta</h3>
    <input id="correoLogin" type="email" placeholder="Correo electrónico">
    <input id="claveLogin" type="password" placeholder="Contraseña">
    <button class="btn-azul btn-completo" onclick="iniciarSesion()">Iniciar sesión</button>
  </div>

  <div id="accesoAdmin" class="oculto">
    <h3>Acceso de administrador</h3>
    <p class="descripcion">Ingresa las credenciales del panel administrativo.</p>
    <input id="adminUsuario" type="text" placeholder="Usuario">
    <input id="adminClave" type="password" placeholder="Contraseña">
    <button class="btn-gris btn-completo" onclick="iniciarAdmin()">Ingresar al panel</button>
  </div>

  <div id="mensajeAcceso" class="mensaje oculto"></div>
</div>
</div>
<div class="container oculto" id="panelUsuario">
<!-- PERFIL -->
<div class="perfil">
<div class="usuario-info">
<h2>
                Hola, <span id="nombreUsuario">
                Usuario
                </span> 👋
            </h2>
<p>
                ¡Gracias por ayudar al planeta!
            </p>
</div>
<button class="btn-salir" onclick="cerrarSesion()">

            Cerrar sesión

        </button>
</div>
<!-- SALDO -->
<div class="saldo">
<div class="saldo-titulo">
            💰 Mi saldo
        </div>
<div class="saldo-monto" id="saldoUsuario">

            S/ 0.00

        </div>
<div class="saldo-puntos" id="puntosUsuario">

            0 puntos

        </div>
</div>
<div class="grid">
<!-- =====================
             RECICLAR
        ====================== -->
<div class="card">
<h2>
                ♻️ Reciclar
            </h2>
<p class="descripcion">

                Selecciona el material
                que deseas reciclar.

                El administrador verificará
                tu entrega.

            </p>
<div class="residuos">
<div class="residuo" onclick="seleccionarResiduo(this,'Plástico',10)" title="10 puntos = S/ 0.10">
<span class="icono">
                        🧴
                    </span>

                    Plástico
                    <small style="display:block;margin-top:6px;color:#607d8b;font-weight:normal;">10 puntos · S/ 0.10</small>

                </div>
<div class="residuo" onclick="seleccionarResiduo(this,'Cartón',5)" title="5 puntos = S/ 0.05">
<span class="icono">
                        📦
                    </span>

                    Cartón
                    <small style="display:block;margin-top:6px;color:#607d8b;font-weight:normal;">5 puntos · S/ 0.05</small>

                </div>
<div class="residuo" onclick="seleccionarResiduo(this,'Papel',5)" title="5 puntos = S/ 0.05">
<span class="icono">
                        📄
                    </span>

                    Papel
                    <small style="display:block;margin-top:6px;color:#607d8b;font-weight:normal;">5 puntos · S/ 0.05</small>

                </div>
<div class="residuo" onclick="seleccionarResiduo(this,'Vidrio',8)" title="8 puntos = S/ 0.08">
<span class="icono">
                        🍾
                    </span>

                    Vidrio
                    <small style="display:block;margin-top:6px;color:#607d8b;font-weight:normal;">8 puntos · S/ 0.08</small>

                </div>
</div>
<div class="puntos-preview" id="puntosPreview">

                Selecciona un material

            </div>
<button class="btn-verde btn-completo" onclick="solicitarReciclaje()">

                ♻️ Solicitar reciclaje

            </button>
<div class="mensaje oculto" id="mensajeReciclaje">
</div>
</div>
<!-- =====================
             RETIRO
        ====================== -->
<div class="card">
<h2>
                💵 Retirar dinero
            </h2>
<p class="descripcion">

                Convierte tus puntos
                en dinero.

            </p>
<div class="limite">

                ℹ️ Retiro mínimo:
                <strong>S/ 1.00</strong>
<br/>

                Retiro máximo:
                <strong>S/ 50.00</strong>
<br/>
<strong>
                    100 puntos = S/ 1.00
                </strong>
</div>
<div class="monto-input">
<span>
                    S/
                </span>
<input id="montoRetiro" max="50" min="1" placeholder="Monto a retirar" step="0.01" type="number"/>
</div>
<button class="btn-naranja btn-completo" onclick="solicitarRetiro()">

                💰 Solicitar retiro

            </button>
<div class="mensaje oculto" id="mensajeRetiro">
</div>
<div class="codigo-box oculto" id="codigoRetiroBox">

                🔐 Código para el administrador

                <div class="codigo" id="codigoRetiro">
</div>
<p style="margin-top:10px">

                    Presenta este código
                    al administrador.

                </p>
</div>
</div>
</div>
<!-- =========================
         ESTADO DE SOLICITUDES
    ========================== -->
<div class="card">
<h2>
            📋 Mis solicitudes
        </h2>
<div id="listaSolicitudes">
</div>
</div>
<!-- =========================
         HISTORIAL
    ========================== -->
<div class="card">
<h2>
            📜 Historial
        </h2>
<div id="historial">
</div>
</div>
</div>
<div class="container oculto" id="panelAdmin">
<div class="admin-header">
<div>
<h2>

                🛠️ Panel del administrador

            </h2>
<p>

                Control de reciclajes y retiros

            </p>
</div>
<button class="btn-salir" onclick="adminCerrarAdmin()">

            Cerrar sesión

        </button>
</div>
<!-- ESTADISTICAS -->
<div class="estadisticas">
<div class="stat stat-pendiente">

            ⏳ Solicitudes pendientes

            <h3 id="totalPendientes">

                0

            </h3>
</div>
<div class="stat stat-aprobado">

            ✅ Reciclajes aprobados

            <h3 id="totalAprobadas">

                0

            </h3>
</div>
<div class="stat stat-rechazado">

            ❌ Rechazados

            <h3 id="totalRechazadas">

                0

            </h3>
</div>
<div class="stat stat-puntos">

            ⭐ Puntos entregados

            <h3 id="totalPuntos">

                0

            </h3>
</div>
<div class="stat stat-retiros">

            💰 Retiros pendientes

            <h3 id="totalRetirosPendientes">

                0

            </h3>
</div>
</div>
<br/>
<!-- ========================
         RETIROS
    ========================= -->
<div class="card">
<h2>

            💰 Solicitudes de retiro

        </h2>
<p>

            Revisa el código y entrega el dinero
            al usuario antes de aprobar el retiro.

        </p>
<div class="filtros">
<button class="activo" id="filtroRetirosTodos" onclick="adminCambiarFiltroRetiro('todas')">

                Todos

            </button>
<button id="filtroRetirosPendientes" onclick="adminCambiarFiltroRetiro('pendiente')">

                ⏳ Pendientes

            </button>
<button id="filtroRetirosAprobados" onclick="adminCambiarFiltroRetiro('aprobado')">

                ✅ Aprobados

            </button>
<button id="filtroRetirosRechazados" onclick="adminCambiarFiltroRetiro('rechazado')">

                ❌ Rechazados

            </button>
</div>
<div id="listaRetiros">
</div>
</div>
<!-- BUSCAR RETIRO -->
<div class="card">
<h2>

            🔎 Buscar código de retiro

        </h2>
<div class="buscador">
<input id="buscarRetiro" placeholder="Ejemplo: RET-4821"/>
<button class="btn-buscar" onclick="adminBuscarRetiro()">

                Buscar

            </button>
</div>
<div id="resultadoRetiro">
</div>
</div>
<!-- ========================
         RECICLAJES
    ========================= -->
<div class="card">
<h2>

            ♻️ Solicitudes de reciclaje

        </h2>
<div class="filtros">
<button class="activo" id="filtroTodas" onclick="adminCambiarFiltroReciclaje('todas')">

                Todas

            </button>
<button id="filtroPendientes" onclick="adminCambiarFiltroReciclaje('pendiente')">

                ⏳ Pendientes

            </button>
<button id="filtroAprobadas" onclick="adminCambiarFiltroReciclaje('aprobado')">

                ✅ Aprobadas

            </button>
<button id="filtroRechazadas" onclick="adminCambiarFiltroReciclaje('rechazado')">

                ❌ Rechazadas

            </button>
</div>
<div id="listaSolicitudesAdmin">
</div>
</div>
</div>
<footer>

    ♻️ EcoPuntos Perú

    <br/><br/>

    Reciclando juntos por un futuro mejor.

</footer>
<div class="firma-creador">
<span>
        Creado por
    </span>
<strong>
        Ing. de Sistemas Yacks Oviedo
    </strong>
</div>
<script>


/* =====================================
   VARIABLES
===================================== */

let usuarios =

JSON.parse(

    localStorage.getItem(
        "ecoUsuarios"
    )

) || {};


let solicitudes =

JSON.parse(

    localStorage.getItem(
        "ecoSolicitudes"
    )

) || {};


if(
    !Array.isArray(solicitudes)
){
    solicitudes = [];
}


let retiros =

JSON.parse(

    localStorage.getItem(
        "ecoRetiros"
    )

) || {};


if(
    !Array.isArray(retiros)
){
    retiros = [];
}


let usuarioActual = null;


let residuoSeleccionado = null;

let puntosSeleccionados = 0;


/* =====================================
   REGISTRAR
===================================== */

function registrar(){

    const nombre =

    document
    .getElementById(
        "nombreRegistro"
    )
    .value
    .trim();


    const correo =

    document
    .getElementById(
        "correoRegistro"
    )
    .value
    .trim()
    .toLowerCase();


    const clave =

    document
    .getElementById(
        "claveRegistro"
    )
    .value;


    if(
        !nombre ||
        !correo ||
        !clave
    ){

        mostrarAcceso(
            "Completa todos los campos.",
            "error"
        );

        return;
    }


    if(
        usuarios[correo]
    ){

        mostrarAcceso(
            "Este correo ya tiene una cuenta.",
            "error"
        );

        return;
    }


    usuarios[correo] = {

        nombre:nombre,

        correo:correo,

        clave:clave,

        puntos:0,

        historial:[]

    };


    guardarUsuarios();


    mostrarAcceso(
        "✅ Cuenta creada correctamente. Ahora puedes iniciar sesión.",
        "exito"
    );


    document
    .getElementById(
        "nombreRegistro"
    )
    .value = "";


    document
    .getElementById(
        "correoRegistro"
    )
    .value = "";


    document
    .getElementById(
        "claveRegistro"
    )
    .value = "";

}


/* =====================================
   LOGIN
===================================== */

function iniciarSesion(){

    const correo =

    document
    .getElementById(
        "correoLogin"
    )
    .value
    .trim()
    .toLowerCase();


    const clave =

    document
    .getElementById(
        "claveLogin"
    )
    .value;


    if(
        !usuarios[correo]
    ){

        mostrarAcceso(
            "❌ No existe una cuenta con ese correo.",
            "error"
        );

        return;
    }


    if(
        usuarios[correo].clave !==
        clave
    ){

        mostrarAcceso(
            "❌ Contraseña incorrecta.",
            "error"
        );

        return;
    }


    usuarioActual = correo;


    document
    .getElementById(
        "pantallaAcceso"
    )
    .classList
    .add("oculto");


    document
    .getElementById(
        "panelUsuario"
    )
    .classList
    .remove("oculto");


    cargarUsuario();

}


/* =====================================
   CARGAR USUARIO
===================================== */

function cargarUsuario(){

    if(
        !usuarioActual
    ){
        return;
    }


    recargarDatos();


    const usuario =

    usuarios[
        usuarioActual
    ];


    document
    .getElementById(
        "nombreUsuario"
    )
    .textContent =
    usuario.nombre;


    actualizarSaldo();


    mostrarSolicitudes();


    mostrarHistorial();

}


/* =====================================
   SALDO
===================================== */

function actualizarSaldo(){

    const usuario =

    usuarios[
        usuarioActual
    ];


    const puntos =

    Number(
        usuario.puntos
    ) || 0;


    const soles =

    puntos / 100;


    document
    .getElementById(
        "saldoUsuario"
    )
    .textContent =

    "S/ " +
    soles.toFixed(2);


    document
    .getElementById(
        "puntosUsuario"
    )
    .textContent =

    puntos +
    " puntos";

}


/* =====================================
   SELECCIONAR RESIDUO
===================================== */

function seleccionarResiduo(

    elemento,
    nombre,
    puntos

){

    document
    .querySelectorAll(
        ".residuo"
    )
    .forEach(
        r =>
        r.classList
        .remove(
            "seleccionado"
        )
    );


    elemento
    .classList
    .add(
        "seleccionado"
    );


    residuoSeleccionado =
    nombre;


    puntosSeleccionados =
    puntos;


    document
    .getElementById(
        "puntosPreview"
    )
    .innerHTML =

    "⭐ Recibirás " +
    "<strong>" +
    puntos +
    " puntos</strong> " +
    "si el administrador acepta y completa tu entrega.";

}


/* =====================================
   SOLICITAR RECICLAJE
===================================== */

function solicitarReciclaje(){

    if(
        !usuarioActual
    ){
        return;
    }


    if(
        !residuoSeleccionado
    ){

        mostrarMensaje(
            "mensajeReciclaje",
            "Selecciona primero un material.",
            "error"
        );

        return;
    }


    const pedidoPendiente = solicitudes.find(
        s => s.usuario === usuarioActual &&
             s.residuo === residuoSeleccionado &&
             s.estado === "pendiente"
    );

    if(pedidoPendiente){
        mostrarMensaje(
            "mensajeReciclaje",
            "⚠️ Ya tienes un pedido de " + residuoSeleccionado + " pendiente. Espera a que el administrador lo acepte o rechace.",
            "info"
        );
        return;
    }

    const codigo =

    generarCodigo(
        "REC"
    );


    const solicitud = {

        id:
        Date.now(),

        usuario:
        usuarioActual,

        nombreUsuario:
        usuarios[
            usuarioActual
        ].nombre,

        residuo:
        residuoSeleccionado,

        puntos:
        puntosSeleccionados,

        codigo:
        codigo,

        estado:
        "pendiente",

        fecha:
        new Date()
        .toLocaleString(),

        fechaAprobacion: null,
        fechaRechazo: null,
        mensaje: "Pedido recibido. Pendiente de verificación del administrador."

    };


    solicitudes.push(
        solicitud
    );


    guardarSolicitudes();


    mostrarMensaje(
        "mensajeReciclaje",
        "✅ Pedido registrado correctamente. Entrega el material y muestra tu código al administrador. Quedará PENDIENTE hasta que él lo acepte.",
        "exito"
    );


    document
    .getElementById(
        "puntosPreview"
    )
    .innerHTML =

    "🔑 Tu código es: " +
    "<strong>" +
    codigo +
    "</strong>";


    mostrarSolicitudes();

}


/* =====================================
   SOLICITAR RETIRO
===================================== */

function solicitarRetiro(){

    if(
        !usuarioActual
    ){
        return;
    }


    const monto =

    Number(

        document
        .getElementById(
            "montoRetiro"
        )
        .value

    );


    if(
        !monto ||
        monto < 1 ||
        monto > 50
    ){

        mostrarMensaje(
            "mensajeRetiro",
            "El retiro debe ser entre S/ 1.00 y S/ 50.00.",
            "error"
        );

        return;
    }


    const usuario =

    usuarios[
        usuarioActual
    ];


    const saldo =

    Number(
        usuario.puntos
    ) / 100;


    if(
        monto > saldo
    ){

        mostrarMensaje(
            "mensajeRetiro",
            "❌ No tienes saldo suficiente. Tu saldo es S/ " +
            saldo.toFixed(2),
            "error"
        );

        return;
    }


    /*
       Evitar varios retiros
       pendientes al mismo tiempo.
    */

    const retiroPendiente =

    retiros.find(

        r =>

        r.usuario ===
        usuarioActual &&

        r.estado ===
        "pendiente"

    );


    if(
        retiroPendiente
    ){

        mostrarMensaje(
            "mensajeRetiro",
            "⚠️ Ya tienes un retiro pendiente. Espera a que el administrador lo procese.",
            "error"
        );

        return;
    }


    const codigo =

    generarCodigo(
        "RET"
    );


    const retiro = {

        id:
        Date.now(),

        usuario:
        usuarioActual,

        nombreUsuario:
        usuario.nombre,

        monto:
        monto,

        codigo:
        codigo,

        estado:
        "pendiente",

        fecha:
        new Date()
        .toLocaleString()

    };


    retiros.push(
        retiro
    );


    guardarRetiros();


    document
    .getElementById(
        "montoRetiro"
    )
    .value = "";


    document
    .getElementById(
        "codigoRetiro"
    )
    .textContent =
    codigo;


    document
    .getElementById(
        "codigoRetiroBox"
    )
    .classList
    .remove(
        "oculto"
    );


    mostrarMensaje(
        "mensajeRetiro",
        "✅ Solicitud enviada. El administrador debe aprobarla.",
        "exito"
    );


    mostrarSolicitudes();

}


/* =====================================
   MOSTRAR SOLICITUDES
===================================== */

function mostrarSolicitudes(){

    const contenedor =

    document
    .getElementById(
        "listaSolicitudes"
    );


    contenedor.innerHTML = "";


    const misReciclajes =

    solicitudes
    .filter(

        s =>

        s.usuario ===
        usuarioActual

    )
    .reverse();


    const misRetiros =

    retiros
    .filter(

        r =>

        r.usuario ===
        usuarioActual

    )
    .reverse();


    if(
        misReciclajes.length === 0 &&
        misRetiros.length === 0
    ){

        contenedor.innerHTML = `

            <p style="color:#78909c">

                📭 Todavía no tienes solicitudes.

            </p>

        `;

        return;
    }


    misReciclajes.forEach(

        solicitud => {

            const estado =

            crearEstado(
                solicitud.estado
            );


            contenedor.innerHTML += `

                <div class="historial-item">

                    <div class="historial-info">

                        <strong>

                            ♻️ ${solicitud.residuo}

                        </strong>

                        <small>

                            Código:
                            ${solicitud.codigo}

                            <br>

                            ${solicitud.fecha}

                        </small>

                        <br>

                        ${estado}

                        <div class="mensaje ${solicitud.estado === "aprobado" ? "exito" : solicitud.estado === "rechazado" ? "error" : "info"}" style="margin-top:8px;font-size:13px;">
                            ${solicitud.mensaje || mensajeProcesoSolicitud("reciclaje", solicitud.estado)}
                            ${solicitud.fechaAprobacion ? "<br><small>Procesado: " + solicitud.fechaAprobacion + "</small>" : ""}
                        </div>

                    </div>


                    <div class="positivo">

                        +${solicitud.puntos}

                        puntos

                    </div>

                </div>

            `;

        }
    );


    misRetiros.forEach(

        retiro => {

            const estado =

            crearEstado(
                retiro.estado
            );


            contenedor.innerHTML += `

                <div class="historial-item">

                    <div class="historial-info">

                        <strong>

                            💰 Retiro de dinero

                        </strong>

                        <small>

                            Código:
                            ${retiro.codigo}

                            <br>

                            ${retiro.fecha}

                        </small>

                        <br>

                        ${estado}

                        <div class="mensaje ${retiro.estado === "aprobado" ? "exito" : retiro.estado === "rechazado" ? "error" : "info"}" style="margin-top:8px;font-size:13px;">
                            ${retiro.mensaje || mensajeProcesoSolicitud("retiro", retiro.estado)}
                            ${retiro.fechaAprobacion ? "<br><small>Procesado: " + retiro.fechaAprobacion + "</small>" : ""}
                        </div>

                    </div>


                    <div class="negativo">

                        S/
                        ${Number(
                            retiro.monto
                        ).toFixed(2)}

                    </div>

                </div>

            `;

        }
    );

}


/* =====================================
   HISTORIAL
===================================== */

function mostrarHistorial(){

    const contenedor =

    document
    .getElementById(
        "historial"
    );


    const usuario =

    usuarios[
        usuarioActual
    ];


    const historial =

    usuario.historial || [];


    if(
        historial.length === 0
    ){

        contenedor.innerHTML = `

            <p style="color:#78909c">

                📭 Tu historial está vacío.

            </p>

        `;

        return;
    }


    contenedor.innerHTML = "";


    historial
    .slice()
    .reverse()
    .forEach(

        item => {

            const clase =

            Number(
                item.puntos
            ) >= 0

            ?

            "positivo"

            :

            "negativo";


            const signo =

            Number(
                item.puntos
            ) >= 0

            ?

            "+"

            :

            "";


            contenedor.innerHTML += `

                <div class="historial-item">

                    <div class="historial-info">

                        <strong>

                            ${item.texto}

                        </strong>

                        <small>

                            ${item.fecha}

                        </small>

                    </div>


                    <div class="${clase}">

                        ${signo}${item.puntos}

                        puntos

                    </div>

                </div>

            `;

        }

    );

}


/* =====================================
   ESTADO
===================================== */

function crearEstado(

    estado

){

    if(
        estado ===
        "aprobado"
    ){

        return `

            <span class="estado estado-aprobado">

                ✅ Aprobado

            </span>

        `;

    }


    if(
        estado ===
        "rechazado"
    ){

        return `

            <span class="estado estado-rechazado">

                ❌ Rechazado

            </span>

        `;

    }


    return `

        <span class="estado estado-pendiente">

            ⏳ Pendiente

        </span>

    `;

}


/* =====================================
   MENSAJE DE PROCESO
===================================== */
function mensajeProcesoSolicitud(tipo, estado){
    if(tipo === "reciclaje"){
        if(estado === "pendiente") return "⏳ Pedido recibido. Esperando que el administrador verifique y acepte tu entrega.";
        if(estado === "aprobado") return "✅ Pedido realizado. El administrador aceptó la entrega y tus puntos ya fueron acreditados.";
        if(estado === "rechazado") return "❌ Pedido rechazado. No se acreditaron puntos.";
    }
    if(tipo === "retiro"){
        if(estado === "pendiente") return "⏳ Retiro solicitado. Esperando que el administrador verifique el código y entregue el dinero.";
        if(estado === "aprobado") return "✅ Retiro realizado. El administrador aprobó la solicitud y registró la entrega del dinero.";
        if(estado === "rechazado") return "❌ Retiro rechazado. No se descontaron puntos.";
    }
    return "";
}


/* =====================================
   GENERAR CODIGO
===================================== */

function generarCodigo(

    prefijo

){

    return (

        prefijo +

        "-" +

        Math.floor(

            1000 +

            Math.random() *
            9000

        )

    );

}


/* =====================================
   MENSAJES
===================================== */

function mostrarMensaje(

    id,
    texto,
    tipo

){

    const caja =

    document
    .getElementById(
        id
    );


    caja.textContent =
    texto;


    caja.className =

    "mensaje " +
    tipo;


    caja.style.display =
    "block";

}


/* =====================================
   MENSAJE ACCESO
===================================== */

function mostrarAcceso(

    texto,
    tipo

){

    mostrarMensaje(

        "mensajeAcceso",

        texto,

        tipo

    );

}


/* =====================================
   GUARDAR DATOS
===================================== */

function guardarUsuarios(){

    localStorage.setItem(

        "ecoUsuarios",

        JSON.stringify(
            usuarios
        )

    );

}


function guardarSolicitudes(){

    localStorage.setItem(

        "ecoSolicitudes",

        JSON.stringify(
            solicitudes
        )

    );

}


function guardarRetiros(){

    localStorage.setItem(

        "ecoRetiros",

        JSON.stringify(
            retiros
        )

    );

}


/* =====================================
   RECARGAR DATOS
===================================== */

function recargarDatos(){

    usuarios =

    JSON.parse(

        localStorage.getItem(
            "ecoUsuarios"
        )

    ) || {};


    solicitudes =

    JSON.parse(

        localStorage.getItem(
            "ecoSolicitudes"
        )

    ) || [];


    retiros =

    JSON.parse(

        localStorage.getItem(
            "ecoRetiros"
        )

    ) || [];

}


/* =====================================
   CERRAR SESION
===================================== */

function cerrarSesion(){
    document.getElementById("panelAdmin").classList.add("oculto");

    usuarioActual = null;


    document
    .getElementById(
        "panelUsuario"
    )
    .classList
    .add(
        "oculto"
    );


    document
    .getElementById(
        "pantallaAcceso"
    )
    .classList
    .remove(
        "oculto"
    );

}


/* =====================================
   ACTUALIZAR AUTOMATICAMENTE
===================================== */

setInterval(

    function(){

        if(
            usuarioActual
        ){

            recargarDatos();

            cargarUsuario();

        }

    },

    3000

);





/* =====================================
   PANEL
===================================== */


function adminCargarPanel(){

    recargarDatos();

    adminActualizarEstadisticas();

    adminMostrarRetiros();

    adminMostrarSolicitudes();

}



/* =====================================
   ESTADISTICAS
===================================== */


function adminActualizarEstadisticas(){


    const pendientes =

        solicitudes.filter(

            s =>

            s.estado ===

            "pendiente"

        ).length;


    const aprobadas =

        solicitudes.filter(

            s =>

            s.estado ===

            "aprobado"

        ).length;


    const rechazadas =

        solicitudes.filter(

            s =>

            s.estado ===

            "rechazado"

        ).length;


    const puntos =

        solicitudes

        .filter(

            s =>

            s.estado ===

            "aprobado"

        )

        .reduce(

            (total,s) =>

            total + Number(s.puntos),

            0

        );


    const retirosPendientes =

        retiros.filter(

            r =>

            r.estado ===

            "pendiente"

        ).length;


    document

    .getElementById(

        "totalPendientes"

    )

    .textContent =

        pendientes;


    document

    .getElementById(

        "totalAprobadas"

    )

    .textContent =

        aprobadas;


    document

    .getElementById(

        "totalRechazadas"

    )

    .textContent =

        rechazadas;


    document

    .getElementById(

        "totalPuntos"

    )

    .textContent =

        puntos;


    document

    .getElementById(

        "totalRetirosPendientes"

    )

    .textContent =

        retirosPendientes;

}



/* =====================================
   MOSTRAR RETIROS
===================================== */


function adminMostrarRetiros(){


    recargarDatos();


    const contenedor =

        document

        .getElementById(

            "listaRetiros"

        );


    contenedor.innerHTML = "";


    let lista =

        retiros

        .slice()

        .reverse();



    if(

        filtroRetiro !==

        "todas"

    ){

        lista =

            lista.filter(

                r =>

                r.estado ===

                filtroRetiro

            );

    }



    if(

        lista.length === 0

    ){

        contenedor.innerHTML = `

            <div class="vacio">

                💰

                <br><br>

                No hay solicitudes
                de retiro.

            </div>

        `;

        return;

    }



    lista.forEach(

        retiro => {


        let textoEstado =

            "⏳ Pendiente";


        let claseEstado =

            "pendiente";



        if(

            retiro.estado ===

            "aprobado"

        ){

            textoEstado =

                "✅ Aprobado";

            claseEstado =

                "aprobado";

        }



        if(

            retiro.estado ===

            "rechazado"

        ){

            textoEstado =

                "❌ Rechazado";

            claseEstado =

                "rechazado";

        }



        let acciones = "";



        if(

            retiro.estado ===

            "pendiente"

        ){

            acciones = `

                <div class="acciones">


                    <button

                        class="btn-aprobar"

                        onclick=

                        "adminAprobarRetiro('${retiro.id}')">

                        ✅ Aceptar y completar entrega

                    </button>


                    <button

                        class="btn-rechazar"

                        onclick=

                        "adminRechazarRetiro('${retiro.id}')">

                        ❌ Rechazar

                    </button>


                </div>

            `;

        }



        const div =

            document

            .createElement(

                "div"

            );


        div.className =

            "solicitud";


        div.innerHTML = `


            <div class="solicitud-header">


                <strong>

                    💰 Solicitud de retiro

                </strong>


                <span

                    class="estado ${claseEstado}">

                    ${textoEstado}

                </span>


            </div>



            <div class="info-grid">


                <div class="info">

                    <strong>

                        👤 Usuario

                    </strong>

                    ${retiro.nombreUsuario}

                </div>


                <div class="info">

                    <strong>

                        📧 Correo

                    </strong>

                    ${retiro.usuario}

                </div>


                <div class="info">

                    <strong>

                        💰 Monto

                    </strong>

                    <span class="monto">

                        S/

                        ${Number(

                            retiro.monto

                        ).toFixed(2)}

                    </span>

                </div>


                <div class="info">

                    <strong>

                        📅 Fecha

                    </strong>

                    ${retiro.fecha}

                </div>


            </div>



            <p>

                🔑 Código de retiro:

            </p>


            <br>


            <span class="codigo">

                ${retiro.codigo}

            </span>

            <div class="mensaje ${retiro.estado === "aprobado" ? "exito" : retiro.estado === "rechazado" ? "error" : "info"}" style="margin-top:15px;">
                ${retiro.mensaje || mensajeProcesoSolicitud("retiro", retiro.estado)}
            </div>


            ${acciones}

        `;


        contenedor.appendChild(

            div

        );

    });

}



/* =====================================
   APROBAR RETIRO
===================================== */


function adminAprobarRetiro(id){


    recargarDatos();


    const retiro =

        retiros.find(

            r =>

            String(r.id) ===

            String(id)

        );


    if(!retiro){

        alert(

            "❌ No se encontró el retiro."

        );

        return;

    }



    if(

        retiro.estado !==

        "pendiente"

    ){

        alert(

            "Este retiro ya fue procesado."

        );

        return;

    }



    /*
       BUSCAR USUARIO
    */


    const usuario =

        usuarios[

            retiro.usuario

        ];


    if(!usuario){

        alert(

            "❌ No se encontró la cuenta del usuario."

        );

        return;

    }



    /*
       CALCULAR SALDO
    */


    const saldoActual =

        Number(

            usuario.puntos

        ) / 100;


    const monto =

        Number(

            retiro.monto

        );



    /*
       VERIFICAR SALDO
    */


    if(

        monto < 1 ||

        monto > 50

    ){

        alert(

            "❌ El monto del retiro no es válido."

        );

        return;

    }



    if(

        monto > saldoActual

    ){

        alert(

            "❌ El usuario ya no tiene saldo suficiente.\n\n" +

            "Saldo actual: S/ " +

            saldoActual.toFixed(2) +

            "\n" +

            "Retiro: S/ " +

            monto.toFixed(2)

        );

        return;

    }



    /*
       CONFIRMACION
    */


    const confirmar =

        confirm(

            "¿Confirmas que verificaste el código " +

            retiro.codigo +

            " y entregaste S/ " +

            monto.toFixed(2) +

            " al usuario?"

        );


    if(!confirmar){

        return;

    }



    /*
       DESCONTAR PUNTOS
       
       S/ 1 = 100 puntos
    */


    const puntosARestar =

        Math.round(

            monto * 100

        );


    usuario.puntos =

        Number(

            usuario.puntos

        ) -

        puntosARestar;



    /*
       REGISTRAR HISTORIAL
    */


    if(

        !usuario.historial

    ){

        usuario.historial = [];

    }



    usuario.historial.push({

        texto:

            "Retiro " +

            retiro.codigo,


        puntos:

            -puntosARestar,


        fecha:

            new Date()

            .toLocaleString()

    });



    /*
       ACTUALIZAR RETIRO
    */


    retiro.estado =

        "aprobado";


    retiro.fechaAprobacion =

        new Date()

        .toLocaleString();

    retiro.mensaje = "Retiro realizado: código verificado y dinero entregado al usuario.";



    /*
       GUARDAR USUARIO
    */


    usuarios[

        retiro.usuario

    ] = usuario;



    localStorage.setItem(

        "ecoUsuarios",

        JSON.stringify(

            usuarios

        )

    );



    /*
       GUARDAR RETIROS
    */


    localStorage.setItem(

        "ecoRetiros",

        JSON.stringify(

            retiros

        )

    );



    /*
       ACTUALIZAR PANTALLA
    */


    adminCargarPanel();



    alert(

        "✅ Retiro aprobado correctamente.\n\n" +

        "Código: " +

        retiro.codigo +

        "\n" +

        "Monto entregado: S/ " +

        monto.toFixed(2) +

        "\n\n" +

        "Se descontaron " +

        puntosARestar +

        " puntos."

    );

}



/* =====================================
   RECHAZAR RETIRO
===================================== */


function adminRechazarRetiro(id){


    recargarDatos();


    const retiro =

        retiros.find(

            r =>

            String(r.id) ===

            String(id)

        );


    if(!retiro){

        alert(

            "❌ Retiro no encontrado."

        );

        return;

    }



    if(

        retiro.estado !==

        "pendiente"

    ){

        alert(

            "Este retiro ya fue procesado."

        );

        return;

    }



    const confirmar =

        confirm(

            "¿Quieres rechazar el retiro " +

            retiro.codigo +

            "?"

        );


    if(!confirmar){

        return;

    }



    retiro.estado =

        "rechazado";

    retiro.mensaje = "Retiro rechazado por el administrador. No se descontaron puntos.";


    retiro.fechaRechazo =

        new Date()

        .toLocaleString();



    localStorage.setItem(

        "ecoRetiros",

        JSON.stringify(

            retiros

        )

    );



    adminCargarPanel();



    alert(

        "❌ Retiro rechazado.\n\n" +

        "El saldo del usuario no fue descontado."

    );

}



/* =====================================
   BUSCAR RETIRO
===================================== */


function adminBuscarRetiro(){


    recargarDatos();


    const codigo =

        document

        .getElementById(

            "buscarRetiro"

        )

        .value

        .trim()

        .toUpperCase();


    const resultado =

        document

        .getElementById(

            "resultadoRetiro"

        );


    if(!codigo){

        resultado.innerHTML = `

            <div class="mensaje error">

                Escribe un código de retiro.

            </div>

        `;

        return;

    }



    const retiro =

        retiros.find(

            r =>

            r.codigo.toUpperCase() ===

            codigo

        );


    if(!retiro){

        resultado.innerHTML = `

            <div class="mensaje error">

                ❌ No se encontró el código

                <strong>

                    ${codigo}

                </strong>.

            </div>

        `;

        return;

    }



    let estado =

        "⏳ Pendiente";


    if(

        retiro.estado ===

        "aprobado"

    ){

        estado =

            "✅ Aprobado";

    }


    if(

        retiro.estado ===

        "rechazado"

    ){

        estado =

            "❌ Rechazado";

    }



    let botones = "";


    if(

        retiro.estado ===

        "pendiente"

    ){

        botones = `

            <div class="acciones">


                <button

                    class="btn-aprobar"

                    onclick=

                    "adminAprobarRetiro('${retiro.id}')">

                    ✅ Aprobar

                </button>


                <button

                    class="btn-rechazar"

                    onclick=

                    "adminRechazarRetiro('${retiro.id}')">

                    ❌ Rechazar

                </button>


            </div>

        `;

    }



    resultado.innerHTML = `

        <br>


        <div class="solicitud">


            <div class="solicitud-header">


                <strong>

                    💰 Retiro encontrado

                </strong>


                <span>

                    ${estado}

                </span>


            </div>



            <div class="info-grid">


                <div class="info">

                    <strong>

                        👤 Usuario

                    </strong>

                    ${retiro.nombreUsuario}

                </div>


                <div class="info">

                    <strong>

                        💰 Monto

                    </strong>

                    S/

                    ${Number(

                        retiro.monto

                    ).toFixed(2)}

                </div>


            </div>



            <p>

                🔑 Código:

            </p>


            <br>


            <span class="codigo">

                ${retiro.codigo}

            </span>


            ${botones}

        </div>

    `;

}



/* =====================================
   FILTRO RETIROS
===================================== */


function adminCambiarFiltroRetiro(

    filtro

){


    filtroRetiro =

        filtro;


    document

    .querySelectorAll(

        ".filtros button"

    )

    .forEach(

        b =>

        b.classList

        .remove("activo")

    );


    if(

        filtro ===

        "todas"

    ){

        document

        .getElementById(

            "filtroRetirosTodos"

        )

        .classList

        .add("activo");

    }


    if(

        filtro ===

        "pendiente"

    ){

        document

        .getElementById(

            "filtroRetirosPendientes"

        )

        .classList

        .add("activo");

    }


    if(

        filtro ===

        "aprobado"

    ){

        document

        .getElementById(

            "filtroRetirosAprobados"

        )

        .classList

        .add("activo");

    }


    if(

        filtro ===

        "rechazado"

    ){

        document

        .getElementById(

            "filtroRetirosRechazados"

        )

        .classList

        .add("activo");

    }


    adminMostrarRetiros();

}



/* =====================================
   RECICLAJES
===================================== */


function adminMostrarSolicitudes(){


    recargarDatos();


    if(!document.getElementById("listaSolicitudesAdmin")){
        return;
    }


    const contenedor =

        document

        .getElementById(

            "listaSolicitudesAdmin"

        );


    contenedor.innerHTML = "";


    let lista =

        solicitudes

        .slice()

        .reverse();



    if(

        filtroReciclaje !==

        "todas"

    ){

        lista =

            lista.filter(

                s =>

                s.estado ===

                filtroReciclaje

            );

    }



    if(

        lista.length === 0

    ){

        contenedor.innerHTML = `

            <div class="vacio">

                📭

                <br><br>

                No hay solicitudes.

            </div>

        `;

        return;

    }



    lista.forEach(

        solicitud => {


        let texto =

            "⏳ Pendiente";


        let clase =

            "pendiente";


        if(

            solicitud.estado ===

            "aprobado"

        ){

            texto =

                "✅ Aprobado";

            clase =

                "aprobado";

        }


        if(

            solicitud.estado ===

            "rechazado"

        ){

            texto =

                "❌ Rechazado";

            clase =

                "rechazado";

        }



        let acciones = "";


        if(

            solicitud.estado ===

            "pendiente"

        ){

            acciones = `

                <div class="acciones">


                    <button

                        class="btn-aprobar"

                        onclick=

                        "adminAprobarReciclaje('${solicitud.id}')">

                        ✅ Aceptar y completar

                    </button>


                    <button

                        class="btn-rechazar"

                        onclick=

                        "adminRechazarReciclaje('${solicitud.id}')">

                        ❌ Rechazar

                    </button>


                </div>

            `;

        }



        const div =

            document

            .createElement(

                "div"

            );


        div.className =

            "solicitud";


        div.innerHTML = `

            <div class="solicitud-header">

                <strong>

                    ♻️

                    ${solicitud.residuo}

                </strong>

                <span

                    class="estado ${clase}">

                    ${texto}

                </span>

            </div>


            <div class="info-grid">


                <div class="info">

                    <strong>

                        👤 Usuario

                    </strong>

                    ${solicitud.nombreUsuario}

                </div>


                <div class="info">

                    <strong>

                        📧 Correo

                    </strong>

                    ${solicitud.usuario}

                </div>


                <div class="info">

                    <strong>

                        ⭐ Puntos

                    </strong>

                    +${solicitud.puntos}

                </div>


                <div class="info">

                    <strong>

                        📅 Fecha

                    </strong>

                    ${solicitud.fecha}

                </div>


            </div>


            <p>

                🔑 Código:

            </p>


            <br>


            <span class="codigo">

                ${solicitud.codigo}

            </span>

            <div class="mensaje ${solicitud.estado === "aprobado" ? "exito" : solicitud.estado === "rechazado" ? "error" : "info"}" style="margin-top:15px;">
                ${solicitud.mensaje || mensajeProcesoSolicitud("reciclaje", solicitud.estado)}
            </div>


            ${acciones}

        `;


        contenedor.appendChild(

            div

        );

    });

}



/* =====================================
   APROBAR RECICLAJE
===================================== */


function adminAprobarReciclaje(id){


    recargarDatos();


    const solicitud =

        solicitudes.find(

            s =>

            String(s.id) ===

            String(id)

        );


    if(!solicitud){

        alert(

            "Solicitud no encontrada."

        );

        return;

    }


    if(

        solicitud.estado !==

        "pendiente"

    ){

        return;

    }



    const usuario =

        usuarios[

            solicitud.usuario

        ];


    if(!usuario){

        alert(

            "Usuario no encontrado."

        );

        return;

    }



    const confirmar =

        confirm(

            "¿Confirmas que verificaste el reciclaje " +

            solicitud.codigo +

            "?"

        );


    if(!confirmar){

        return;

    }



    solicitud.estado =

        "aprobado";

    solicitud.fechaAprobacion = new Date().toLocaleString();
    solicitud.mensaje = "Pedido realizado: entrega verificada y puntos acreditados.";


    usuario.puntos =

        Number(

            usuario.puntos

        ) +

        Number(

            solicitud.puntos

        );



    if(

        !usuario.historial

    ){

        usuario.historial = [];

    }



    usuario.historial.push({

        texto:

            solicitud.residuo,

        puntos:

            solicitud.puntos,

        fecha:

            new Date()

            .toLocaleString()

    });



    usuarios[

        solicitud.usuario

    ] = usuario;



    localStorage.setItem(

        "ecoUsuarios",

        JSON.stringify(

            usuarios

        )

    );


    localStorage.setItem(

        "ecoSolicitudes",

        JSON.stringify(

            solicitudes

        )

    );


    adminCargarPanel();


    alert(

        "✅ Reciclaje aprobado.\n\n" +

        "Se agregaron +" +

        solicitud.puntos +

        " puntos."

    );

}



/* =====================================
   RECHAZAR RECICLAJE
===================================== */


function adminRechazarReciclaje(id){


    recargarDatos();


    const solicitud =

        solicitudes.find(

            s =>

            String(s.id) ===

            String(id)

        );


    if(!solicitud){

        return;

    }


    if(

        solicitud.estado !==

        "pendiente"

    ){

        return;

    }



    const confirmar =

        confirm(

            "¿Deseas rechazar este reciclaje?"

        );


    if(!confirmar){

        return;

    }



    solicitud.estado =

        "rechazado";

    solicitud.fechaRechazo = new Date().toLocaleString();
    solicitud.mensaje = "Pedido rechazado por el administrador. No se acreditaron puntos.";


    localStorage.setItem(

        "ecoSolicitudes",

        JSON.stringify(

            solicitudes

        )

    );


    adminCargarPanel();


    alert(

        "❌ Reciclaje rechazado."

    );

}



/* =====================================
   FILTRO RECICLAJE
===================================== */


function adminCambiarFiltroReciclaje(

    filtro

){


    filtroReciclaje =

        filtro;


    document

    .querySelectorAll(

        ".card:nth-of-type(4) .filtros button"

    );



    adminMostrarSolicitudes();

}



/* =====================================
   CERRAR
===================================== */


function adminCerrarAdmin(){


    document

    .getElementById(

        "panelAdmin"

    )

    .classList

    .add("oculto");


    document

    .getElementById(

        "pantallaLogin"

    )

    .classList

    .remove("oculto");


    document

    .getElementById(

        "adminUsuario"

    )

    .value = "";


    document

    .getElementById(

        "adminClave"

    )

    .value = "";

}




/* =====================================
   ACCESO UNIFICADO
===================================== */
const ADMIN_USUARIO = "administrador";
const ADMIN_CLAVE = "eco123";

function mostrarAccesoTipo(tipo){
    document.getElementById("accesoUsuario").classList.toggle("oculto", tipo !== "usuario");
    document.getElementById("accesoAdmin").classList.toggle("oculto", tipo !== "admin");
    document.getElementById("tabUsuario").classList.toggle("activo", tipo === "usuario");
    document.getElementById("tabAdmin").classList.toggle("activo", tipo === "admin");
    document.getElementById("mensajeAcceso").className = "mensaje oculto";
}

function iniciarAdmin(){
    const usuario = document.getElementById("adminUsuario").value.trim();
    const clave = document.getElementById("adminClave").value;
    const caja = document.getElementById("mensajeAcceso");
    if(usuario === ADMIN_USUARIO && clave === ADMIN_CLAVE){
        document.getElementById("pantallaAcceso").classList.add("oculto");
        document.getElementById("panelUsuario").classList.add("oculto");
        document.getElementById("panelAdmin").classList.remove("oculto");
        adminCargarPanel();
    } else {
        caja.textContent = "❌ Usuario o contraseña incorrectos.";
        caja.className = "mensaje error";
    }
}

</script>
</body>
</html>
