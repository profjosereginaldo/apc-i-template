---
name: "Prática 02"
about: "Template para criar a issue da pratica02"
title: "[Prática 02] – Saída de Dados em C"
labels: ["pratica02"]
assignees: ''
---

## 🎯 Objetivo
Nesta prática, você irá:
- Dominar a função de saída `printf()`;
- Aprender a formatar números inteiros e decimais (casas decimais e alinhamento);
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
2. Crie uma nova pasta chamada `pratica02`.
3. Dentro dela, desenvolva os arquivos solicitados (cada arquivo é um programa independente com sua própria `main()`):

- **`imprima_caracteres.c`**: Imprimir o caractere `A`, uma quebra de linha `\n` e o texto `Isso aqui eh uma string`.
- **`imprima_inteiros.c`**: Imprimir os números `10`, `-5` e `00004`.
- **`imprima_decimais.c`**: Imprimir o número `3.1415926` com todas as casas e também com apenas duas casas.
- **`imprima_formatado.c`**: Imprimir um cupom fiscal conforme layout abaixo:
  ```text
  ==============================
        N O T A    L E G A L
  ==============================
  Produto         Qtd Valor Unit
  Camiseta        002      39.99
  Calca           001      89.90
  Meia Social     003      19.99
  ==============================
  Total                   229.85
  ```

### 3️⃣ Compilação e execução local
1. No terminal, acesse a pasta da prática:
   ```bash
   cd praticas/pratica02
   ```
2. Compile e execute cada programa individualmente:
   ```bash
   gcc imprima_caracteres.c -o imprima_caracteres
   ./imprima_caracteres          # Linux / macOS
   imprima_caracteres.exe        # Windows
   ```
   ```bash
   gcc imprima_inteiros.c -o imprima_inteiros
   ./imprima_inteiros
   ```
   ```bash
   gcc imprima_decimais.c -o imprima_decimais
   ./imprima_decimais
   ```
   ```bash
   gcc imprima_formatado.c -o imprima_formatado
   ./imprima_formatado
   ```

### 4️⃣ Enviar para o GitHub
1. Volte para a pasta raiz do repositório:
   ```bash
   cd ../..
   ```
2. Adicione os arquivos, grave as alterações e envie:
   ```bash
   git add .
   git commit -m "feat: conclui pratica02. Fixes #ID"
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
└── pratica02/
    ├── imprima_caracteres.c
    ├── imprima_decimais.c
    ├── imprima_formatado.c
    └── imprima_inteiros.c
```

## ✅ Critérios de Conclusão
- [ ] Pasta `praticas/pratica02/` criada com os 4 arquivos `.c`.
- [ ] Todos os programas compilam e executam corretamente na máquina local.
- [ ] Código enviado para o GitHub com `git push origin main`.
- [ ] GitHub Actions exibiu o check verde (✅) para todos os arquivos.
- [ ] Issue fechada automaticamente pelo commit (aparece `closed` na aba Issues).
