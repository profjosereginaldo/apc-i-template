---
name: "Prática 09"
about: "Template para criar a issue da pratica09"
title: "[Prática 09] – Manipulação de Strings em C"
labels: ["pratica09"]
assignees: ''
---

## 🎯 Objetivo
Nesta prática, você irá:
- Declarar e inicializar strings em C;
- Utilizar funções da biblioteca `<string.h>` para manipulação de textos;
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
2. Crie uma nova pasta chamada `pratica09`.
3. Dentro dela, desenvolva os arquivos solicitados (cada arquivo é um programa independente com sua própria `main()`):

- **`concatenar_nome.c`**: Ler o primeiro nome e o último nome de uma pessoa. Concatenar os dois em uma única string e exibi-la na tela.
- **`ordenar_strings.c`**: Ler três strings do usuário e exibir as strings em ordem alfabética.
- **`verbo_ar.c`**: Ler um verbo digitado pelo usuário e verificar se ele termina com "ar".
- **`lista_de_palavras.c`**: Ler N palavras e armazená-las em um vetor de strings. Em seguida, imprimir todas as palavras lidas.

### 3️⃣ Compilação e execução local
1. No terminal, acesse a pasta da prática:
   ```bash
   cd praticas/pratica09
   ```
2. Compile e execute cada programa individualmente:
   ```bash
   gcc concatenar_nome.c -o concatenar_nome
   ./concatenar_nome          # Linux / macOS
   concatenar_nome.exe        # Windows
   ```
   ```bash
   gcc ordenar_strings.c -o ordenar_strings
   ./ordenar_strings
   ```
   ```bash
   gcc verbo_ar.c -o verbo_ar
   ./verbo_ar
   ```
   ```bash
   gcc lista_de_palavras.c -o lista_de_palavras
   ./lista_de_palavras
   ```

### 4️⃣ Enviar para o GitHub
1. Volte para a pasta raiz do repositório:
   ```bash
   cd ../..
   ```
2. Adicione os arquivos, grave as alterações e envie:
   ```bash
   git add .
   git commit -m "feat: conclui pratica09. Fixes #ID"
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
└── pratica09/
    ├── concatenar_nome.c
    ├── lista_de_palavras.c
    ├── ordenar_strings.c
    └── verbo_ar.c
```

## ✅ Critérios de Conclusão
- [ ] Pasta `praticas/pratica09/` criada com os 4 arquivos `.c`.
- [ ] Todos os programas compilam e executam corretamente na máquina local.
- [ ] Código enviado para o GitHub com `git push origin main`.
- [ ] GitHub Actions exibiu o check verde (✅) para todos os arquivos.
- [ ] Issue fechada automaticamente pelo commit (aparece `closed` na aba Issues).
