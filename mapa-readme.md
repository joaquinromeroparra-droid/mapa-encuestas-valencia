# 🗺️ Mapa de Problemáticas - Valencia

Visualización interactiva de las encuestas ciudadanas por barrio de Valencia.

## 🌐 Demo

[https://joaquinromeroparra-droid.github.io/mapa-encuestas-valencia/](https://joaquinromeroparra-droid.github.io/mapa-encuestas-valencia/)

## ✨ Características

- 🗺️ **Mapa interactivo** con los 19 barrios de Valencia
- 🎨 **Colores por problemática** (verde → amarillo → naranja → rojo)
- 📊 **9 tipos de problemáticas** seleccionables
- 📈 **Ranking** de los 5 barrios con mayor problemática
- 💬 **Popups informativos** al hacer clic en cada barrio
- ☁️ **Datos en tiempo real** desde Supabase
- 📱 **Responsive** (funciona en móvil y tablet)

## 📋 Problemáticas visualizadas

1. Seguridad ciudadana
2. Limpieza y residuos
3. Transporte público
4. Zonas verdes y jardines
5. Ruido y contaminación
6. Estado de calles y aceras
7. Servicios sanitarios
8. Comercio local
9. Vivienda

## 🎨 Escala de colores

| Color | Rango | Significado |
|-------|-------|-------------|
| 🟢 Verde | 0.0 - 3.0 | Baja problemática |
| 🟡 Amarillo | 3.1 - 6.0 | Problemática media |
| 🟠 Naranja | 6.1 - 8.0 | Alta problemática |
| 🔴 Rojo | 8.1 - 10.0 | Problemática crítica |

## 🛠️ Tecnologías

- **Leaflet.js** - Mapa interactivo
- **GeoJSON** - Polígonos de barrios
- **Supabase** - Base de datos en tiempo real
- **OpenStreetMap** - Tiles del mapa

## 📂 Estructura del proyecto

```
mapa-encuestas-valencia/
├── index.html                  # Aplicación principal
├── valencia-barrios.geojson    # Geometrías de los barrios
└── README.md                   # Este archivo
```

## 🚀 Instalación local

### Opción 1: Servidor Python

```bash
python -m http.server 8000
```

Abre: http://localhost:8000

### Opción 2: Live Server (VS Code)

1. Instala la extensión "Live Server"
2. Clic derecho en `index.html` → "Open with Live Server"

## 🔗 Conexión con la encuesta

Este mapa se conecta automáticamente con la base de datos de:
- [Encuesta Ciudadana Valencia](https://joaquinromeroparra-droid.github.io/encuesta-valencia/)

Los datos se actualizan en tiempo real desde Supabase.

## 📊 Origen de datos

**Fuente:** Encuestas ciudadanas anónimas  
**Base de datos:** Supabase (PostgreSQL)  
**Actualización:** Tiempo real  
**Cobertura:** 19 barrios de Valencia

## 🎯 Uso

1. **Selecciona una problemática** en el menú desplegable
2. **El mapa se colorea** según los datos
3. **Haz clic en un barrio** para ver estadísticas detalladas
4. **Consulta el ranking** de barrios en el panel lateral

## 🔄 Actualizar datos

Haz clic en el botón **"🔄 Actualizar datos"** para recargar la información más reciente.

## 📱 Responsive

El mapa se adapta automáticamente a dispositivos móviles. En pantallas pequeñas, el panel lateral se oculta para maximizar el área del mapa.

## 🌍 GeoJSON

El archivo `valencia-barrios.geojson` contiene las geometrías de los 19 barrios de Valencia en formato GeoJSON estándar.

### Barrios incluidos:

- Ciutat Vella
- Eixample
- Extramurs
- Campanar
- La Saïdia
- El Pla del Real
- L'Olivereta
- Patraix
- Jesús
- Quatre Carreres
- Poblats Marítims
- Camins al Grau
- Algirós
- Benimaclet
- Rascanya
- Benicalap
- Pobles del Nord
- Pobles de l'Oest
- Pobles del Sud

## 📄 Licencia

MIT - Proyecto educativo para mejora ciudadana

## 👥 Autor

Proyecto de análisis de encuestas ciudadanas para Valencia

## 🔗 Enlaces relacionados

- [Repositorio de la encuesta](https://github.com/joaquinromeroparra-droid/encuesta-valencia)
- [Encuesta ciudadana](https://joaquinromeroparra-droid.github.io/encuesta-valencia/)
- [Base de datos Supabase](https://supabase.com/dashboard/project/gnaczccnprnuqbjmzdts)

---

**⭐ Si te resulta útil este proyecto, dale una estrella en GitHub!**