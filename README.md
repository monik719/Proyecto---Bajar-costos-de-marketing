# Proyecto---Bajar-costos-de-marketing
En un entorno empresarial altamente competitivo, **la eficiencia en la asignación de recursos** de marketing se ha convertido en un factor decisivo para el éxito de las organizaciones. El objetivo principal de este proyecto es la optimización de los gastos de marketing.
**Identificar y maximizar el retorno de inversión en marketing (ROMI) de las estrategias**, mediante un análisis exhaustivo de los canales.
.

#### Herramientas y tipo de proyecto
![Python](https://img.shields.io/badge/python-357ebd?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23357ebd.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-357ebd?style=for-the-badge)
![Numpy](https://img.shields.io/badge/numpy-%23357ebd.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/matplotlib-295F98?style=for-the-badge)
![Limpieza de datos](https://img.shields.io/badge/Limpieza_de_datos-295F98?style=for-the-badge)
![Transformación de datos](https://img.shields.io/badge/Transformación_de_datos-295F98?style=for-the-badge)
![Análisis de datos](https://img.shields.io/badge/Análisis_de_datos-295F98?style=for-the-badge)
![Análisis de cohortes](https://img.shields.io/badge/Análisis_de_cohortes-295F98?style=for-the-badge)

### Preguntas clave
1. ¿Cómo los clientes usan el servicio?
2. ¿Cuándo empiezan a comprar?
3. ¿cuánto dinero aporta cada cliente a la compañía?
4. ¿cuándo los ingresos cubren el costo de adquisición de los clientes?

### Descripción de los datos
La tabla visits (registros del servidor con datos sobre las visitas al sitio web):

- Uid: identificador único del usuario;
- Device: dispositivo del usuario;
- Start Ts: fecha y hora de inicio de la sesión;
- End Ts: fecha y hora de término de la sesión;
- Source Id: identificador de la fuente de anuncios de la que proviene el usuario.
Todas las fechas de esta tabla están en formato AAAA-MM-DD.

La tabla orders (datos sobre pedidos):

- Uid: identificador único del usuario que realiza un pedido;
- Buy Ts: fecha y hora del pedido;
- Revenue: ingresos de Y.Afisha de este pedido.
  
La tabla costs (datos sobre gastos de marketing):

- source_id: identificador de la fuente de anuncios
- dt: fecha;
- costs: gastos en esta fuente de anuncios en este día.

### Metodología
- **Preprocesamiento de datos:** Se limpiaron y estandarizaron los datos, eliminando inconsistencias y verificando la ausencia de duplicados y valores faltantes.
- **Analisis exploratorio de los datos (EDA):**
- **Informes y calculo de metricas:**
  1. **Visitas:** Se analizaron la cantidad de personas que visitan la pagina cada semana mes, ect. Identificando patrones del número de sesiones, como la duración de la misma, tambien la frecuencia con la que regresan.
  2. **Ventas:** Se identifico en que momento el usuario se vuelve cliente, asi como la cantidad de pedidos que hacen en un determinado tiempo, tiempo de compra y cuanto dinero traen **LTV (total de dinero que un cliente aporta a la empresa en promedio al realizar compras)**.
  3. **Marketing:** Se analizo **por cada fuente y cohorte** (usuarios ingresados en un cierto tiempo), cuando dinero se gasto a lo largo del tiempo como el costo de adquisicion de clientes. **Identificando cuan rentables eran las inversiones de cada fuente ROMI**
     
### Conclusiones y recomendaciones
- En ninguna de las cohortes, ni en su ciclo de vida ha dado los resultados esperandos, cabe aclarar que se establecio un margen de benefio del 30%.
- la cohorte 10,11 y 12 del 2017 son las que mas pedidos realizaron.
- la fuente mas efectiva de conversion es la id 10, y la ffuente 1 es  que la que tiene mas personas que se demoran en convertirse.
- En cuanto al retorno de la inversion las fuentes icdfhoifb

#### Recomendaciones:
- Descontinuar las fuentes 7, 9 y 10 debido a su bajo rendimiento.
- Reducir la inversión en la fuente 3, ya que no genera retornos significativos.
- Invertir en la fuente 1, que sigue siendo una aliada clave con baja inversión y alto rendimiento.

### Visualizaciones destacadas
1. **Costo de adquisicion de cada una de las fuentes:** Se pudo observar que la fuente id 3, es en la que mas se ha gastado en marketing y la fuente id 4 a comparación de la 3, tiene menos gastos en marketing, mas visitantes y mas personas convertidas a clientes.
![Tabla costos por fuente y cohorte](https://github.com/monik719/Portafolio/blob/main/assets/costos%20marketing%20fuentes.png).

2. **ROMI de la fuente 5:** En las primeras 5 cohortes se ve reflejado el retorno de la inversion, en cada una de ella. Pero enfocandonos en la cuarta esta genero hasta cuatro veces mas ganancia en varios meses de vida. pero en las demas cohortes no se reflejado la rcuperacion de la inversión.
   ![ROMI fuente 5](https://github.com/monik719/Portafolio/blob/main/assets/fuente5.png)
