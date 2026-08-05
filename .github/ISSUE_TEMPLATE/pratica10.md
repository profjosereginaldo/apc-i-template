---
name: "Prática 10"
about: "Template para criar a issue da pratica10"
title: "[Prática 10] – Tipos Estruturados e Enumerações em C"
labels: ["pratica10"]
assignees: ''
---

## 🎯 Objetivo
Nesta prática, você irá:
- Criar tipos de dados personalizados utilizando `struct`;
- Declarar e inicializar variáveis baseadas em tipos estruturados;
- Definir e utilizar enumerações com `enum`;
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
2. Crie uma nova pasta chamada `pratica10`.
3. Dentro dela, desenvolva os arquivos solicitados (cada arquivo é um programa independente com sua própria `main()`):

- **`cadastro_pessoa.c`**: Criar uma estrutura Pessoa com campos: nome, idade, altura e sexo. Ler os dados de uma pessoa e exibi-los.
- **`lista_de_alunos.c`**: Criar uma estrutura Aluno com campos: nome e matrícula. Ler os dados de 5 alunos e exibir a lista completa.
- **`dia_da_semana.c`**: Criar uma enumeração DiaSemana com os dias da semana. Ler um número de 1 a 7 e exibir o dia correspondente.
- **`playlist.c`**: Criar uma enumeração GeneroMusical com valores POP, ROCK e MPB. Criar uma estrutura Musica com campos título, duração e gênero (do tipo GeneroMusical). Ler os dados de 5 músicas e exibir a playlist completa.

### 3️⃣ Compilação e execução local
1. No terminal, acesse a pasta da prática:
   ```bash
   cd praticas/pratica10
   ```
2. Compile e execute cada programa individualmente:
   ```bash
   gcc cadastro_pessoa.c -o cadastro_pessoa
   ./cadastro_pessoa          # Linux / macOS
   cadastro_pessoa.exe        # Windows
   ```
   ```bash
   gcc lista_de_alunos.c -o lista_de_alunos
   ./lista_de_alunos
   ```
   ```bash
   gcc dia_da_semana.c -o dia_da_semana
   ./dia_da_semana
   ```
   ```bash
   gcc playlist.c -o playlist
   ./playlist
   ```

### 4️⃣ Enviar para o GitHub
1. Volte para a pasta raiz do repositório:
   ```bash
   cd ../..
   ```
2. Adicione os arquivos, grave as alterações e envie:
   ```bash
   git add .
   git commit -m "feat: conclui pratica10. Fixes #ID"
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
└── pratica10/
    ├── cadastro_pessoa.c
    ├── dia_da_semana.c
    ├── lista_de_alunos.c
    └── playlist.c
```

## ✅ Critérios de Conclusão
- [ ] Pasta `praticas/pratica10/` criada com os 4 arquivos `.c`.
- [ ] Todos os programas compilam e executam corretamente na máquina local.
- [ ] Código enviado para o GitHub com `git push origin main`.
- [ ] GitHub Actions exibiu o check verde (✅) para todos os arquivos.
- [ ] Issue fechada automaticamente pelo commit (aparece `closed` na aba Issues).
