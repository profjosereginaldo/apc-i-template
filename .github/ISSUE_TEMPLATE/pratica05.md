---
name: "Prática 05"
about: "Template para criar a issue da pratica05"
title: "[Prática 05] – Operadores Aritméticos e Expressões em C"
labels: ["pratica05"]
assignees: ''
---

## 🎯 Objetivo
Nesta prática, você irá:
- Realizar cálculos matemáticos utilizando operadores aritméticos (`+`, `-`, `*`, `/`, `%`);
- Entender a precedência de operadores e o uso de parênteses;
- Aplicar conceitos de incremento (`++`) e decremento (`--`);
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
2. Crie uma nova pasta chamada `pratica05`.
3. Dentro dela, desenvolva os arquivos solicitados (cada arquivo é um programa independente com sua própria `main()`):

- **`operadores_aritmeticos.c`**: Ler dois números reais fornecidos pelo usuário e exibir os resultados das quatro operações aritméticas básicas (adição, subtração, multiplicação e divisão).
- **`decompor_numero.c`**: Ler um número inteiro de quatro dígitos fornecido pelo usuário e exibir sua decomposição em milhares, centenas, dezenas e unidades.
- **`incremento_decremento.c`**: Ler um número inteiro e exibir os resultados das operações de incremento e decremento nas formas pré-fixada e pós-fixada.
- **`calcula_impostos.c`**: Definir constantes para as alíquotas de ICMS (17%), ISS (5%) e PIS (1,65%). Em seguida, ler o valor de um produto e calcular o valor de cada imposto individualmente, além do preço final, utilizando a fórmula: `(1+ICMS+ISS+PIS)×valor`.

### 3️⃣ Compilação e execução local
1. No terminal, acesse a pasta da prática:
   ```bash
   cd praticas/pratica05
   ```
2. Compile e execute cada programa individualmente:
   ```bash
   gcc operadores_aritmeticos.c -o operadores_aritmeticos
   ./operadores_aritmeticos          # Linux / macOS
   operadores_aritmeticos.exe        # Windows
   ```
   ```bash
   gcc decompor_numero.c -o decompor_numero
   ./decompor_numero
   ```
   ```bash
   gcc incremento_decremento.c -o incremento_decremento
   ./incremento_decremento
   ```
   ```bash
   gcc calcula_impostos.c -o calcula_impostos
   ./calcula_impostos
   ```

### 4️⃣ Enviar para o GitHub
1. Volte para a pasta raiz do repositório:
   ```bash
   cd ../..
   ```
2. Adicione os arquivos, grave as alterações e envie:
   ```bash
   git add .
   git commit -m "feat: conclui pratica05. Fixes #ID"
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
└── pratica05/
    ├── calcula_impostos.c
    ├── decompor_numero.c
    ├── incremento_decremento.c
    └── operadores_aritmeticos.c
```

## ✅ Critérios de Conclusão
- [ ] Pasta `praticas/pratica05/` criada com os 4 arquivos `.c`.
- [ ] Todos os programas compilam e executam corretamente na máquina local.
- [ ] Código enviado para o GitHub com `git push origin main`.
- [ ] GitHub Actions exibiu o check verde (✅) para todos os arquivos.
- [ ] Issue fechada automaticamente pelo commit (aparece `closed` na aba Issues).
