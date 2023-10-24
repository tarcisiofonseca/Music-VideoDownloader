# Simplest Video and Music Downloader
Como o nome sugere, esse é o baixador de músicas e vídeos mais simples que eu consegui pensar para usuários não experientes, o qual também poder ser usado em smartphones. O programa é capaz de baixar músicas ou vídeos de mais de 1.000 sites diferentes, já que usa a biblioteca [youtube-dl](https://github.com/ytdl-org/youtube-dl) para fazer o download. A lista completa dos sites suportados pode ser visualizada [aqui](https://ytdl-org.github.io/youtube-dl/supportedsites.html).

## Requisitos

Apenas uma conta Google. O script usa o ambiente do Google Colab para baixar os arquivos diretamente para o seu Google Drive, possibilitando que seja usado em smartphones sem root e sem a necessidade do [Termux](https://termux.dev/en/).

## Primeiros passos

1 - Baixe o arquivo chamado "Music_VideoDownloader.ipynb" <br>
2 - Acesse https://colab.research.google.com/ <br>
3 - Faça upload do arquivo (o Google talvez o chame de "notebook") <br>

## Como usar

Antes de executar o script, há três variáveis que você precisa configurar:

**output_ext** = Use o valor 0 para baixar apenas o áudio (.mp3) ou 1 caso deseje tanto áudio quanto vídeo (.mp4). <br><br>
**folder_name** = Insira o nome da pasta no Google Drive onde os arquivos baixados serão armazenados (escreva o nome entre aspas). Caso a pasta ainda não exista, ela será criada na hora. <br><br>
**videos_list** = Basta seguir o exemplo no código: coloque os links dos vídeos/músicas desejados entre aspas e separados por vírgula (exceto pelo último link). Virtualmente, não há limite para quantos arquivos você pode baixar de uma única vez (provavelmente o limite é o cache do próprio Google Colab). 

Você **pode** baixar playlists inteiras do Youtube, por exemplo, inserindo apenas o link da própria playlist, sem a necessidade de inserir os links das músicas um a um. <br><br>

Depois de fazer as configurações acima, basta selecionar a opção "Executar tudo" ou "Run All" (o atalho é CTRL + F9 se você estiver usando um computador) e conceder permissão de acesso ao seu Google Drive para que o script possa mover os arquivos do ambiente Colab para a sua conta pessoal.
