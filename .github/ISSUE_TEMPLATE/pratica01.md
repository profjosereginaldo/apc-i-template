---
name: "Prática 01"
about: "Template para criar a issue da pratica01"
title: "[Prática 01] – Estrutura Básica de um Programa em C"
labels: ["pratica01"]
assignees: ''
---

## 🎯 Objetivo
Nesta prática, você irá:
- Criar, compilar e executar seu primeiro programa em C;
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
2. Crie uma nova pasta chamada `pratica01`.
3. Dentro dela, crie o arquivo `ola_mundo.c` com o seguinte código:
   ```c
   #include <stdio.h>

   int main() {
       printf("Olá, Mundo!");
       return 0;
   }
   ```

### 3️⃣ Compilação e execução local
1. No terminal, acesse a pasta da prática:
   ```bash
   cd praticas/pratica01
   ```
2. Compile e execute o programa:
   ```bash
   gcc ola_mundo.c -o ola_mundo
   ./ola_mundo          # Linux / macOS
   ola_mundo.exe        # Windows
   ```
   > Se aparecer `Olá, Mundo!`, seu código está correto.

### 4️⃣ Enviar para o GitHub
1. Volte para a pasta raiz do repositório:
   ```bash
   cd ../..
   ```
2. Adicione os arquivos, grave as alterações e envie:
   ```bash
   git add .
   git commit -m "feat: conclui pratica01. Fixes #ID"
   git push origin main
   ```
   > Substitua `#ID` pelo número desta Issue (ex: `Fixes #3`).

### 5️⃣ Verificar a correção automática
1. No GitHub, acesse a aba **Actions** do seu repositório.
2. Clique no workflow do seu último commit.
3. Verifique o resultado:
   - ✅ **Verde:** Seu código compilou com sucesso.
   - ❌ **Vermelho:** Houve erro de compilação. Clique em **"Compilar arquivos .c"** para ver a mensagem de erro, corrija no VS Code e faça um novo `git push`.

## 📂 Estrutura Final
Seu repositório deve ficar assim:
```text
praticas/
└── pratica01/
    └── ola_mundo.c
```

## ✅ Critérios de Conclusão
- [ ] Arquivo `praticas/pratica01/ola_mundo.c` criado e testado localmente.
- [ ] Código enviado para o GitHub com `git push origin main`.
- [ ] GitHub Actions exibiu o check verde (✅).
- [ ] Issue fechada automaticamente pelo commit (aparece `closed` na aba Issues).
