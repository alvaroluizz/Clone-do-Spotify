# Clone do Spotify

Este projeto é um clone do Spotify desenvolvido com HTML, CSS e JavaScript. Ele conta com uma API local baseada em JSON para buscar artistas dinamicamente, permitindo a pesquisa em tempo real no header.

# Estrutura do Projeto

O projeto está organizado da seguinte forma:

* api-artists/ -> Contém os dados da API em um arquivo JSON.  
* src/ -> Contém:
  * assets/ -> Imagens, ícones e fotos das playlists.
  * styles/ -> Contém os seguintes arquivos CSS:
    - main-content.css
    - media-queries.css
    - reset.css
    - sidebar-footer.css
    - vars.css
* index.html -> Página principal do projeto.
* script.js -> Código JavaScript responsável pela interatividade.

# Como Iniciar a API Local

Para que a API local funcione corretamente, siga os passos abaixo:

1. Certifique-se de ter o json-server instalado
   -> npm install -g json-server

2. Verifique a versão do json-server (deve ser no mínimo 0.17.4):
   -> json-server --version

3. Se a versão instalada for beta ou inferior, desinstale e reinstale:
   -> npm uninstall -g json-server
   -> npm install -g json-server@0.17.4

4. Inicie o servidor JSON na porta 3000
   -> json-server --watch api-artists/artists.json --port 3000

5. Acesse os dados da API
   - Todos os artistas: http://localhost:3000/artists
   - Buscar por nome (exemplo: "Michael"): http://localhost:3000/artists?name_like=Michael

Agora, a API local estará pronta para uso.
