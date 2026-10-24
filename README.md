# 🎮 Jogo da Adivinhação (Número Secreto)

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
</p>

<p align="center">
  <img src="https://img.shields.io/github/last-commit/LucKsz001/Jogo-da-Advinhajs?style=flat-square" alt="Último commit">
  <img src="https://img.shields.io/github/languages/count/LucKsz001/Jogo-da-Advinhajs?style=flat-square" alt="Linguagens">
  <img src="https://img.shields.io/github/repo-size/LucKsz001/Jogo-da-Advinhajs?style=flat-square" alt="Tamanho do repositório">
</p>

<p align="center">
  Um jogo web simples, divertido e didático onde o jogador precisa descobrir o número secreto gerado aleatoriamente pelo sistema.
</p>

---

## 📖 Índice

- [Sobre o projeto](#-sobre-o-projeto)
- [Funcionalidades](#-funcionalidades)
- [Tecnologias utilizadas](#-tecnologias-utilizadas)
- [Pré-requisitos](#-pré-requisitos)
- [Instalação](#-instalação)
- [Como jogar](#-como-jogar)
- [Estrutura do projeto](#-estrutura-do-projeto)
- [Funcionamento do código](#-funcionamento-do-código)
- [Personalização](#-personalização)
- [Possíveis melhorias](#-possíveis-melhorias)
- [Contribuição](#-contribuição)
- [Boas práticas](#-boas-práticas)
- [FAQ](#-faq)
- [Autor](#-autor)
- [Agradecimentos](#-agradecimentos)

---

## 📌 Sobre o projeto

O **Jogo da Adivinhação** (também conhecido como *Jogo do Número Secreto*) é uma aplicação web que sorteia um número aleatório e desafia o jogador a descobri-lo por meio de tentativas. A cada chute, o sistema informa se o número secreto é **maior** ou **menor** que o valor digitado, até que o jogador acerte.

O projeto foi desenvolvido com **HTML, CSS e JavaScript puro** (Vanilla JS), sem qualquer dependência externa ou framework, tornando-o ideal para:

- 🎓 **Estudos** de lógica de programação;
- 🧠 **Prática** de manipulação do DOM;
- 🎨 **Aprendizado** de estilização com CSS moderno;
- 💼 **Portfólio** de projetos iniciantes em desenvolvimento web.

A interface é estilizada com fundo em gradiente, imagens de apoio e layout responsivo, proporcionando uma experiência agradável tanto em desktops quanto em dispositivos móveis.

---

## ✨ Funcionalidades

- ✅ **Geração de número aleatório** — O sistema sorteia um número secreto no início de cada partida.
- ✅ **Dicas inteligentes** — A cada tentativa, o jogo informa se o número secreto é **maior** ou **menor** que o chute.
- ✅ **Contador de tentativas** — Ao acertar, o jogador recebe uma mensagem com o número total de tentativas.
- ✅ **Botão "Novo Jogo"** — Permite reiniciar a partida a qualquer momento.
- ✅ **Validação de entrada** — Impede chutes vazios, valores inválidos ou repetidos.
- ✅ **Feedback visual** — Mensagens dinâmicas exibidas na tela para orientar o jogador.
- ✅ **Layout responsivo** — Interface adaptável a diferentes tamanhos de tela.
- ✅ **Sem dependências externas** — Executado diretamente no navegador, sem instalação.

---

## 🛠️ Tecnologias utilizadas

| Tecnologia | Descrição |
|------------|-----------|
| **HTML5** | Estruturação semântica da página |
| **CSS3** | Estilização, gradientes, animações e responsividade |
| **JavaScript (ES6+)** | Lógica do jogo, manipulação do DOM e sorteio de números |

O projeto **não utiliza frameworks, bibliotecas ou ferramentas de build**, sendo executado diretamente no navegador ao abrir o arquivo `index.html`.

---

## 📋 Pré-requisitos

Para rodar o projeto, você só precisa de:

- Um **navegador web moderno** (Chrome, Firefox, Edge, Safari ou Opera);
- (Opcional) Um **editor de código** para visualizar/editar os arquivos (VS Code, Sublime Text, etc.);
- (Opcional) O **Git** instalado, caso queira clonar o repositório.

Nenhuma instalação de Node.js, npm, ou similares é necessária.

---

## 🚀 Instalação

### Opção 1 — Clonar via Git (recomendado)

```bash
# Clone o repositório
git clone https://github.com/LucKsz001/Jogo-da-Advinhajs.git

# Entre na pasta do projeto
cd Jogo-da-Advinhajs
```

Depois, basta abrir o arquivo `index.html` no navegador.

### Opção 2 — Download direto

1. Acesse o repositório no GitHub.
2. Clique em **Code** → **Download ZIP**.
3. Extraia o arquivo `.zip` em uma pasta de sua preferência.
4. Abra o arquivo `index.html` no navegador.

### Opção 3 — Servidor local (opcional)

Caso deseje servir o projeto com um servidor local (útil para evitar problemas com CORS ou `file://`):

```bash
# Com Python 3
python -m http.server 8000

# Com Node.js (via npx)
npx http-server

# Com VS Code
# Instale a extensão "Live Server" e clique em "Go Live"
```

Depois, acesse `http://localhost:8000` no navegador.

---

## 🎮 Como jogar

1. **Abra o jogo** no navegador (`index.html`).
2. **Digite um número** no campo de entrada.
3. **Clique em "Chutar"** (ou pressione `Enter`).
4. **Siga as dicas** exibidas na tela:
   - 🔼 **"O número secreto é maior"** → tente um número mais alto.
   - 🔽 **"O número secreto é menor"** → tente um número mais baixo.
5. **Acerte o número** para receber a mensagem de vitória com o total de tentativas.
6. **Clique em "Novo jogo"** para reiniciar a partida.

> 🎯 **Dica:** Tente usar a estratégia da **busca binária** para acertar no menor número de tentativas possível!

---

## 📁 Estrutura do projeto

```text
Jogo-da-Advinhajs/
│
├── img/                     # Imagens utilizadas no layout
│   ├── (background)         # Imagem de fundo do jogo
│   ├── (ruído/textura)      # Texturas aplicadas via CSS
│   └── ...
│
├── app.js                   # Lógica principal do jogo
├── index.html               # Estrutura da página
├── style.css                # Estilização e responsividade
└── README.md                # Documentação do projeto
```

---

## ⚙️ Funcionamento do código

O jogo é dividido em três arquivos principais:

### `index.html`
- Contém a estrutura da página: título, campo de entrada, botão "Chutar", botão "Novo jogo" e a área de mensagens.
- Vincula os arquivos de estilo (`style.css`) e script (`app.js`).

### `style.css`
- Define o visual do jogo: gradiente de fundo, tipografia, cores, espaçamentos e estados (hover, focus, disabled).
- Aplica **media queries** para adaptar a interface a telas menores.

### `app.js`
- **`gerarNumeroAleatorio()`** — Sorteia um número inteiro aleatório dentro de um intervalo definido.
- **`verificaChute()`** — Compara o chute do jogador com o número secreto e retorna as dicas.
- **`exibirTextoNaTela()`** — Função utilitária para atualizar textos no DOM.
- **`limparCampo()`** — Reseta o campo de entrada após cada chute.
- **`reiniciarJogo()`** — Reinicia a partida, sorteando um novo número secreto.

O estado do jogo é controlado por variáveis globais simples, como `numeroSecreto`, `tentativas` e `listaDeNumerosSorteados`.

---

## 🎨 Personalização

Quer adaptar o jogo para o seu gosto? Aqui vão algumas ideias:

### Alterar o intervalo de números

No arquivo `app.js`, procure a função `gerarNumeroAleatorio`:

```javascript
function gerarNumeroAleatorio() {
  const numeroEscolhido = parseInt(Math.random() * 10 + 1); // 1 a 10
  return numeroEscolhido;
}
```

Altere os valores `10` (intervalo) e `1` (mínimo) conforme desejado.

### Alterar o limite de tentativas

Caso queira adicionar um limite máximo, crie uma constante:

```javascript
const MAX_TENTATIVAS = 5;
```

E verifique dentro do fluxo do jogo se `tentativas >= MAX_TENTATIVAS`.

### Alterar as cores e o visual

No arquivo `style.css`, edite as variáveis ou os valores diretamente:

```css
:root {
  --cor-primaria: #4CAF50;
  --cor-fundo: linear-gradient(135deg, #667eea, #764ba2);
  --cor-texto: #ffffff;
}
```

---

## 🔧 Possíveis melhorias

- [ ] Adicionar limite máximo de tentativas e modo "difícil".
- [ ] Implementar histórico de números já sorteados (evitar repetições).
- [ ] Criar placar de melhores resultados usando `localStorage`.
- [ ] Adicionar sons e animações de feedback (acerto/erro).
- [ ] Melhorar acessibilidade (ARIA, navegação por teclado, contraste).
- [ ] Adicionar tema claro/escuro.
- [ ] Criar versão em React ou Vue como estudo comparativo.
- [ ] Escrever testes unitários com Jest para as funções de lógica.

---

## 🤝 Contribuição

Contribuições são **muito bem-vindas**! Para contribuir:

1. Faça um **fork** do projeto.
2. Crie uma **branch** para sua feature:
   ```bash
   git checkout -b feature/minha-feature
   ```
3. Faça suas alterações e **commit**:
   ```bash
   git commit -m "feat: adiciona minha feature"
   ```
4. Faça **push** para sua branch:
   ```bash
   git push origin feature/minha-feature
   ```
5. Abra um **Pull Request** no repositório original.

### 📝 Padrão de commits (sugestão)

Utilize [Conventional Commits](https://www.conventionalcommits.org/pt-br/):

- `feat:` nova funcionalidade
- `fix:` correção de bug
- `docs:` documentação
- `style:` formatação/estilo
- `refactor:` refatoração
- `test:` testes
- `chore:` tarefas de manutenção

---

## 📚 Boas práticas

Este projeto segue (ou busca seguir) boas práticas de desenvolvimento web:

- ✅ **Semântica HTML** — Uso correto de tags como `<header>`, `<main>`, `<section>`.
- ✅ **Separação de responsabilidades** — HTML, CSS e JS em arquivos separados.
- ✅ **Nomenclatura clara** — Variáveis e funções com nomes descritivos.
- ✅ **Código comentado** — Trechos principais documentados.
- ✅ **Responsividade** — Media queries para diferentes tamanhos de tela.
- ✅ **Acessibilidade básica** — Campos com `label`, foco visível, mensagens claras.

---

## ❓ FAQ

**1. Preciso instalar algo para jogar?**
Não! Basta abrir o `index.html` no navegador.

**2. O jogo funciona em celular?**
Sim, o layout é responsivo e funciona em dispositivos móveis.

**3. Posso usar o código em projetos pessoais?**
O projeto é de código aberto e pode ser usado para fins de estudo. Para outros usos, entre em contato com o autor.

**4. Como altero o intervalo de números?**
Veja a seção [Personalização](#-personalização).

**5. O jogo salva meu progresso?**
Atualmente não. Essa é uma das [possíveis melhorias](#-possíveis-melhorias).

---

## 👤 Autor

Desenvolvido com 💙 por **Pedro Lucas (LucKsz001)**

- 🐙 GitHub: [@LucKsz001](https://github.com/LucKsz001)
- 💼 LinkedIn: [Pedro Lucas](https://www.linkedin.com/in/pedro-lucas-b66187349)
- 📧 Email: [pedrolucas19souza@gmail.com](mailto:pedrolucas19souza@gmail.com)

---

## 🙏 Agradecimentos

- A todos que contribuírem com o projeto;
- À comunidade **open source** por tornar o aprendizado acessível;
- A você, que está lendo este README — obrigado pelo interesse! 🚀

---

<p align="center">
  <i>Feito com dedicação e café ☕</i>
</p>

<p align="center">
  ⭐ <b>Se este projeto te ajudou de alguma forma, deixe uma estrela no repositório!</b> ⭐
</p>
