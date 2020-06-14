# Saperi - Composición musical con inteligencia artificial

**Proyecto Final Informática Musical, Facultad de Informática, Universidad Complutense de Madrid**

_**Autor:** Alberto Pastor Moreno_

_**Grupo:** 15, Moogers_

_**Repositorio GitHub:** https://github.com/albertopastormr/saperi_

## Descripción

Saperi es un proyecto de composición musical utilizando únicamente en el desarrollo creativo herramientas de inteligencia artificial. Durante el desarrollo del proyecto he probado las herramientas más avanzadas en la predicción creativa musical, componiendo tres piezas con Magenta Studio, Music Transformer y MuseNet. Todas estas herramientas, las cuales trabajan sobre MIDI y no audio en crudo, se basan en algoritmos de inteligencia artificial entrenados sobre cientos de miles de obras musicales con el objetivo de predecir el siguiente conjunto de notas con sus tiempos y duraciones.

## Tecnología utilizada

### Magenta Studio

Magenta Studio es una colección de utilidades de composición musical con inteligencia artificial open source desarrollado por GoogleAI utilizando el framework Tensorflow. Esta herramienta tiene una aplicación standalone y un plugin para Ableton Live. Las utilidades que contiene son las siguientes:

- _Continue:_ dado un clip MIDI, produce otro clip MIDI que pueda funcionar como consecución a la referencia. Trabaja con clips de batería y de melodía.
- _Generate:_ genera un clip MIDI de una duración de 4 compases de melodía o de batería sin tomar referencias. 
- _Drumify:_ produce un clip MIDI de batería que acompañe a una melodía indicada.
- _Interpolate:_ dados dos clips MIDI de melodía o de batería, los mezcla produciendo un clip MIDI nuevo que transiciona entre los dos clips originales.
- _Groove:_ le aporta a un clip MIDI de batería el _feel_ de la actuación de un baterista humano, modificando el tiempo y nivel de cada nota del clip.

El resultado del proceso creativo de composición con esta herramienta se puede escuchar [aqui](Magenta-Studio.mp3)

### Ableton Live

Para desarrollar la pieza musical explicada en el apartado anterior utilicé Ableton Live 10.1 Suite, DAW que tiene integración nativa con el plugin Magenta Studio. La vista de sesión de este DAW me permitió probar ágilmente diferentes configuraciones del plugin ya que el manejo de clips exportados por éste es realmente rápido. La línea de bajo utiliza el VST _iZotope Iris 2_, la percusión utiliza el kit de percusión incluido en el DAW llamado _Crystal Clear Kit_ y el instrumento punteado utiliza el VST _Analog Dreams_ de _Kontakt_.

### Music Transformer

Music Transformer es una herramienta de composición de piezas musicales en piano considerando estructuras de larga duración. A diferencia de lo producido con Magenta Studio, con Music Transformer he podido producir una pieza de 5 minutos de duración sobre la cual se pueden distinguir diferentes partes coherentes entre sí. Esta herramienta predice las siguientes notas dada una secuencia recursiva, al igual que Magenta Studio, pero tiene consideración de la estructura musical de toda la pieza. 

El resultado del proceso creativo de composición con esta herramienta se puede encontrar [aquí](Music-Transformer.mp3)

### MuseNet

MuseNet es una herramienta de composición de piezas musicales por fragmentos con hasta 10 instrumentos diferentes, desarrollada por OpenAI, que permite basarse en el estilo de grandes compositores como Mozart, Chopin o Beethoven, utilizando instrumentos que no eran típicos en sus obras. Utilizando esta herramienta he producido una pieza basada en el estilo de Beethoven.

El resultado del proceso creativo de composición con esta herramienta se puede encontrar [aquí](MuseNet-Beethoven.mp3)

## Futuro de Saperi

El futuro de Saperi se encuentra en la integración de herramientas potentes como Music Transformer o MuseNet en el entorno de trabajo de un artista en la actualidad, el DAW. Para lograr una usabilidad creativa rica, enfocada en usuarios no expertos en inteligencia artificial, considero necesario poder entrelazar las utilidades vistas en este proyecto. Así, las funcionalidades que aportan se podrían enriquecer entre ellas, pudiendo lograr cubrir un mayor espectro del desarrollo creativo musical, ya que actualmente estas herramientas solo nos ayudan en ciertas fases, como por ejemplo en la composición de percusión en base a una melodía existente.

## Bibliografía

- \[1]: [Magenta Studio: Augmenting Creativity with Deep Learning in Ableton Live](https://research.google/pubs/pub48280/)
- \[2]: [Learning to Create Piano Performances](https://research.google/pubs/pub46748/)
- \[3]: [Approachable music composition with machine learning at scale](https://research.google/pubs/pub48629/)
- \[4]: [Learning to Groove with Inverse Sequence Transformations](https://research.google/pubs/pub48238/)
- \[5]: [DDSP: Differentiable Digital Signal Processing](https://openreview.net/forum?id=B1x1ma4tDr)
- \[6]: [Magenta Studio](https://magenta.tensorflow.org/studio-announce)
- \[7]: [Magenta Studio: Ableton Live](https://magenta.tensorflow.org/studio/ableton-live)
- \[8]: [Music Transformer: Generating Music with Long-Term Structure](https://magenta.tensorflow.org/music-transformer)
- \[9]: [Ableton Reference Manual](https://www.ableton.com/en/manual/welcome-to-live/)
- \[10]: [MusicVAE: Creating a palette for musical scores with machine learning](https://magenta.tensorflow.org/music-vae)
- \[11]: [MuseNet](https://openai.com/blog/musenet/)
- \[12]: [The MAESTRO Dataset and Wave2Midi2Wave](https://magenta.tensorflow.org/maestro-wave2midi2wave)
