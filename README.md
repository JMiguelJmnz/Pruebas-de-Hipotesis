# Pruebas de Hipotesis

Análisis de pruebas de hipótesis para un modelo de regresión lineal múltiple mediante matrices de manera que puedas establecer qué variables son adecuadas en un proceso predictivo.

Tomamos los datos ya cargados para comenzar
<br>![image](https://github.com/user-attachments/assets/0833d5c3-52dd-4dcc-bed3-b26ff3b95bd5)

Comenzamos calculando la información necesaria, como los betas
<br>![image](https://github.com/user-attachments/assets/ce7e56f7-01e4-4eab-9c44-ce06bdbd3008)

Nuestra R cuadrada y R cuadrada ajustada comienzan en 65.2%
<br>![image](https://github.com/user-attachments/assets/deb1d0a2-ff3e-480a-9267-19ac24fb8516)

Calculamos la varianza, desviacion y las t’s estadísticas
<br>![image](https://github.com/user-attachments/assets/fa84381b-6709-4f9b-b6dc-dd2f8646c4f2)

Revisamos la significancia con las betas
<br>![image](https://github.com/user-attachments/assets/ec5638f7-f31d-4427-b529-0fa15583ff46)

El valor de p de beta nos corrobora la significancia de las variables 9 y 11, siendo que son las que se acercan más a 1
<br>![image](https://github.com/user-attachments/assets/ed590c4d-357b-4d6c-ba85-cb42c94101a3)
<br>![image](https://github.com/user-attachments/assets/dd30c533-b87d-4823-b825-99cd7986c712)

Con el resumen de OLS podemos observar lo observado anteriormente con el Criterio 1 y 2
<br>![image](https://github.com/user-attachments/assets/df174a0f-3594-4ce8-9ff3-461b396fb3eb)

Tomando en cuenta betas no significativas en el criterio 1 y el valor de p en el criterio 2, la primer variable a eliminar seria la 8 debido a que su valor p es el más cercano a 1, seguido de beta 10 en caso de ser necesario
<br>![image](https://github.com/user-attachments/assets/ef05a49a-335e-48a2-8355-e457a4278fed)

El valor P más alto es el de la variable 9 por lo que procedemos eliminandola para repetir el modelo
<br>![image](https://github.com/user-attachments/assets/0621762d-fd73-44ef-8a2b-7ce364e7c65d)

Utilizamos Recursive Feature Elimination para seguir seleccionando las variables menos importantes primero
<br>![image](https://github.com/user-attachments/assets/a0e1954e-a3bf-4a27-922c-a7bb731e08ab)

Al seguir removiendo variables, los valores de R2 y R2 ajustada continúan bajando, en este punto lo mejor seria buscar otro modelo con cual evaluar esta información
<br>![image](https://github.com/user-attachments/assets/450c521f-bb25-415f-bcb4-05391404734a)
