# Objetivo principal #

## En breves lineas, el objetivo principal del trabajo es crear un modelo de regresión logística para predecir si un paciente padece o no de una enfermedad en el corazón, a través de 11 características que posee el Heart Failure Prediction Dataset.
![Imagen de WhatsApp 2024-07-24 a las 12 50 13_7e5648cf](https://github.com/user-attachments/assets/77408243-2bb0-477c-8f09-7b47c7f60fad)

# Introducción 
## Las enfermedades cardiovasculares (ECV) son la principal causa de muerte en el mundo y se cobran aproximadamente 17,9 millones de vidas cada año, lo que representa el 31 % de todas las muertes en el mundo. Cuatro de cada cinco muertes por ECV se deben a ataques cardíaco y accidentes cerebrovasculares, y un tercio de estas muertes ocurren de forma prematura en personas menores de 70 años. La insuficiencia cardíaca es un evento común causado por ECV y este conjunto de datos contiene 11 características que se pueden utilizar para predecir una posible enfermedad cardíaca.

## Las personas con enfermedad cardiovascular o que tienen un alto riesgo cardiovascular (debido a la presencia de uno o más factores de riesgo como hipertensión, diabetes, hiperlipidemia o enfermedad ya establecida) necesitan una detección y un tratamiento tempranos en los que un modelo de aprendizaje automático puede ser de gran ayuda. El conjunto de datos seleccionado para este trabajo se creó combinando 5 conjuntos de datos que ya estaban disponibles de forma independiente pero que no se habían combinado antes, estos son:
### • Cleveland: 303 observaciones
### • Húngaro: 294 observaciones
### • Suiza: 123 observaciones
### • Long Beach, Virginia: 200 observaciones 
### • Conjunto de datos de Stalog (corazón): 270 observaciones
###### Total: 1190 observaciones
###### Duplicadas: 272 observaciones
###### Dataset Final: 918 observations

# Consideraciones a tener en cuenta
## 1. Para poder crear el modelo de regresión logística se realizó una conversión de las variables de tipo cualitativa a cuantitativa. La variables cualitativas quedaron estructuradas de la siguiente forma:
#### • Sexo: [M = 1, F = 0]
#### • ChestPainType: [TA = 3, ATA = 1, NAP = 2, ASY: 0]
#### • RestingECG [Normal = 1, ST = 2, HVI = 0]
#### • ExerciseAngina: [Y = 1, N = 0]
#### • STSlope: [Up = 2, Flat = 1, Down = 0]
## 2. Encontramos en el Heart Failure Prediction Dataset , que numerosas filas tenían valor 0 en la columna Colesterol, lo cuál es imposible clínicamente, esto significa que no se contaba con la medida del Colesterol de esos pacientes, para continuar con nuestro modelo de regresión reemplazamos los valores 0 por la media de los valores que no son 0 en la columna Colesterol. La media es de aproximadamente 244.
