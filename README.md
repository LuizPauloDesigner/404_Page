# Página 404 Customizada

Este repositório contém os arquivos para uma página de erro 404 customizada, que pode ser utilizada em websites para fornecer uma experiência mais amigável aos usuários quando uma página não é encontrada.

## Visão Geral

A página 404 é um elemento crucial para a usabilidade de qualquer website. Em vez de exibir uma mensagem de erro genérica do navegador, esta solução oferece uma página estilizada e informativa, com um design atraente e uma mensagem clara de que a página solicitada não está disponível.

## Tecnologias Utilizadas

* **HTML5**: Estrutura e conteúdo da página.
* **CSS3**: Estilização e design da página, incluindo responsividade.
* **Bootstrap**: Framework CSS para layout e componentes (utilizado via CDN).
* **Google Fonts**: Para a fonte 'Arvo', que contribui para o estilo visual.

## Como Usar

Para utilizar esta página 404 em seu projeto, siga os passos abaixo:

1.  **Clone o Repositório:**
    ```bash
    git clone [https://github.com/LuizPauloDesigner/404_Page.git](https://github.com/LuizPauloDesigner/404_Page.git)
    ```
2.  **Copie os Arquivos:**
    Copie os arquivos `index.html` e `styles.css` para o diretório raiz do seu projeto web ou para o local onde você gerencia suas páginas de erro.
3.  **Configure seu Servidor Web:**
    Para que a página 404 seja exibida automaticamente, você precisará configurar seu servidor web (Apache, Nginx, etc.) para redirecionar erros 404 para o arquivo `index.html`.

    * **Exemplo para Apache (.htaccess):**
        Crie ou edite o arquivo `.htaccess` no diretório raiz do seu site e adicione a seguinte linha:
        ```apache
        ErrorDocument 404 /index.html
        ```
    * **Exemplo para Nginx:**
        No bloco `server` do seu arquivo de configuração Nginx, adicione:
        ```nginx
        error_page 404 /index.html;
        location = /index.html {
            root /caminho/para/o/seu/projeto; # Substitua pelo caminho real
            internal;
        }
        ```
4.  **Personalize (Opcional):**
    * **Texto:** Edite o arquivo `index.html` para alterar as mensagens de texto (`Look like you're lost`, `the page you are looking for not available!`).
    * **Link "Go to Home":** Altere o atributo `href` do link `Go to Home` para a URL da sua página inicial.
    * **Estilo:** Modifique o arquivo `styles.css` para ajustar cores, fontes, tamanhos e outros elementos visuais conforme a identidade visual do seu site.
    * **Imagem de Fundo:** A imagem de fundo animada (`https://cdn.dribbble.com/users/285475/screenshots/2083086/dribbble_1.gif`) é carregada via URL. Você pode substituí-la por uma imagem local ou outra URL de sua preferência no `styles.css` (`.four_zero_four_bg`).

## Estrutura do Projeto

* `index.html`: Contém a estrutura HTML da página 404.
* `styles.css`: Contém as regras de estilo CSS para a página.

## Créditos e Propósito

Este projeto é uma **replicação para fins de estudo de frontend**, baseada em uma página 404 desenvolvida originalmente por **@coding.stella**. O objetivo desta replicação é aprimorar habilidades em HTML e CSS, além de entender a estrutura e estilização de interfaces web.

## Contribuição

Contribuições são bem-vindas! Se você tiver sugestões de melhoria ou encontrar algum problema, sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` (se você criar um) para mais detalhes.

---

Feito com ❤️ por Luiz Paulo Teixeira [LuizPauloDesigner]
