# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**# 🐍 Neon Snake — Jogo da Cobrinha

Um jogo inspirado no clássico **Snake**, desenvolvido com HTML5, CSS3 e JavaScript puro. O **Neon Snake** combina uma jogabilidade simples e desafiadora com um visual moderno, efeitos neon e controles responsivos para proporcionar uma experiência divertida diretamente no navegador. 🎮

## ✨ Funcionalidades

- 🎯 **Sistema de pontuação:** ganhe pontos ao coletar os itens de energia.
- 🏆 **Recorde salvo:** o jogo armazena a melhor pontuação no dispositivo.
- ⚡ **Velocidade progressiva:** a cobrinha fica mais rápida conforme você coleta os itens.
- ⏸️ **Pausar e continuar:** interrompa e retome a partida quando quiser.
- 🔄 **Reiniciar partida:** comece uma nova rodada a qualquer momento.
- 💥 **Efeitos visuais:** partículas, brilho neon, cores em gradiente e animações.
- 📱 **Controles responsivos:** interface adaptada para computadores e dispositivos móveis.
- 🖥️ **Execução no navegador:** não exige instalação de bibliotecas ou frameworks.
- ♿ **Acessibilidade básica:** botões identificados, foco visível no teclado e respeito à preferência por movimento reduzido.

## 🛠️ Tecnologias aplicadas

### 🌐 HTML5

Utilizado para estruturar a interface do jogo, incluindo:

- Cabeçalho e identificação do jogo.
- Painéis de pontuação, recorde e velocidade.
- Área de jogo com o elemento `canvas`.
- Botões para iniciar, pausar e reiniciar a partida.
- Controles direcionais para dispositivos móveis.

### 🎨 CSS3

Responsável pelo design e pela experiência visual da aplicação:

- Tema escuro com cores neon.
- Layout responsivo com Flexbox, Grid e media queries.
- Efeitos de brilho, sombras e gradientes.
- Transições e estados visuais dos botões.
- Adaptação da interface para telas menores.
- Suporte à preferência do usuário por movimento reduzido.

### ⚙️ JavaScript (Vanilla JS)

Implementa a lógica e a interatividade do jogo, sem depender de frameworks externos.

Principais recursos:

- Movimentação e crescimento da cobrinha.
- Geração aleatória dos itens de energia.
- Detecção de colisões com as paredes e com o próprio corpo.
- Cálculo da pontuação e atualização do recorde.
- Aumento progressivo da velocidade.
- Controle dos estados da partida: pronta, em andamento, pausada e encerrada.
- Animação do jogo com `requestAnimationFrame()`.
- Tratamento de eventos do teclado, dos botões e da tela.
- Armazenamento do recorde com `localStorage`.

### 🖌️ Canvas API

A API Canvas do HTML5 é utilizada para desenhar e atualizar os elementos gráficos do jogo.

Com ela, são renderizados:

- 🟩 A cobrinha, com cabeça destacada e corpo em gradiente.
- 🟡 Os itens de energia com efeito de brilho.
- 📐 A grade do tabuleiro.
- ✨ As partículas geradas durante os eventos do jogo.

### 💾 LocalStorage

Utilizado para salvar o recorde no próprio navegador, por meio da chave `neonSnakeBest`.

O valor permanece disponível no mesmo navegador e dispositivo, mesmo após atualizar ou fechar a página, desde que os dados locais não sejam apagados.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Na tela inicial, clique em **COMEÇAR PARTIDA**.
3. Controle a cobrinha para coletar os pontos de energia espalhados pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou botões |
|---|---|
| ⬆️ Mover para cima | `↑` ou `W` |
| ⬇️ Mover para baixo | `↓` ou `S` |
| ⬅️ Mover para a esquerda | `←` ou `A` |
| ➡️ Mover para a direita | `→` ou `D` |
| ⏸️ Pausar ou continuar | `Espaço` |
| ▶️ Iniciar ou continuar | `Enter` |
| 🔄 Reiniciar a partida | Botão **Reiniciar** |

**Em celulares e tablets:** utilize os botões direcionais exibidos abaixo do tabuleiro.

