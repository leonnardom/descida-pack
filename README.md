# descida-pack

Resource pack do servidor Descida. Publico porque o Minecraft baixa o pack por URL direta
e nao manda credencial nenhuma.

O que tem dentro: uma fonte bitmap (`descida:logo`) com o logo do Zafriel em dois tamanhos,
usada no titulo da scoreboard e no cabecalho do tab.

| Glifo | Tamanho | Onde |
|---|---|---|
| `U+E000` | 48px | cabecalho do tab |
| `U+E001` | 16px | titulo da sidebar |

`pack_format` 84 (Minecraft 26.1), declarado com `supported_formats` ate 88 (26.2).

O servidor aponta pra uma URL **fixada no commit**, nao no branch. Raw do branch tem cache
de alguns minutos, e um pack atualizado com sha1 novo contra um arquivo velho em cache faz
o cliente recusar a entrada. URL por commit e imutavel e nunca descasa do sha1.
