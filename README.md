# SALA — Siguiendo Atentamente Los Acontecimientos

**Dashboard de inteligencia para conflictos y situaciones geopolíticas globales**

🔗 [Ver en vivo → GitHub Pages](https://TU-USUARIO.github.io/sala/)

---

## ¿Qué es SALA?

SALA es un dashboard de inteligencia de fuentes abiertas (OSINT) para el seguimiento de conflictos armados, tensiones geopolíticas y situaciones de crisis a nivel mundial. Diseñado con estética de sala de operaciones militares.

## Características

- **🗺️ Mapa mundial interactivo** con 23+ conflictos y situaciones activas geolocalizadas
- **🏷️ Tags filtrables** — GUERRA / CRISIS / TENSIÓN / NAVAL / AÉREO / CYBER / NUCLEAR
- **📰 12 fuentes de noticias RSS** — Al Jazeera, BBC, CNN, Reuters, AP, ISW, Bellingcat y más
- **🔍 14 cuentas OSINT/SIGINT/HUMINT** verificadas en X/Twitter
- **🛩️ 12 trackers en tiempo real** — MarineTraffic, ADS-B Exchange, LiveUAMap, DeepStateMap, Sentinel Hub
- **📊 Índice de tensión** por región geográfica
- **📡 Ticker de últimas novedades** en tiempo real
- **🕐 Reloj UTC** en la barra superior

## Deploy en GitHub Pages

1. Fork o clonar este repositorio
2. Ir a **Settings → Pages**
3. Source: **Deploy from branch → main → / (root)**
4. El sitio estará disponible en `https://TU-USUARIO.github.io/sala/`

## Estructura

```
sala/
├── index.html      # App completa (HTML + CSS + JS en un archivo)
├── conflicts.json  # (opcional) Datos de conflictos externos
└── README.md
```

## Agregar/Actualizar Conflictos

Editar el array `conflicts` en `index.html`:

```javascript
{ 
  id: 24, 
  title: "Nombre del conflicto", 
  region: "Región geográfica", 
  lat: 0.0, 
  lng: 0.0, 
  tag: "war",        // war | crisis | tension | naval | air | cyber | nuclear
  intensity: 75,     // 0-100
  desc: "Descripción del conflicto.", 
  updated: "2025-03-01" 
}
```

## Fuentes de Datos

- **ACLED** — Armed Conflict Location & Event Data Project
- **ISW** — Institute for the Study of War
- **UNOCHA** — UN Office for the Coordination of Humanitarian Affairs
- **Global Conflict Tracker** — CFR

## Próximas Funcionalidades

- [ ] Integración RSS real via proxy CORS (AllOrigins / rss2json)
- [ ] Carga dinámica desde `conflicts.json`
- [ ] Filtro por fecha de último update
- [ ] Modo oscuro/claro
- [ ] Exportar a PDF/imagen
- [ ] Alertas por keyword en feeds

## Créditos

Desarrollado para uso académico y de inteligencia abierta. Todas las fuentes son públicas y abiertas (OSINT).

---
*Federico Andino — [fedeandino.com](https://www.fedeandino.com)*
