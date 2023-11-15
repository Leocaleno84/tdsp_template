# Project Charter - Entendimiento del Negocio

## Nombre del Proyecto

#### Despliegue Modelo Estimación de Precios de Energía de Corto Plazo
## Objetivo del Proyecto

- Utilizando los modelos desarrollados a través del diplomado, el objetivo es implementar y desplegar el modelo de estimación de precios de energía usando Deep learning para que un usuario final pueda alimentarlo y tener resultados sin necesidad de entender la programación realizada.

## Alcance del Proyecto

### Incluye:

- [Descripción de los datos disponibles]
- - El dataset ofrece utilizado ofrece una visión de la dinámica del mercado eléctrico colombiano durante los años 2008 a 2023 en resolución diaria. El conjunto permitirá realizar análisis e inferir implicaciones de las correlaciones entre las diferentes variables y su peso en la determinación de los precios de la energía. El ejercicio se puede llevar a una complejidad mayor con detalle horario de las variables, sin embargo, por practicidad se trabajarán con los datos diarios.

- Los datos se descargan en formato txt del ftp del operados del sistema eléctrico colombiano.

- Se manejaran variables numéricas y categóricas sobre las cuales se debe hacer one hot encoding.
-
Descripción de los Datos.

| Variable | Detalle                     |
| -------- | ------------------------------ |
| Fecha    | Fecha de operación del mercado |
|NombreDiaSemana| Día de la semana de operación|
|DiaSemana|Codificación para el día de la semana, Lunes=1, Domingo =7|
|TipoDia|Tres tipos: Laborales=1, Sábados=2, Festivos=3|
|PBNA|Precio Promedio Día de Energía en Bolsa en $/kWh|
|DemandaDia|Demanda en GWh-día|
|AportesEnergíaSIN|Cantidad de lluvia del día a nivel nacional en GWh-día|
|AportesSIN_Porc|Lluvias del día en % respecto a la media histórica.|
|VolumenEnergíaSIN|Nivel de embalses agregados a nivel nacional del día|
|VolumenUtil_Porc|Nivel de embalses en %|
|IndisponibilidadHidraulica|Indisponibilidad en GWh-día de recursos hidráulicos|
|IndisponibilidadTermica|Indisponibilidad en GWh-día de recursos térmicos|
|G_Hidro|Generación Hidráulica del día en GWh-día|
|G_termico|Generación Térmica del día en GWh-día|
|G_Menor|Generación No despachada Centralmente en GWh-día|
|AportesAntioquia|Aportes en % en la región.|
|VolumenAntioquia|% Nivel de embalses en la región en referencia a su nivel máximo.|
|AportesCaribe|Aportes en % en la región.|
|VolumenCaribe|% Nivel de embalses en la región en referencia a su nivel máximo.|
|AportesCentro|Aportes en % en la región.|
|VolumenCentro|% Nivel de embalses en la región en referencia a su nivel máximo.|
|AportesOriente|Aportes en % en la región.|
|VolumenOriente|% Nivel de embalses en la región en referencia a su nivel máximo.|
|AportesValle|Aportes en % en la región.|
|VolumenValle|% Nivel de embalses en la región en referencia a su nivel máximo.|

- [Descripción de los resultados esperados]

La estimación tanto de los precios de la energía como de la demanda de energía son unas tareas muy importantes y complejas dado el actual modelo de transición energética. Tener un buen pronostico de estas dos variables permite tener un insumo adecuado para la toma de decisiones de inversión, expansión del sistema, compra de combustibles, reserva de recursos hidráulicos dependiendo de la expectativa climatológica (lluvias) para lograr un balance adecuado de generación hidrotérmica que no afecte los precios a corto plazo pero que tampoco ponga en riesgo el suministro en el mediano plazo.

De manera particular, la previsión de los precios de energía en bolsa a corto plazo es un instrumento esencial para la planificación de la operación de las plantas de generación de energía, más cuando estás son centrales térmicas que tienen que contratar combustibles para su operación.

## Metodología

[Descripción breve de la metodología que se utilizará para llevar a cabo el proyecto]
Se utilizará la metodología CRISP-DM, que ha sido la metodología usada a lo largo del diplomado.

## Cronograma

| Etapa | Duración Estimada | Fechas |
|------|---------|-------|
| Entendimiento del negocio y carga de datos | 1 semanas | del 07 al 14 de noviembre |
| Preprocesamiento, análisis exploratorio | 1 semanas | del 15 al 21 de noviembre |
| Modelamiento y extracción de características | 1 semanas | del 22 al 28 de noviembre |
| Despliegue | 1 semanas | del 29 de noviembre al 05 de diciembre |
| Evaluación y entrega final | 4 días | del 05 al 08 de diciembre |

## Equipo del Proyecto

- [Nombre y cargo del líder del proyecto]
> [!Leonardo Fajardo Bernal]

