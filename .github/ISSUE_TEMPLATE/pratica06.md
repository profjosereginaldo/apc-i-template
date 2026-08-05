---
name: "Prática 06"
about: "Template para criar a issue da pratica06"
title: "[Prática 06] – Estruturas de Seleção em C"
labels: ["pratica06"]
assignees: ''
---

## 🎯 Objetivo
Nesta prática, você irá:
- Utilizar as estruturas `if`, `else` e `else if` para controle do fluxo de execução;
- Implementar estruturas de seleção múltipla com `switch`;
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
2. Crie uma nova pasta chamada `pratica06`.
3. Dentro dela, desenvolva os arquivos solicitados (cada arquivo é um programa independente com sua própria `main()`):

- **`par_impar.c`**: Ler um número inteiro e informar se ele é par ou ímpar.
- **`classificacao_idade.c`**: Ler a idade de uma pessoa e classificar como: criança (0–12 anos), adolescente (13–17 anos), adulto (18–64 anos) ou idoso (65+ anos).
- **`dia_da_semana.c`**: Ler um número correspondente ao dia da semana (1 a 7) e informar se é dia útil ou final de semana.
- **`menu_jogo.c`**: Exibir um menu de jogo com as opções: `1 - Novo jogo`, `2 - Continuar jogo`, `3 - Ver pontuação` e `4 - Sair`. Ler a opção escolhida e exibir a mensagem correspondente. Caso a opção seja inválida, informar o usuário.

### 3️⃣ Compilação e execução local
1. No terminal, acesse a pasta da prática:
   ```bash
   cd praticas/pratica06
   ```
2. Compile e execute cada programa individualmente:
   ```bash
   gcc par_impar.c -o par_impar
   ./par_impar          # Linux / macOS
   par_impar.exe        # Windows
   ```
   ```bash
   gcc classificacao_idade.c -o classificacao_idade
   ./classificacao_idade
   ```
   ```bash
   gcc dia_da_semana.c -o dia_da_semana
   ./dia_da_semana
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
   git commit -m "feat: conclui pratica06. Fixes #ID"
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
└── pratica06/
    ├── classificacao_idade.c
    ├── dia_da_semana.c
    ├── menu_jogo.c
    └── par_impar.c
```

## ✅ Critérios de Conclusão
- [ ] Pasta `praticas/pratica06/` criada com os 4 arquivos `.c`.
- [ ] Todos os programas compilam e executam corretamente na máquina local.
- [ ] Código enviado para o GitHub com `git push origin main`.
- [ ] GitHub Actions exibiu o check verde (✅) para todos os arquivos.
- [ ] Issue fechada automaticamente pelo commit (aparece `closed` na aba Issues).
