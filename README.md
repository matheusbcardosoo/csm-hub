# csm-hub

Hub de acessos do Colégio São Marcos, criado como uma aplicação estática em HTML e CSS.

## Estrutura do projeto

- `index.html`: ponto de entrada da aplicação.
- `assets/styles/index.css`: estilos globais da interface.
- `assets/images/`: imagens, ícones e logotipos utilizados na página.

## Requisitos

- Deploy via EasyPanel.
- Build com Nixpacks.
- Versão utilizada e operante: `Nixpacks 1.41.0`.

## Como publicar no EasyPanel

1. Crie um novo projeto no EasyPanel.
2. Dentro do projeto, crie um serviço do tipo aplicativo.
3. Cole o link do repositório Git.
4. Em caminho de build, informe `/`.
5. Confirme que a opção de build está usando Nixpacks.
6. Mantenha a versão `1.41.0` do Nixpacks, pois ela já está funcionando corretamente neste projeto.
7. Implemente o serviço e aguarde a finalização do processo.

## Atenção

**Manter o nome do arquivo `index.html` é essencial.** O Nginx só consegue mapear a aplicação corretamente quando esse arquivo existe no diretório raiz.

Se o nome do arquivo for alterado, o serviço pode subir sem entregar a aplicação corretamente.

## Observações

- A aplicação é totalmente estática.
- Não há etapa de build complexa ou dependências adicionais para instalar.
- Se forem feitas alterações de layout, preserve a estrutura principal e o arquivo de entrada na raiz do projeto.
