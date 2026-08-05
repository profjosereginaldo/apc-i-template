---
name: "Prática 04"
about: "Template para criar a issue da pratica04"
title: "[Prática 04] – Entrada de Dados em C"
labels: ["pratica04"]
assignees: ''
---

## 🎯 Objetivo
Nesta prática, você irá:
- Dominar a função de entrada `scanf()`;
- Aprender a ler caracteres, números inteiros e decimais;
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
2. Crie uma nova pasta chamada `pratica04`.
3. Dentro dela, desenvolva os arquivos solicitados (cada arquivo é um programa independente com sua própria `main()`):

- **`leia_caracteres.c`**: Ler um caractere digitado pelo usuário e imprimir o caractere informado e seu respectivo código na tabela **ASCII**.
- **`leia_inteiros.c`**: Ler dois números inteiros fornecidos pelo usuário e exibir os valores lidos.
- **`leia_decimais.c`**: Ler duas notas de um aluno fornecidas pelo usuário e exibir os valores lidos.
- **`leia_dados.c`**: Ler a idade, a altura (ex.: `1.75f`), o sexo (`M` ou `F`) e o peso (ex.: `72.825`) de uma pessoa e exibir todas as informações organizadas em formato de ficha cadastral.

### 3️⃣ Compilação e execução local
1. No terminal, acesse a pasta da prática:
   ```bash
   cd praticas/pratica04
   ```
2. Compile e execute cada programa individualmente:
   ```bash
   gcc leia_caracteres.c -o leia_caracteres
   ./leia_caracteres          # Linux / macOS
   leia_caracteres.exe        # Windows
   ```
   ```bash
   gcc leia_inteiros.c -o leia_inteiros
   ./leia_inteiros
   ```
   ```bash
   gcc leia_decimais.c -o leia_decimais
   ./leia_decimais
   ```
   ```bash
   gcc leia_dados.c -o leia_dados
   ./leia_dados
   ```

### 4️⃣ Enviar para o GitHub
1. Volte para a pasta raiz do repositório:
   ```bash
   cd ../..
   ```
2. Adicione os arquivos, grave as alterações e envie:
   ```bash
   git add .
   git commit -m "feat: conclui pratica04. Fixes #ID"
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
└── pratica04/
    ├── leia_caracteres.c
    ├── leia_dados.c
    ├── leia_decimais.c
    └── leia_inteiros.c
```

## ✅ Critérios de Conclusão
- [ ] Pasta `praticas/pratica04/` criada com os 4 arquivos `.c`.
- [ ] Todos os programas compilam e executam corretamente na máquina local.
- [ ] Código enviado para o GitHub com `git push origin main`.
- [ ] GitHub Actions exibiu o check verde (✅) para todos os arquivos.
- [ ] Issue fechada automaticamente pelo commit (aparece `closed` na aba Issues).
