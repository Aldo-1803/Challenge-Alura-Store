# 🏬 Challenge: Análisis de Sucursales de Zoop

Este proyecto es parte de un **challenge del curso de Data Science**, donde se simula ayudar al Sr. Juan a decidir **qué sucursal vender** entre 4 opciones.  
El análisis combina métricas financieras, operativas y de satisfacción del cliente para dar una recomendación sustentada con datos y visualizaciones.

---

## 📊 Objetivos del análisis
1. Calcular los **ingresos totales** por tienda.  
2. Analizar las **ventas por categoría de producto**.  
3. Medir la **calificación promedio de clientes** por tienda.  
4. Identificar **productos más y menos vendidos**.  
5. Evaluar el **costo de envío promedio** por tienda.  
6. Integrar todo en una recomendación final para el Sr. Juan.

---

## 📂 Datos utilizados
Cada tienda tiene un archivo CSV con las siguientes columnas principales:

- `Categoría del Producto` → tipo de producto vendido.  
- `Precio` → importe de la compra.  
- `Costo de envío` → gasto logístico de cada pedido.  
- `Fecha de Compra` → fecha en formato datetime.  
- `Lugar de Compra` → identifica la tienda (1 a 4).  
- `Calificación` → evaluación del cliente (0 a 5).  
- `Método de pago`, `Cantidad de cuotas`, `lat`, `lon` → datos adicionales.

---

## 🛠️ Tecnologías usadas
- **Python 3.10+**  
- Librerías principales:
  - `pandas` → manipulación de datos
  - `matplotlib` → visualización
  - `seaborn` → gráficos de apoyo
  - `numpy` → operaciones numéricas

---

## 📈 Visualizaciones principales
El proyecto incluye tres gráficos refinados para mejorar la interpretación:

1. **Ingresos Totales por Tienda**  
   - Barras horizontales ordenadas.  
   - Azul = tienda líder, rojo = peor, gris = intermedias.  
   - Anotaciones con montos y diferencias porcentuales.  

2. **Calificación Promedio de Clientes**  
   - Barras horizontales con zoom en el rango 3.9–4.1.  
   - Verde = mejor tienda, rojo = peor.  
   - Línea de promedio general + etiquetas con delta %.  

3. **Costo de Envío Promedio por Tienda**  
   - Barras horizontales ordenadas.  
   - Verde = más eficiente, rojo = menos eficiente.  
   - Línea de referencia con el promedio + etiquetas comparativas.  

---

## 📝 Conclusiones del análisis
- **Tienda 1** → Mayor facturación, pero peor calificación promedio y costos de envío más altos.  
- **Tienda 3** → Mejor calificación promedio, ingresos sólidos y costos intermedios → *tienda con mayor potencial*.  
- **Tienda 4** → Menores ingresos, aunque con el costo de envío más bajo → *candidata a ser vendida*.  
- **Tienda 2** → Rendimiento intermedio en todos los indicadores.  

👉 **Recomendación:**  
Vender la **Tienda 4**, dado que combina el menor nivel de ingresos con una satisfacción del cliente que no compensa su baja eficiencia.  
Las otras tiendas muestran un mejor balance entre ingresos, satisfacción y costos.

---
