# CESE-6Co2018_PCB
Poncho Procesador de Audio

El Poncho "Procesador de Audio" es una placa de circuito impreso que se diseñadara para ser montada sobre la EDU-CIAA-NXP. Dicho pcb le brindara a la EDU-CIAA-NXP el hardware necesario para realizar la generación y adquisición de audio. A su vez, implementará protecciones para proteger a la EDU-CIAA-NXP del mal uso del procesador.

Para la generación de audio el poncho posee un DAC PCM5100 para la generación de audio estéreo con un pin de Mute para poder controlar el encendido y apagado de la salida mediante un pin del lpc4337. Además, posee mapeado a la salida el DAC de salida de la EDU-CIAA-NXP para poder realizar desarrollo.

Para la adquisición de audio el poncho posee accesibles los canales 1 y 2 del ADC de la EDU-CIAA-NXP mediante el hardware pertinente para realizar el ajuste de niveles de entrada. Este incluye el agregado de un nivel de continua a la señal de audio adquirida, un ajuste de volumen y las protecciones pertinentes para la entrada del ADC. Además, se agregará un ADC por SPI con resolución de 16 bits y 96KHz de frecuencia de muestreo para realizar pruebas de adquisición

A su vez se agregará hardware para poder trabajar en monoestereo. Este utilizara un nivel de continua, canal derecho y canal izquierdo sumados mediante un amplificador operacional. Para las entradas y salidas de audio se utilizarán conectores miniplug de 3.5mm(4 en total).

Por último, se incluirán 3 leds para usar a modo de indicación de nivel de entrada y un buzzer.
