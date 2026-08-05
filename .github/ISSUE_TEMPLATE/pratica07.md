---
name: "Prática 07"
about: "Template para criar a issue da pratica07"
title: "[Prática 07] – Estruturas de Repetição em C"
labels: ["pratica07"]
assignees: ''
---

## 🎯 Objetivo
Nesta prática, você irá:
- Utilizar as estruturas `for`, `while` e `do while` para repetir instruções diversas vezes;
- Controlar a execução de laços com contadores e condições;
- Praticar o fluxo de versionamento: **Código → Commit → Push**.

## 📝 Instruções da Atividade

### 1️⃣ Preparação do ambiente
1. Abra o **Visual Studio Code** na pasta do seu repositório.
2. Abra um terminal e certifique-se de que está na branch `main`.
   ```bash
   git checkout main
   git pull origin main
   ```

### 2️⃣ Implementação do código
1. No painel esquerdo do VS Code, localize a pasta `praticas`.
2. Crie uma nova pasta chamada `pratica07`.
3. Dentro dela, desenvolva os arquivos solicitados (cada arquivo é um programa independente com sua própria `main()`):

- **`fatorial.c`**: Ler um número inteiro positivo e calcular o seu fatorial.
- **`multiplos_de_n.c`**: Ler um número inteiro N e imprimir seus múltiplos no intervalo de 1 a 100.
- **`validacao_nota.c`**: Ler uma nota do usuário até que o valor esteja entre 0 e 10. Exibir a nota válida lida.
- **`menu_jogo.c`**: Exibir um menu de jogo com as opções: `1 - Novo jogo`, `2 - Continuar jogo`, `3 - Ver pontuação` e `4 - Sair`. Ler a opção do usuário repetidamente até que seja escolhida a opção "Sair". Caso a opção seja inválida, informar o usuário.

### 3️⃣ Compilação e execução local
1. No terminal, acesse a pasta da prática:
   ```bash
   cd praticas/pratica07
   ```
2. Compile e execute cada programa individualmente:
   ```bash
   gcc fatorial.c -o fatorial
   ./fatorial          # Linux / macOS
   fatorial.exe        # Windows
   ```
   ```bash
   gcc multiplos_de_n.c -o multiplos_de_n
   ./multiplos_de_n
   ```
   ```bash
   gcc validacao_nota.c -o validacao_nota
   ./validacao_nota
   ```
   ```bash
   gcc menu_jogo.c -o menu_jogo
   ./menu_jogo
   ```

### 4️⃣ Enviar para o GitHub
1. Volte para a pasta raiz do repositório:
   ```bash
   cd ../..
   ```
2. Adicione os arquivos, grave as alterações e envie:
   ```bash
   git add .
   git commit -m "feat: conclui pratica07. Fixes #ID"
   git push origin main
   ```
   > Substitua `#ID` pelo número desta Issue (ex: `Fixes #3`).

### 5️⃣ Verificar a correção automática
1. No GitHub, acesse a aba **Actions** do seu repositório.
2. Clique no workflow do seu último commit.
3. Verifique o resultado:
   - ✅ **Verde:** Todos os arquivos compilaram com sucesso.
   - ❌ **Vermelho:** Houve erro de compilação em algum arquivo. Clique em **"Compilar arquivos .c"** para ver a mensagem de erro, corrija no VS Code e faça um novo `git push`.

## 📂 Estrutura Final
Seu repositório deve ficar assim:
```text
praticas/
└── pratica07/
    ├── fatorial.c
    ├── menu_jogo.c
    ├── multiplos_de_n.c
    └── validacao_nota.c
```

## ✅ Critérios de Conclusão
- [ ] Pasta `praticas/pratica07/` criada com os 4 arquivos `.c`.
- [ ] Todos os programas compilam e executam corretamente na máquina local.
- [ ] Código enviado para o GitHub com `git push origin main`.
- [ ] GitHub Actions exibiu o check verde (✅) para todos os arquivos.
- [ ] Issue fechada automaticamente pelo commit (aparece `closed` na aba Issues).
