# Electronica-Digital-- #Reloj# ![C++](https://img.shields.io/badge/-C++-000000?style=flat&logo=c%2B%2B)
<a href="https://deepwiki.com/JEAS-14/Electronica-Digital---Reloj"><img src="https://deepwiki.com/badge.svg" alt="Ask DeepWiki"></a>

⏰ Reloj Electrónico Digital

Proyecto de construcción y diseño de un reloj electrónico digital, enfocado en la integración precisa de componentes lógicos para la medición y visualización del tiempo. Desarrollado en el curso de Electrónica Digital de la Universidad Privada del Norte. 

💡 Acerca del Proyecto

Este proyecto consiste en la construcción de un Reloj Electrónico Digital que integra de manera precisa componentes clave de electrónica digital para medir y mostrar la hora. El diseño utiliza la compuerta 555 como oscilador, contadores 74193 para el almacenamiento de unidades de tiempo (horas, minutos, segundos), y decodificadores 7447 para la visualización en displays de 7 segmentos. El proyecto no solo busca la funcionalidad, sino también la eficiencia en la gestión del tiempo y destaca su relevancia para el desarrollo en zonas rurales del Perú. 

![Diseño completo en Proteus](assets/proteus-reloj.png)

![Construcción física del circuito](assets/reloj-fisico.jpeg)

🎯 Objetivos

- Diseño Eficiente: Desarrollar un diseño funcional que integre la compuerta 555 como oscilador principal, los contadores 74193 y los decodificadores 7447 para una visualización clara en displays de 7 segmentos. 

- Precisión Temporal: Lograr una medición exacta del tiempo mediante la sincronización adecuada de los contadores y la gestión eficiente de las señales de reloj. 

- Aprendizaje Práctico: Proporcionar una experiencia práctica en el diseño y construcción de circuitos electrónicos digitales, mejorando las habilidades en la aplicación de principios de electrónica digital. 

🔑 Palabras Clave

- Compuertas lógicas 

- Circuito digital 

- Integración 

- Diseño de circuitos 

- Eficiencia 

- Temporización 

- Reloj 

📈 Importancia del Proyecto

La creación de este reloj electrónico representa un proyecto fundamental para el aprendizaje práctico y el desarrollo de habilidades en electrónica digital. Este proyecto no solo involucra el diseño e integración de compuertas lógicas, sino que también implica la aplicación directa de conceptos teóricos transmitidos durante el curso. 

🛠️ Tecnologías y Componentes Utilizados

- Compuerta 555 | Generador de pulsos (oscilador principal) para el sistema. 

- Contadores 74193 | Encargados de contar y almacenar las unidades de tiempo (segundos, minutos, horas) de manera sincronizada. 

- Decodificadores 7447 | Convierten las unidades de tiempo en señales para displays de 7 segmentos. 

- Compuertas 7408 (AND) | Utilizadas para la lógica de reseteo de los contadores. 

- Compuerta 7432 (OR) | Componente adicional utilizado en la lógica de las horas. 

- Displays de 7 Segmentos | Elementos visuales que muestran digitalmente el tiempo. 

- Proteus 9 Professional | Software de simulación para el diseño y verificación del circuito. 

🏗️ Proceso de Construcción

El proceso de construcción del reloj electrónico digital siguió una lógica secuencial para integrar sus diferentes módulos:

- Generación de Pulsos (Módulo de Segundos): Se utiliza una compuerta 555 para generar los pulsos de reloj. Se conectan dos contadores 74193 (uno en modo 10 y otro en modo 6 para el conteo hasta 59) y decodificadores 7447 para la visualización en displays de 7 segmentos. La lógica de reseteo se implementa con una compuerta 7408. 

 <img width="703" height="609" alt="image" src="https://github.com/user-attachments/assets/ff8ba2df-d329-4145-bf21-263de0d66e57" />

<img width="895" height="683" alt="image" src="https://github.com/user-attachments/assets/d23869c1-b174-482b-9caa-08eeccbacd77" />


- Integración de Minutos: El mismo proceso se replica para los minutos, utilizando dos 74193 adicionales y decodificadores 7447. El contador de minutos se activa con el reseteo del segundo 74193 de segundos.

   <img width="884" height="663" alt="image" src="https://github.com/user-attachments/assets/05dd27b4-6797-46d8-bab6-4e2afa6e5056" />

