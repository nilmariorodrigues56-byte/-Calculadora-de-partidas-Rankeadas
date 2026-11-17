# 2️⃣ Calculadora de Partidas Rankeadas

Desafio de Projeto da DIO: criar uma função que calcula o saldo de partidas rankeadas (vitórias − derrotas) e classifica o herói em um nível de acordo com a quantidade de vitórias.

## 📜 Regras de classificação

| Vitórias        | Nível    |
| --------------- | -------- |
| Menor que 10    | Ferro    |
| Entre 11 e 20   | Bronze   |
| Entre 21 e 50   | Prata    |
| Entre 51 e 80   | Ouro     |
| Entre 81 e 90   | Diamante |
| Entre 91 e 100  | Lendário |
| Maior ou igual a 101 | Imortal |

> Observação: o enunciado não define explicitamente o caso de exatamente **10 vitórias**. Na implementação, 10 vitórias caem em **Bronze** (estrutura `if/else` encadeada, em que o primeiro `if` pecha apenas `< 10`). Se seu curso exigir outra regra para esse caso, basta ajustar a primeira condição.

## 🎯 Saída esperada

A mensagem exibida ao final deve seguir o formato:

```
O Herói tem de saldo de {saldoVitorias} está no nível de {nivel}
```

Exemplo com 60 vitórias e 20 derrotas (saldo = 40):

```
O Herói tem de saldo de 40 está no nível de Ouro
```

## 🧠 Conceitos utilizados

- Variáveis
- Operadores (subtração, comparação)
- Laços de repetição (`for...of` nos exemplos de teste)
- Estruturas de decisão (`if/else if/else`)
- Funções (`calcularRankeadas` e `exibirResultado`)

## ▶️ Como executar

Pré-requisito: [Node.js](https://nodejs.org/) instalado.

```bash
node index.js
```

O programa percorre uma lista de exemplos e imprime o resultado de cada um.

## 📂 Estrutura do projeto

```
calculadora-partidas-rankeadas/
├── index.js   # Código da solução (função + exemplos de teste)
└── README.md  # Este arquivo
```

## 🚀 Como subir este projeto no GitHub

### Opção A — Pelo terminal (Git)

1. Crie uma conta em <https://github.com> (caso ainda não tenha).
2. No GitHub, clique em **+** (canto superior direito) → **New repository**:
   - Nome sugerido: `calculadora-partidas-rankeadas`
   - Deixe **pública** (Public) e, para enviar arquivos locais, **não** marque "Add a README file".
   - Clique em **Create repository**.
3. Abra o terminal dentro da pasta do projeto e execute:

```bash
git init
git add .
git commit -m "Desafio Calculadora de Partidas Rankeadas - DIO"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/calculadora-partidas-rankeadas.git
git push -u origin main
```

4. Na primeira autenticação via terminal, o GitHub pode pedir login. Em vez da senha normal, use um **Personal Access Token** (Configurações → Developer settings → Personal access tokens), ou use o [GitHub CLI](https://cli.github.com/) (`gh auth login`) / o [GitHub Desktop](https://desktop.github.com/).

### Opção B — Pelo navegador (sem instalar o Git)

1. Crie o repositório vazio no GitHub (passos 1–2 da Opção A).
2. Na página do repositório, clique em **Add file** → **Upload files**.
3. Arraste os arquivos `index.js` e `README.md` e clique em **Commit changes**.

### Dica do enunciado

Se o expert da turma tiver um repositório público da solução de referência, use o botão **Fork** para criar sua cópia e enviar suas alterações mantendo a referência ao código original.
