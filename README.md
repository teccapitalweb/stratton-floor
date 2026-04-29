# Stratton Floor · TEC CAPITAL GROUP

Dashboard de ventas en vivo + panel admin para las 15 consultoras de IPCI.

## 🚀 URLs

- **Arena (proyectar en TV):** `https://teccapitalweb.github.io/stratton-floor/`
- **Panel admin (operadora):** `https://teccapitalweb.github.io/stratton-floor/panel.html`

## 📁 Estructura

```
stratton-floor/
├── index.html      ← Dashboard principal (el Floor con barras)
├── panel.html      ← Panel admin con +1 por consultora
└── img/            ← 15 logos de consultoras
    ├── sinergia.png
    ├── bionova.png
    └── ... (13 más)
```

## ⚡ Cómo funciona

Las dos páginas comparten **localStorage** (`stratton.state.v10`).
Cuando la operadora hace `+1` en `panel.html`, el Floor en `index.html` actualiza al instante via `storage` event.

## 🎨 Stack

- HTML/CSS/JS vanilla — sin frameworks ni build
- Web Audio API para sonidos sintetizados
- Canvas para confetti
- localStorage para persistencia

## 🔧 Workflow diario

1. **10:00 AM CDMX** — el bono del día se revela automáticamente con animación
2. **Durante el día** — operadora hace `+1` en panel cuando entra venta
3. **5:00 PM** — se activa modo estadio (drone bass + frase rota cada 5min)
4. **6:00 PM** — cierre de turno con podio 3D de los 3 ganadores
5. **Medianoche** — reset automático y archivado al historial
