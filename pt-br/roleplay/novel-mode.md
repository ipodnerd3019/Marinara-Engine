# Novel Mode: escrever uma história em parceria

Este guia explica o Novel Mode no Marinara Engine. O Novel Mode transforma um chat de Roleplay em uma única página contínua, como um manuscrito, em que você e a IA escrevem uma história juntos. Ele mostra como começar um romance, escrever e editar trechos, orientar a IA e ouvir a história.

## O que é o Novel Mode

O Novel Mode é um estilo de exibição para chats de Roleplay. A história é lida como uma única página em vez de um chat: não há avatares, nomes, horários nem balões de mensagem. Cada vez que a IA escreve, ela adiciona um trecho à página. Os parágrafos têm recuo como em um livro impresso, e os trechos seguem um após o outro sem quebra.

Diferente de um roleplay comum, a IA também escreve o seu protagonista. Ela escreve as ações, as falas e os pensamentos dele, então a história continua andando sem esperar a sua vez. Em vez disso, você a orienta escrevendo trechos próprios, editando o que já está na página e dando orientações curtas para o próximo trecho.

Por baixo, um romance continua sendo um chat de Roleplay. Lorebooks, resumos, memória, ramificações e agentes funcionam do mesmo jeito que em qualquer roleplay.

Com vários personagens, um romance sempre usa o modo de grupo **Merged** (mesclado): a IA escreve todos os personagens com uma só voz, como faz um romancista, então não há turnos para revezar. Nos romances, **Chat Settings** (configurações do chat) esconde as opções de modo de grupo, ordem de resposta e cor dos diálogos. O **Scenario Override** (substituição do cenário) do grupo continua valendo.

## Começar um romance

1. Comece um novo chat de Roleplay.
2. Na primeira etapa do assistente de configuração, defina **Display style** (estilo de exibição) como **Novel** (romance).
3. Conclua o assistente. Personagens e persona são opcionais. Adicione personagens só se quiser os cards de personagem deles no contexto da história.

Escolher **Novel** mantém os seus agentes, como em qualquer roleplay. Sprites, o HUD e os efeitos de clima aparecem quando os agentes por trás deles estão ativados (Expression Engine, World State e os agentes de tracker); remova esses agentes no assistente ou em **Chat Settings** para ter uma página limpa. Os romances mostram um ícone de livro na lista de chats.

Escolher **Novel** também seleciona o **Marinara's Novel Preset**, que diz à IA para escrever o seu protagonista (veja abaixo). Você pode escolher outro preset na etapa **Preset** do assistente ou mais tarde em **Chat Settings**. Se você voltar para outro estilo de exibição no mesmo assistente, o seu preset anterior volta, a menos que você tenha escolhido um diferente nesse meio-tempo.

## Escrever e editar

- **Adicionar o seu próprio texto:** digite na linha no fim da página, que mostra **Keep writing, or press Send…** (continue escrevendo ou pressione Enviar). Quando você sai da linha ou pressiona **Send** (enviar), o seu texto vira o próximo trecho da história.
- **Editar qualquer coisa na página:** a página inteira é um único editor. Clique em qualquer lugar e digite, como em um processador de texto. As suas alterações são salvas sozinhas um instante depois que você para de digitar, e **Ctrl+Z** as desfaz.
- **Formatação:** o texto de um trecho pode ficar em *itálico* ou em **negrito**. Selecione-o e pressione **Ctrl+I** ou **Ctrl+B** (**Cmd** no Mac). Ele é salvo como markdown, como `*italic*` e `**bold**`, e `*text*`, `_text_`, `**text**` e `__text__` que já estejam em um trecho aparecem em itálico e em negrito. Qualquer outra marcação, como títulos, listas, links e HTML, aparece como texto simples e não recebe tratamento especial. As quebras de linha são mantidas: um trecho cujos parágrafos estão em linhas simples continua assim quando você o edita.
- **Selecionar entre trechos:** você pode selecionar, copiar e excluir texto que se estende por vários trechos. Cada trecho continua sendo uma parte própria da história: excluir através de vários tira texto de cada um, nunca os trechos em si. Se você esvaziar um trecho por completo e seguir em frente, o Marinara pergunta se deve excluí-lo.
- **Ações do trecho:** aponte para um trecho, ou coloque o cursor nele, para ver as ações dele na margem: copiar, traduzir, gerar de novo, marcador, fixar ou nota, **Mark as new start** (marcar como novo início), ocultar da IA, ramificar e excluir, além de **Speak** (falar) quando o texto para fala está ativado. O último trecho também tem **Peek prompt** (espiar o prompt), e um trecho escrito com orientação tem **Stored guidance** (orientação salva), que mostra a direção que foi dada a ele. No celular, toque no trecho, ou mova o cursor para ele, para mostrar as ações.

## Pedir mais à IA

A barra de mensagem abaixo da página funciona como em qualquer roleplay, com uma diferença: o que você digita ali nunca vira uma mensagem. Só orienta o próximo trecho.

