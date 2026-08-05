---
name: "Prática 03"
about: "Template para criar a issue da pratica03"
title: "[Prática 03] – Declaração de Variáveis e Constantes em C"
labels: ["pratica03"]
assignees: ''
---

## 🎯 Objetivo
Nesta prática, você irá:
- Declarar e inicializar variáveis de diferentes tipos (`char`, `int`, `float` e `double`);
- Declarar constantes com `#define` e com o qualificador `const`;
- Compreender o tamanho de cada tipo de dado na memória;
- Utilizar modificadores de tipo (`short`, `long`, `long long`, `unsigned`);
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
2. Crie uma nova pasta chamada `pratica03`.
3. Dentro dela, desenvolva os arquivos solicitados (cada arquivo é um programa independente com sua própria `main()`):

- **`declara_variaveis.c`**: Declarar variáveis para armazenar a idade, o sexo (`M` ou `F`), a altura (ex.: `1.75f`) e o peso (ex.: `72.845`) de uma pessoa e, em seguida, imprimir todos esses valores utilizando os especificadores de formato corretos.
- **`declara_constantes.c`**: Definir a constante **PI** (`3.14159265`) utilizando `#define` e o número de **Euler** (`2.71828182`) utilizando `const`. Em seguida, imprimir os valores dessas constantes. Tente alterar o valor da constante declarada com `const` para observar o erro gerado pelo compilador.
- **`tamanho_tipos.c`**: Utilizar o operador `sizeof()` para imprimir o tamanho (em bytes) dos seguintes tipos: `char`, `short int`, `int`, `long int`, `long long int`, `float`, `double` e `long double`.
- **`tipos_especiais.c`**: Declarar variáveis para armazenar o número de países (`195`), o número de idiomas (`7100`), a população mundial (`8274065924L`) e a proporção áurea (`1.61803398874989484820L`) e, em seguida, imprimir esses valores utilizando os especificadores de formato corretos.

### 3️⃣ Compilação e execução local
1. No terminal, acesse a pasta da prática:
   ```bash
   cd praticas/pratica03
   ```
2. Compile e execute cada programa individualmente:
   ```bash
   gcc declara_variaveis.c -o declara_variaveis
   ./declara_variaveis          # Linux / macOS
   declara_variaveis.exe        # Windows
   ```
   ```bash
   gcc declara_constantes.c -o declara_constantes
   ./declara_constantes
   ```
   ```bash
   gcc tamanho_tipos.c -o tamanho_tipos
   ./tamanho_tipos
   ```
   ```bash
   gcc tipos_especiais.c -o tipos_especiais
   ./tipos_especiais
   ```

### 4️⃣ Enviar para o GitHub
1. Volte para a pasta raiz do repositório:
   ```bash
   cd ../..
   ```
2. Adicione os arquivos, grave as alterações e envie:
   ```bash
   git add .
   git commit -m "feat: conclui pratica03. Fixes #ID"
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
└── pratica03/
    ├── declara_constantes.c
    ├── declara_variaveis.c
    ├── tamanho_tipos.c
    └── tipos_especiais.c
```

## ✅ Critérios de Conclusão
- [ ] Pasta `praticas/pratica03/` criada com os 4 arquivos `.c`.
- [ ] Todos os programas compilam e executam corretamente na máquina local.
- [ ] Código enviado para o GitHub com `git push origin main`.
- [ ] GitHub Actions exibiu o check verde (✅) para todos os arquivos.
- [ ] Issue fechada automaticamente pelo commit (aparece `closed` na aba Issues).
