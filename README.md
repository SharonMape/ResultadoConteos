```html
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Avances de Conteos</title>

<style>
body{
    font-family: 'Segoe UI', sans-serif;
    background:#f7f8fa;
    margin:0;
    padding:20px 40px;
}
.section-title{
    font-size:22px;
    font-weight:700;
    margin:30px 0 10px;
}
.counter{color:#777;margin-left:6px;font-weight:500;}
.grid{
    display:grid;
    grid-template-columns:repeat(auto-fill,minmax(350px,1fr));
    gap:20px;
    margin-bottom:40px;
}
.card{
    background:white;
    padding:20px;
    border-radius:14px;
    box-shadow:0 2px 5px rgba(0,0,0,0.05);
    border-top:5px solid;
    margin-left: 20px;
    margin-right: 20px;
}
.card.green{border-color:#3bb54a;}
.card.red{border-color:#e95353;}
.card-title{
    font-size:18px;
    font-weight:600;
    margin-bottom:5px;
}
.percent{
    font-size:20px;
    font-weight:700;
    margin-left:auto;
}
.row{
    display:flex;
    align-items:center;
    justify-content:space-between;
}
.status{
    padding:3px 10px;
    border-radius:10px;
    font-size:12px;
    font-weight:600;
}
.status.green{background:#e7f7ec;color:#3bb54a;}
.status.red{background:#fdeaea;color:#e95353;}
.weeks{
    margin-top:18px;
    display:flex;
    justify-content:space-between;
}
.week-item{
    text-align:center;
    font-size:12px;
}
.circle{
    width:22px;height:22px;
    border-radius:50%;
    margin:auto;
    margin-top:4px;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:12px;
}
.circle.green{background:#3bb54a;color:white;}
.circle.red{background:#e95353;color:white;}
.circle.empty{border:2px solid #d9d9d9;}

/* ⭐ TARJETA DEL HEADER – LÍNEA MÁS DELGADA */
.header-card {
    background: white;
    padding: 12px 0px;
    margin: 0 20px 10px;
    border-radius: 18px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.03);
    border: 0.6px solid #eceff3;
}

.header-container {
    padding: 18px 25px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    animation: fadeSlide 0.8s ease-out forwards;
}

.content-body {
    margin-top: 20px;
    padding: 0 10px;
}

.header-section {
    padding: 2px 0;
}

.header-card {
    padding: 1px 0px;
}

@keyframes fadeSlide {
    from { opacity: 0; transform: translateY(12px); }
    to { opacity: 1; transform: translateY(0); }
}
</style>

</head>
<body>

<!-- ⭐ HEADER DENTRO DE TARJETA -->
<div class="header-card">
    <div class="header-container">
        <div class="header-left">
            <div class="chip">
                <div class="chip-dot"></div>
                IE - Internacional de Electricos
            </div>
            <h1>Avances de Conteos</h1>
            <div class="subtitle">
                Seguimiento semanal del cumplimiento de conteos por sucursal
            </div>
        </div>

        <div class="header-right">
            <div class="info-card">
                <div class="info-label">FECHA</div>
                <div class="info-value">09/02/2026</div>
            </div>

            <div class="info-card">
                <div class="info-label">SEMANA</div>
                <div class="info-value">01</div>
            </div>
        </div>
    </div>
</div>

<!-- ⭐ CONTENIDO PRINCIPAL -->
<div class="content-body">

<h2 class="section-title" style="color:#3bb54a;"> Sucursales que Cumplieron <span class="counter">(7)</span></h2>

<div class="grid">
    <!-- Aquí van todas tus tarjetas verdes -->
    <div class="card green">
        <div class="row">
            <div class="card-title">1. Ibagué</div>
            <div class="percent">25%</div>
        </div>
        <div class="status green">Al día</div>
        <div class="weeks">
            <div class="week-item">SEM 1 <div class="circle green">✓</div></div>
            <div class="week-item">SEM 2 <div class="circle empty"></div></div>
            <div class="week-item">SEM 3 <div class="circle empty"></div></div>
            <div class="week-item">SEM 4 <div class="circle empty"></div></div>
        </div>
    </div>

    <!-- Resto de tarjetas verde y roja igual -->
</div>

<h2 class="section-title" style="color:#c93030;"> Sucursales que No Cumplieron <span class="counter">(7)</span></h2>

<div class="grid">
    <!-- Aquí van todas tus tarjetas rojas -->
    <div class="card red">
        <div class="row">
            <div class="card-title">9. Bogotá</div>
            <div class="percent">0%</div>
        </div>
        <div class="status red">Pendiente</div>
        <div class="weeks">
            <div class="week-item">SEM 1 <div class="circle red">✕</div></div>
            <div class="week-item">SEM 2 <div class="circle empty"></div></div>
            <div class="week-item">SEM 3 <div class="circle empty"></div></div>
            <div class="week-item">SEM 4 <div class="circle empty"></div></div>
        </div>
    </div>

    <!-- Resto de tarjetas rojas igual -->
</div>

</div> <!-- FIN CONTENT BODY -->

</body>
</html>
```

