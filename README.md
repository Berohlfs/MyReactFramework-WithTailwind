# MyReactFramework-WithTailwind

Template pessoal para aplicações em React.js, utilizando `Vite.js` (toolchain) e Tailwind/Radix UI Themes (UI library)

[Acessar demo!](https://mrf-tailwind.bernardorohlfs.site/)

## Libs utilizadas

* `tailwindcss`, `postcss` e `autoprefixer` para estilização avançada.
* `@radix-ui/themes` como biblioteca UI.
* `@radix-ui/react-icons` para ícones.
* `postcss-import` para utilização de 'CSS imports'.
* `axios` para requisições HTTP.
* `next-themes` para manipulação de temas.
* `react-router-dom` para roteamento.
* `sonner` para notificações.
* `react-imask` para aplicação de máscaras de input.
* `zod` e `react-hook-form` para validação de formulário.
* `js-cookie` para gerenciamento de cookies.

## Extensões do VS Code recomendadas

* `Color Highlight`.
* `Material Icon Theme`.
* `Tailwind CSS Intellisense`.
* `Tailwind Docs`.
* `Tailwind Fold`.
  
## Arquivo `.htaccess`

Um arquivo `.htaccess` é necessário para que a aplicação funcione corretamente após ser hospedada. Adicione o arquivo à pasta da aplicação no servidor FTP, com o seguinte conteúdo:

```
<IfModule mod_rewrite.c>

  RewriteEngine On
  RewriteBase /
  RewriteRule ^index\.html$ - [L]
  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME} !-l
  RewriteRule . /index.html [L]

</IfModule>
```
