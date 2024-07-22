## MQTT

<div class="regular">

MQTT (Message Queuing Telemetry Transport) é um protocolo de mensagens leve e simples, projetado para dispositivos com pouca largura de banda — que estão em conexões lentas junto a internet — e alta latência — que estão em conexões instáveis, cujos pacotes podem ser perdidos ou atrasados.

Ele é baseado em um modelo de publicação/assinatura, onde partes interessadas se conectam a um servidor MQTT (broker — corretor, negociador, intermediário) e enviam ou recebem mensagens através de tópicos.

</div>

### MQTT - Tópicos, _Publishers_ e _Subscribers_

<div class="regular">

Tópicos são identificadores textuais que são usados para separar (e categorizar) as mensagens gerenciadas pelo broker. Normalmente são compostos por uma ou mais palavras separadas por barras (`/`), como `temperatura/belo_horizonte`.

Dispositivos que precisam enviar mensagens devem publicá-las em um tópico, enquanto dispositivos que precisam receber mensagens devem se inscrever em um tópico.

O broker recebe as mensagens publicadas nos tópicos e as envia para todos os dispositivos inscritos nos tópicos correspondentes.

Uma estação metereológica na cidade de belo horizonte pode **publicar** sua temperatura atual (a cada intervalo pré-definido) no tópico `temperatura/belo_horizonte`, enquanto um aplicativo de celular pode se **inscrever** nesse tópico para <ins>receber</ins> a temperatura atual da cidade.

</div>
