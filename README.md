# S14--TELECOMUNICACIONES
Identificar a los operadores menos eficaces de una empresa de telecomunicaciones; y creación de Dashboard.

## Descripción 
Identificar a los operadores menos eficaces mediante los siguientes indicadores:
* La cantidad de llamadas entrantes perdidas (internas y externas).
* El tiempo de espera a las llamadas entrantes.
* Cantidad de llamadas salientes.

En la presentación se definen las características del dashboard creado en Tableu.

## Herramientas utilizadas
![Python](https://img.shields.io/badge/:Python-024A86?style=for-the-badge&logo=python&logoColor=white&labelColor=101010)</br>
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/seaborn-%233F4F75.svg?style=for-the-badge&logo=seaborn&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white)
![Datetime](https://img.shields.io/badge/datetime-%233F4F75.svg?style=for-the-badge&logo=datetime&logoColor=white)


![Tableu](https://img.shields.io/badge/:Tableu-8C4966?style=for-the-badge&logo=microstrategy&logoColor=white&labelColor=101010)</br>
![Google Drive](https://img.shields.io/badge/Google%20Drive-4285F4?style=for-the-badge&logo=googledrive&logoColor=white)

![Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)


## Conclusiones
Dado que las pruebas de hipótesis resultaron en rechazar las hipotesis nulas, quiere decir que se obtuvieron los valores de las métricas en las culaes los grupos de los operadores eficientes y no eficientes pueden ser diferenciados con un valor de alpha (precisión) de 5% . 
Esos valores son, para identificar a los operadores menos eficientes:
- La cantidad de llamadas entrantes perdidas totales es mayor a 4. 
- La cantidad de llamadas entrantes perdidas internas es mayor a 1.
- La cantidad de llamadas entrantes perdidas externas es  mayor a 4.
- El tiempo de espera a las llamadas entrantes es mayor a 44 unidades de tiempo.
- Cantidad de llamadas salientes es menor a 101.

Se recomienda combinar varios parámetros para tomar decisiones. Además de felicitar a aquello valores atípicos, por ejemplo los operadores que hicieron gran tantidad de llamadas o aquellos que tuvieron tiempos de espera más cortos a la media.

## Profundización técnica
* Descomposicón de proyecto: 
* *  Contestar : ¿A quién y por qué le interesa este análisis? ¿Qué se quiere conseguir? ¿Qué decisiones se tomaran de acuerdo al análisis?
  *  Propuesta de hipótesis.
  *  Planeación de pasos a seguir : Exploración, preprocesamiento, visualizaciones, pruebas de hipótesis.
  *  * Exploración de datos:
     * * Nombres de columnas a snake_case
       * Manejo de valores auscentes , ¿Qué puede estar sucediendo para que falten estos datos?
       * Manejo de valores duplicados
    * Análisis de datos:
    * * Cálculos de interés
      * Manejo de ouliers
      * Visualizaciones y estadísticos para ver distribución de los datos
    * Pruebas estadísticas para pruebas de hipótesis:
    * * Prueba de Levene - par ver si varianzas de los grupos son estadísticamente iguales, para settear valor de equal_var en ttest.
      *  Taylor test de 1 cola entre dos poblaciones (ttest_ind)  : ((results[1] / 2) < alpha) and (group_1[column].mean() > group_2[column].mean()) - se rechaza hipótesis nula.
* 
