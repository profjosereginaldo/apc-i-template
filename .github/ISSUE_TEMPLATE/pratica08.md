---
name: "Prática 08"
about: "Template para criar a issue da pratica08"
title: "[Prática 08] – Manipulação de Vetores e Matrizes em C"
labels: ["pratica08"]
assignees: ''
---

## 🎯 Objetivo
Nesta prática, você irá:
- Declarar, inicializar e acessar elementos de vetores e matrizes em C;
- Percorrer e manipular vetores e matrizes utilizando estruturas de repetição;
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
2. Crie uma nova pasta chamada `pratica08`.
3. Dentro dela, desenvolva os arquivos solicitados (cada arquivo é um programa independente com sua própria `main()`):

- **`media_aritmetica.c`**: Ler n números inteiros e armazená-los em um vetor. Calcular e exibir a média aritmética dos números.
- **`localiza_numero.c`**: Ler 10 números inteiros e armazená-los em um vetor. Em seguida, ler um número adicional e localizar sua posição no vetor. Caso o número não seja encontrado, informar que ele não está no vetor.
- **`boletim.c`**: Ler as notas de uma turma de 10 alunos, sendo 2 notas por aluno. Calcular a média de cada aluno e exibir o boletim de notas.
- **`diagonal_principal.c`**: Ler uma matriz 3x3 e imprimir apenas os elementos da diagonal principal.

### 3️⃣ Compilação e execução local
1. No terminal, acesse a pasta da prática:
   ```bash
   cd praticas/pratica08
   ```
2. Compile e execute cada programa individualmente:
   ```bash
   gcc media_aritmetica.c -o media_aritmetica
   ./media_aritmetica          # Linux / macOS
   media_aritmetica.exe        # Windows
   ```
   ```bash
   gcc localiza_numero.c -o localiza_numero
   ./localiza_numero
   ```
   ```bash
   gcc boletim.c -o boletim
   ./boletim
   ```
   ```bash
   gcc diagonal_principal.c -o diagonal_principal
   ./diagonal_principal
   ```

### 4️⃣ Enviar para o GitHub
1. Volte para a pasta raiz do repositório:
   ```bash
   cd ../..
   ```
2. Adicione os arquivos, grave as alterações e envie:
   ```bash
   git add .
   git commit -m "feat: conclui pratica08. Fixes #ID"
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
└── pratica08/
    ├── boletim.c
    ├── diagonal_principal.c
    ├── localiza_numero.c
    └── media_aritmetica.c
```

## ✅ Critérios de Conclusão
- [ ] Pasta `praticas/pratica08/` criada com os 4 arquivos `.c`.
- [ ] Todos os programas compilam e executam corretamente na máquina local.
- [ ] Código enviado para o GitHub com `git push origin main`.
- [ ] GitHub Actions exibiu o check verde (✅) para todos os arquivos.
- [ ] Issue fechada automaticamente pelo commit (aparece `closed` na aba Issues).