### 3. Objetivo do jogo

🍏 Colete os pontos de energia para aumentar sua pontuação e fazer a cobrinha crescer.

- Cada item coletado vale **1 ponto**.
- A cobrinha aumenta de tamanho a cada item coletado.
- A velocidade aumenta progressivamente conforme a pontuação sobe.
- A cada 5 pontos, o nível exibido na interface aumenta.
- O objetivo é conseguir a maior pontuação possível sem colidir com obstáculos.

### 4. Regras do jogo

⚠️ Para continuar jogando, siga estas regras:

- **Não bata nas paredes:** atingir os limites do tabuleiro encerra a partida.
- **Não colida com o próprio corpo:** se a cabeça atingir o corpo da cobrinha, ocorre o fim de jogo.
- **Planeje seus movimentos:** como a cobrinha cresce e fica mais rápida, é importante antecipar as mudanças de direção.
- **Evite movimentos opostos imediatos:** o jogo impede uma inversão direta de direção.
- **Continue tentando:** após o fim da partida, clique em **JOGAR NOVAMENTE** para começar outra rodada.

🏆 Se conseguir ocupar todas as posições disponíveis no tabuleiro, você vence a partida!

### 5. Pontuação, velocidade e recorde

Durante o jogo, três indicadores ficam disponíveis:

- 🎯 **Pontuação:** quantidade de itens coletados na partida atual.
- 🏆 **Recorde:** maior pontuação registrada no dispositivo.
- ⚡ **Velocidade e nível:** mostram a velocidade atual e o nível calculado a partir da pontuação.

A velocidade aumenta a cada três pontos, até atingir o limite máximo de velocidade definido na implementação.

## 🚀 Como executar o projeto

O jogo utiliza tecnologias nativas do navegador e não requer instalação de dependências.

1. Baixe ou copie o arquivo `index.html` para uma pasta do computador.
2. Abra a pasta e localize o arquivo.
3. Clique duas vezes em `index.html` ou abra-o diretamente no navegador.
4. Clique em **COMEÇAR PARTIDA** e divirta-se! 🎮

**Requisitos:** um navegador moderno com suporte a HTML5, CSS3, JavaScript, Canvas API e `localStorage`.

## 📁 Estrutura do projeto

O projeto está concentrado em um único arquivo HTML:

```text
neon-snake/
└── index.html
```

O arquivo contém:

- **HTML:** estrutura da interface.
- **CSS:** estilos, layout e responsividade.
- **JavaScript:** regras, controles, animações e pontuação.

Essa organização facilita a execução, a distribuição e a manutenção do jogo, especialmente em projetos de pequeno porte.

## 🎨 Identidade visual

O Neon Snake utiliza uma identidade visual inspirada nos jogos arcade:

- 🌑 Fundo escuro para destacar os elementos.
- 🟢 Tons de verde e menta com efeito neon.
- ✨ Brilhos e partículas para enriquecer a experiência.
- 🕹️ Tipografia monoespaçada que remete aos jogos clássicos.
- 📱 Interface adaptável para diferentes tamanhos de tela.

## 📚 Objetivo educacional

Este projeto demonstra a aplicação prática de conceitos fundamentais do desenvolvimento Front-End, como:

- Estruturação de páginas com HTML5.
- Estilização responsiva com CSS3.
- Manipulação do DOM com JavaScript.
- Desenho e animação com Canvas API.
- Gerenciamento de estados e eventos.
- Detecção de colisões e lógica de jogos.
- Persistência de dados no navegador.
- Desenvolvimento de interfaces interativas e responsivas.

## 👨‍💻 Considerações finais

O **Neon Snake** é um projeto leve, acessível e divertido que combina a nostalgia dos jogos arcade com recursos modernos de interface e animação.

Desenvolvido com tecnologias nativas da Web, é uma demonstração de como HTML5, CSS3 e JavaScript podem ser utilizados em conjunto para criar uma experiência interativa completa, sem a necessidade de frameworks ou dependências externas.

**🚀 Jogue, desafie seus limites e tente bater seu recorde! 🐍🏆**
