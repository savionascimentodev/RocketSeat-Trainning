# Boas práticas para escrever um HTML profissional

---

### DOCTYPE

- Não é um elemento HTML;
- Como seu documento será interpretado;

---

### Escrever títulos inteligentes

- Significativos;
- Palavras-chave (buscas);

---

### Aprenda a usar MetaTags

- Charset - Acentuações e caracteres especiais;
- Description - Duas linhas que vão aparecer;
- Viewport - Adaptar para outros dispositivos;

---

### Não use o atributo `STYLE`

- Separação de responsabilidades;
- Especificações X !Important;
- Código sujo;
- Arquivo Separado;

---

### Importação de CSS e JS'

- Estilos no `<head>`
  - Melhor performace de renderização da página;
- Scripts antes de fechar o `<body>`
  - Melhor performace de renderização;
  - Prevenção de erros;
  - Quer deixar no `<head>`? Use o atributo `defer`

---

### Tags Semânticas

- Nem tudo são divs:

  ```html
  <div class="section-card">
    <div class="title">Card Title</div>
    <div>This is some Card</div>
    <div>Thank you</div>
    <div onclick="handleClick()">Clique me</div>
  </div>
  ```

- Utilize as tags para melhor semântica:

```html
<section class="card">
  <h2>Card Title</h2>
  <p>This is some Card</p>
  <p>Thank you</p>
  <button onclick="handleClick()">Clique me</button>
</section>
```

---

### Use atributos de acessibilidade!

- Img: alt;
- Title;
- Aria;
- TabIndex - formulário;

---

### Escrita

- Letras minúsculas;
- Fechamento de tags
- Formatação e Limpeza de código;
  - Prettier

---

### Formulários

- FieldSet + legend;
- Label + input;

---

### Compress HTML

- Diminui o tamanho do arquivo;
- Automatizado Vs Manual;
  - Online tool
  - Gulp (or Webpack?)

---

### Validar o HTML

- Verificar os padrões;
- Alertas e erros;
- Lighthouse (DevTools);
- [Validator](https://validator.w3.org/)
