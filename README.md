# Spike-Challenge
Combatiendo el cambio climático con Machine Learning!

El presente repositorio cuenta con mis respuestas para el desafío Spike Octubre 2019 - Predicción de caudales extremos en Chile.
Recomiendo descargar tanto el notebook: https://github.com/xaerincl/Spike-Challenge/blob/master/SpikeChallengeOscarM.ipynb como el modelo entrenado https://github.com/xaerincl/Spike-Challenge/blob/master/modelo_final.h5 .



## Motivación

Nota: este segmento de motivación es para que entiendan un poco más del problema y por qué es relevante. No es necesario que entiendan todo, el resto del desafío los irá guiando en las cosas específicas que deben hacer. En otras palabras: lean esto rápido y luego concéntrense en las preguntas e instrucciones del desafío.

Las olas de calor son eventos meteorológicos extremos (temperaturas extremas), que pueden generar impactos negativos en nuestro ecosistema. Estos impactos van desde días de verano muy calurosos, deshidratación, hasta aumento del riesgo de incendios y riesgo de aluviones por crecidas de los ríos (por derretimiento de nieve o lluvias líquidas en zonas altas de la cordillera).
Dado que las olas de calor responden a patrones de circulación atmosférica que pueden ser detectadas con días e incluso semanas de anticipación, existe una oportunidad sin precedentes de intentar predecir la ocurrencia de algunos de los impactos negativos asociados a estos eventos extremos. Esto es clave en el contexto de calentamiento global, en donde la frecuencia a escala global de este tipo de eventos extremos ha aumentado en el último siglo (https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2012GL053361).
Para explorar esta potencial predictibilidad de los impactos asociados a las olas de calor, en particular los eventos de peakflows (crecidas de ríos, los que en casos extremos pueden llegar a desbordar el cauce), en Chile contamos con una amplia red de monitoreo de variables hidro-meteorológicas. Las estaciones meteorológicas que miden temperatura y precipitación son mantenidas por la Dirección General de Aguas (DGA) y la Dirección Meteorológica de Chile. Para potenciar el uso y la generación de conocimiento en base a estos datos públicos, el Centro de Ciencia del Clima y la Resiliencia (CR2) desarrolló un explorador climático (http://explorador.cr2.cl), desde el cual se pueden visualizar y descargar estos registros.

En el explorador climático se encuentran también los datos de caudal de las estaciones fluviométricas de la DGA, los que representan el agua total que aporta una cuenca hidrográfica a una sección de río. En el CR2 también se generó una base de datos de cuencas, que provee una serie de atributos de cada área aportante a las estaciones fluviométricas (http://camels.cr2.cl), además de series meteorológicas de temperatura y caudal promediadas dentro de la cuenca (es decir, no son datos de estaciones puntuales, sino que agregados espacialmente sobre el polígono de cada cuenca). 

Algunas de las preguntas claves que en Chile debemos responder son:
- ¿Ha aumentado la frecuencia de olas de calor en Chile? Para esto se deben analizar las estaciones de temperatura.
- ¿Existe una relación entre olas de calor y eventos extremos de caudal? 
- De existir una relación entre olas de calor y eventos extremos de caudal, ¿se puede explicar este evento extremo por las características de la cuenca en donde ocurre el peakflow?
