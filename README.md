# Mi Observatorio Financiero

Aplicación educativa construida con Python y Streamlit en la S23.

## Qué permite hacer la aplicación

● Elegir activos financieros y consultar su comportamiento histórico en diferentes horizontes de tiempo.

● Visualizar precios normalizados (base común) para comparar el rendimiento relativo de los activos de forma equitativa.

● Analizar indicadores clave como el rendimiento acumulado, la volatilidad (riesgo) y las medias móviles.

● Consultar matrices o gráficos de correlación entre los activos seleccionados para evaluar la diversificación.

## Ejecución

```bash
pip install -r requirements.txt
streamlit run app.py
```

## Funcionalidades
Selección de tickers, comparación de precios, rendimiento, volatilidad y estadística descriptiva.

## Fuente
Yahoo Finance mediante yfinance; si falla, la app informa que utiliza datos simulados.

## Qué significan sus indicadores
● **Precios normalizados:** Ajustan los precios de distintos activos a un valor inicial común (por ejemplo, base 100) para poder evaluar qué acción o activo creció más proporcionalmente, sin importar el precio nominal de su acción.

● **Rendimiento:** Mide la ganancia o pérdida porcentual obtenida por el activo en el período seleccionado utilizando cambios porcentuales (pct_change()).

● **Volatilidad:** Representa la desviación estándar de los rendimientos, anualizada multiplicándola por la raíz cuadrada de 252 (días bursátiles del año). Indica qué tan inestable o riesgoso es el activo.

● **Medias móviles:** Promedian los precios de un activo en una ventana de tiempo específica (ej. 20 o 50 días) para suavizar la fluctuación y ayudar a identificar tendencias del mercado.

● **Correlación:** Mide cómo se mueven dos activos entre sí en una escala de -1 a 1. Una correlación cercana a 1 indica que se mueven en la misma dirección, mientras que una cercana a -1 o 0 muestra baja relación o movimientos opuestos, ideal para diversificar carteras.
## Autor e interpretación
Completar con tu nombre y un breve análisis de los resultados.