- **Send** com a barra vazia escreve os próximos parágrafos da história.
- Digite uma direção curta, como `a storm arrives` ("chega uma tempestade"), e pressione **Send**. A IA leva o próximo trecho nessa direção sem escrevê-la na história.
- Comandos de barra, ditado e os seletores de conexão e de persona funcionam como de costume. Anexos e as respostas rápidas **Post only** (só publicar) e **Guide reply** (guiar a resposta) não são oferecidos: nada do que você publica vira uma mensagem, e **Send** já envia o seu texto como orientação.
- Impersonate não é oferecido em um romance: não há uma vez sua para escrever, porque a IA já escreve o seu protagonista. O comando `/impersonate`, a resposta rápida Impersonate e as configurações de Impersonate do chat ficam ocultos.
- Com o agente CYOA ativado, escolher uma das opções dele orienta o próximo trecho nessa direção, como uma orientação. A escolha nunca vira uma mensagem sua, por isso o botão de Impersonate nas escolhas fica oculto. Com **Add CYOA choices to the message box instead of sending them** (adicionar as escolhas CYOA à caixa de mensagem em vez de enviá-las) ativado, a escolha vai para a barra de mensagem, onde você pode combiná-la com a sua própria orientação.
- Para escrever um trecho de novo, use gerar de novo (**Regenerate**, regenerar) nas ações dele. As suas edições são salvas antes. Com **Guide swipes/regens with chat input** (guiar swipes e novas gerações com a caixa de mensagem) ativado em **Settings** (Configurações) e texto na barra de mensagem, o botão mostra **Regenerate (guided)** e leva a nova versão em direção a esse texto, como **Send** faz. Quando um trecho tem mais de uma versão, setas embaixo dele alternam entre elas, e qualquer edição que você estava digitando é salva na versão em que você a digitou.
- Enquanto a IA escreve, **Send** vira **Stop** (parar).

## Como a IA é instruída a escrever um romance

O **Marinara's Novel Preset** é um preset integrado escrito para romances. Ele diz à IA que ela está escrevendo um único manuscrito junto com você, que ela escreve todos os personagens, inclusive o seu protagonista, e que ela escreve prosa de livro: parágrafos, falas entre aspas, *itálico* só para pensamentos e ênfase, e nenhum outro markdown. Cada trecho continua de onde a página termina e para em uma pausa natural, nunca em uma pergunta para você. Ela segue a orientação que você digita na barra de mensagem sem citá-la nem escrever notas sobre ela no trecho.

Quem é o protagonista depende de como você configura o romance:

| Configuração | Protagonista | Elenco |
| --- | --- | --- |
| Nenhuma persona e nenhum personagem | O protagonista que o manuscrito já acompanha. Em uma página vazia, a IA cria um, com nome, voz e algo que ele deseja, e o mantém coerente. | Nenhum elenco preparado. A IA apresenta personagens conforme a história precisa deles. |
| Uma persona e personagens | A sua persona. O perfil dela faz parte da bíblia da história. | Os seus personagens, cada um fiel ao seu card. |
| Personagens, mas nenhuma persona | O protagonista que o manuscrito já acompanha. Se não houver, com um personagem, esse personagem, a menos que o card dele descreva outra pessoa; nesse caso, a IA cria essa pessoa. Com vários, a IA escolhe um deles, ou um personagem novo se os cards apontarem para outra pessoa. | Os seus personagens. |
| Uma persona, mas nenhum personagem | A sua persona. | Nenhum elenco preparado. |

Uma persona conta quando tem uma descrição ou outro texto. Uma persona só com nome conta como nenhuma persona, já que a IA nunca vê o nome dela. Sem persona, um card que menciona `{{user}}` é lido como "User"; por isso, cards escritos para um romance sem persona funcionam melhor quando dão nome ao protagonista ou não mencionam `{{user}}`.

O preset faz algumas perguntas quando você começa o romance: a classificação do conteúdo (**NSFW** ou **SFW**), o ponto de vista (terceira, primeira ou segunda pessoa), o estilo de narração (próximo ao protagonista, alternando entre personagens de ponto de vista nas mudanças de cena, ou onisciente), o tempo verbal, o tamanho do trecho (**Length**, tamanho) e o idioma. A primeira opção de cada uma é o padrão.

Assim como o Marinara's Universal Preset, o preset Novel é somente leitura e não pode ser excluído. Abra-o em **Presets** e crie uma cópia editável para mudar o texto dele. Ele usa as suas configurações de geração da conexão e do chat em vez de configurações próprias. Veja [Editor de presets e gerenciador de prompts](../prompts/presets.md).

Algumas coisas para saber:

- Em chats de Roleplay, uma conexão com a sua própria substituição de preset usa esse preset no lugar, inclusive em romances.
- Mudar um romance depois para Visual Novel ou Classic com o botão **Visual Novel display** (exibição de Visual Novel) em **Settings > Appearance** (Configurações > aparência) mantém o preset Novel. Escolha outro preset em **Chat Settings** se você não quiser mais que a IA escreva o seu protagonista. O botão também muda o seu estilo de exibição padrão para chats de Roleplay sem um estilo salvo, não só o romance aberto.
- Outro preset também funciona em um romance, mas a maioria dos presets de roleplay diz à IA para nunca escrever o seu personagem. O Marinara's Universal Preset faz isso, então, com ele, a IA deixa o seu protagonista com você.

## Ouvir a história

Quando o texto para fala está ativado, as ações de cada trecho incluem **Speak**. Com **Only read dialogues** (ler só os diálogos) desativado, a narração também é lida, com a voz do narrador quando **Use separate narrator voice** (usar uma voz de narrador separada) está ativado. Com **Only read dialogues** ativado, só as falas entre aspas são lidas.
