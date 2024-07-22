## Trabalho Prático 2 — Contador Automatizado de Fichas de Sinuca

<div class="small">

Problemas relevantes merecem ser revisitados e aprimorados sempre que possível, por isso, este problema do ano de 2017 será abordado na nossa disciplina prática por grupos de até sete componentes.

</div>

### Objetivos

<div class="small">

1. Construir um sensor discretizado de luminosidade com um LDR para detectar abertura e fechamento da gaveta de fichas de sinuca.
    - Como é possível ver neste [vídeo](https://www.youtube.com/watch?v=WTS_p4C4cXs) o mecanismo de abertura da gaveta da mesa de sinuca trava a alavanca que empurra a gaveta até o momento em que uma ficha é inserida. Portanto, quando não existem fichas inseridas, a alavanca não consegue empurrar completamente a gaveta para abri-la, o que deixa um espaço entre a gaveta e a alavanca onde pode ser inserido um resistor dependente de luminosidade em frente a um LED sempre aceso, que mantém a resistência do LDR em um valor baixo. Quando uma ficha é inserida, a alavanca empurra a gaveta para abri-la e se coloca entre o sensor e o LED, o que faz com que a resistência do LDR aumente considerávelmente. A partir destes fatos, você deverá construir um sensor de luminosidade discretizado com LDR, LED e um transistor NPN ou PNP (BC548 por exemplo) para detectar se a gaveta da ficha de sinuca encontra-se aberta ou fechada.
2. Construir um autômato de estados finitos para mapear os estados da mesa de sinuca.
3. Manter registro da contagem das fichas de sinuca inseridas até o momento na mesa.
4. Informar a cada nova inserção de ficha o total de fichas inseridas até o momento por meio do protocolo MQTT na plataforma Adafruit.IO.
5. Informar se a mesa de sinuca se encontra aberta a muito tempo (travada para uso) também por meio de MQTT na plataforma Adafruit.IO.

As etapas 2, 3, 4 e 5 estão completamente descritas nos comentários do arquivo `coin-counter.ino` disponível no [zip](https://ava.cefetmg.br/pluginfile.php/309192/mod_assign/introattachment/0/coin-counter.zip?forcedownload=1) do TP2 no Moodle (AVA).

</div>