- Diseño de Horas: Se considera un conteo hasta 24 horas. Se añade una compuerta 7432 y se ajusta la lógica de reseteo con compuertas 7408 para el conteo adecuado, enlazando la salida del contador de minutos. 

<img width="884" height="917" alt="image" src="https://github.com/user-attachments/assets/cced21f8-44f5-4350-827e-69d936af0640" />


Ensamblaje y Verificación: Se realiza el diseño completo en Proteus y, posteriormente, se construye el formato físico en protoboard. 

<img width="884" height="392" alt="image" src="https://github.com/user-attachments/assets/73ce2c6e-f7fc-451b-8834-46de68735031" />

<img width="884" height="470" alt="image" src="https://github.com/user-attachments/assets/70ca05bf-d84c-43df-abce-6eff8c31292e" />




📊 Resultados

- La implementación del reloj se llevó a cabo con resultados satisfactorios, demostrando su funcionalidad. 

- El pulsómetro (compuerta 555) fue fundamental como base del funcionamiento. 

- La compuerta 74193 almacenó correctamente la salida para segundos, minutos y horas. 

- Los modos de reseteo (modo 6 y modo 10) se implementaron eficazmente. 

- La conexión con la compuerta 7447 permitió el control adecuado de los LEDs de siete segmentos para la visualización.

  <img width="884" height="613" alt="image" src="https://github.com/user-attachments/assets/2d12c25b-78a9-43e3-a088-48068f8d8076" />


⚠️ Limitaciones

- Sensibilidad del Cableado: Cualquier contacto mínimo puede afectar el funcionamiento de las compuertas lógicas. 


- Acceso y Voltaje de la Fuente de Alimentación: Es crítico que la fuente de poder proporcione el voltaje adecuado para evitar errores en la visualización. 


- Tiempo de Comprobación: La verificación de horas y minutos requiere esperar el tiempo estimado, lo que puede ser un desafío. 

💡 Recomendaciones

Para futuras investigaciones, se recomienda explorar y perfeccionar técnicas para mejorar el proceso de construcción del reloj. Esto podría incluir métodos más eficientes para la integración de componentes (555, 74193, 7447) y la exploración de nuevas herramientas y tecnologías que faciliten el montaje y ajuste del circuito. 

✅ Conclusiones

Este proyecto ha demostrado la viabilidad y aplicabilidad de los conceptos teóricos de electrónica digital, transformándolos en un producto funcional y tangible. La utilización efectiva de los componentes clave permitió diseñar un sistema que mide y muestra el tiempo con precisión. Además, el proceso de construcción mejoró las habilidades de diseño de circuitos y gestión de componentes, sirviendo como un punto de partida para la exploración en electrónica digital. 

🚀 Instalación y Simulación

Para explorar o simular el proyecto:

Clonar el repositorio:

Bash

git clone https://github.com/TuUsuario/NombreDeTuRepoDelReloj.git

cd NombreDeTuRepoDelReloj

Abrir en Proteus:

Abre los archivos de Proteus (ej. reloj_digital.pdsprj) en Proteus 9 Professional para visualizar el diseño del circuito y ejecutar la simulación.

(Opcional) Abrir Código (si lo subes):

Si subes el código, abre los archivos .ino o .cpp en tu IDE (ej. Arduino IDE) para revisar la lógica.

🧑‍💻 Autores

Juan Elias Arango Salvador 


Erick Daniel Carbajal Quiñonez 


Crisdel Aldemir Gonzales Canales 


Manases Neftali Huaman Churo 

Asesor:

Cesar Augusto Reyes Gutierrez 

Curso:

Electrónica Digital 

Carrera:

Ingeniería de Sistemas Computacionales 

Institución:

Universidad Privada del Norte - UPN 

✉️ Contacto
Si tienes preguntas o comentarios sobre este proyecto, no dudes en contactarnos:


Juan Elias Arango Salvador: N00334240@upn.pe 


Erick Daniel Carbajal Quiñonez: N00334471@upn.pe 


Crisdel Aldemir Gonzales Canales: N00333088@upn.pe 


Manases Neftali Huaman Churo: N00310402@upn.pe 

LinkedIn: linkedin.com/in/elias-juan-arango-salvador-87b782369
