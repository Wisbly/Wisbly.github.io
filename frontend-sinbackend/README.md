# CineTeatro — Demo Interactiva (sin backend)

Prototipo visual de la plataforma **CineTeatro SaaS** para presentar a clientes. No requiere base de datos, servidor ni instalación.

## Cómo abrir

Doble clic en **`index.html`** — se abre en el navegador y ya está.

O sirve la carpeta con cualquier servidor estático (opcional):
```
npx serve frontend-sinbackend
```

## Páginas incluidas

### Cliente / público
| Archivo | Descripción |
|---|---|
| `index.html` | Página principal — cartelera + funciones de hoy + eventos |
| `pelicula.html` | Detalle de película con funciones disponibles y reseñas |
| `reserva.html` | Mapa de asientos **interactivo** — haz clic para seleccionar |
| `checkout.html` | Confirmación con cupón, descuentos, canje de puntos |
| `exito.html` | Ticket generado con QR code |

### Panel de administrador
| Archivo | Descripción |
|---|---|
| `admin.html` | Dashboard con métricas, ventas de la semana y top películas |
| `admin-peliculas.html` | Gestión de películas — grid con póster, edición |
| `admin-funciones.html` | Programación de funciones — tabla con ocupación |
| `admin-salas.html` | Editor visual de asientos con tipos y precios editables |
| `admin-cupones.html` | Cupones de descuento con métricas de uso |
| `admin-reportes.html` | Reportes con gráficos, top películas, distribución |
| `admin-taquilla.html` | Venta presencial en boletería |
| `admin-usuarios.html` | Usuarios del sistema (clientes + personal) |

## Flujo recomendado para presentar al cliente

1. Abre `index.html` — muestra la vista pública del cine
2. Clic en cualquier película → `pelicula.html`
3. Clic en "Elegir asientos" → `reserva.html` (**demuestra la interactividad**, selecciona varios asientos)
4. Clic en "Continuar" → `checkout.html`
5. Clic en "Confirmar pago" → `exito.html` (ticket con QR)
6. Vuelve al inicio y clic en **"Panel de administrador"** (arriba a la derecha)
7. Recorre el sidebar: Películas → Funciones → Salas → Cupones → Reportes → Taquilla → Usuarios

## Notas

- Todos los datos son **ficticios** pero realistas (nombres chilenos, precios en CLP, películas actuales)
- Las imágenes se cargan desde TMDb (necesita internet)
- Es una demo **puramente visual** — los formularios no guardan datos
- El único elemento realmente interactivo es la selección de asientos (`reserva.html`)
