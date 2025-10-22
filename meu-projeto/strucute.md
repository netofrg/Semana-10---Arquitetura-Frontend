#  Estrutura de Pastas — Projeto Frontend
Este documento descreve a **organização das pastas e arquivos** do projeto **meu-projeto-frontend**, explicando a **função** e a **importância** de cada parte do sistema.

---

##  public/
Contém arquivos **públicos**, acessíveis diretamente pelo navegador.  
Esses arquivos **não passam por processamento** do bundler (Vite/Webpack).

- **index.html** → Documento base onde o React é injetado (ponto inicial da aplicação).  
- **favicon.ico** → Ícone exibido na aba do navegador.  

 *Importância:* mantém separado o conteúdo estático que o navegador precisa acessar diretamente.

---

##  src/
Pasta principal do **código-fonte** do aplicativo React.  
Aqui estão todos os componentes, páginas, estilos, serviços e utilitários do app.

###  assets/
Imagens, ícones, fontes e outros arquivos estáticos usados no app.  
Exemplo: `logo.png`, `background.jpg`.

 *Importância:* centraliza os recursos visuais, facilitando manutenção e organização.

---

###  components/
Componentes **reutilizáveis** de interface, como botões, cards, inputs, headers, etc.  
Exemplo: `Button.jsx`, `Header.jsx`.

 *Importância:* melhora a **reutilização** e a **consistência visual** do sistema.

---

###  pages/
Contém **páginas completas** do sistema (ex: Home, Login, Dashboard).  
Cada página importa componentes e lida com a lógica de tela.

 *Importância:* ajuda a separar a estrutura de navegação e as telas da aplicação.

---

###  services/
Centraliza a **comunicação com APIs** externas (via `fetch` ou `axios`).  
Exemplo: `api.js` (configuração base), `authService.js` (login, cadastro, etc).

 *Importância:* separa a lógica de requisições da interface, deixando o código mais limpo e testável.

---

###  hooks/
Contém **hooks personalizados do React**, como `useAuth`, `useFetch`, etc.  
São funções que reutilizam lógicas de estado e efeitos em diferentes componentes.

 *Importância:* evita repetição de lógica e torna o código mais modular.

---

###  styles/
Arquivos de **estilo global** (CSS, SCSS ou Tailwind).  
Exemplo: `globals.css` define estilos gerais e `theme.css` define variáveis de tema.

 *Importância:* mantém os estilos organizados e facilita o controle visual do projeto.

---

###  utils/
Funções **utilitárias** e auxiliares, como formatadores de datas ou validações.  
Exemplo: `formatDate.js`, `validations.js`.

 *Importância:* promove o reuso de funções simples em várias partes do sistema.

---

###  main.jsx
Ponto de entrada do React.  
Renderiza o componente principal dentro do elemento `#root` do `index.html`.

 *Importância:* é o **início da aplicação**, onde o React é inicializado.

---

##  Outros arquivos na raiz
- **package.json** → Lista as dependências, scripts e metadados do projeto.  
- **vite.config.js** → Configuração do Vite (servidor e build).  
- **.gitignore** → Define arquivos e pastas ignorados pelo Git (`node_modules/`, `.env`, etc).  
- **README.md** → Documentação geral do projeto (instalação, uso e descrição).  
- **structure/README.md** → Este arquivo, que explica a arquitetura das pastas.

---

##  Benefícios da Estrutura
- Organização clara e padronizada.  
- Facilita o trabalho em equipe.  
- Melhora a manutenção e evolução do código.  
- Evita duplicação e mistura de responsabilidades.


