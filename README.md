# 🎓 APC-I: Algoritmos e Programação de Computadores I
Repositório destinado às aulas teóricas e às atividades práticas da disciplina.

## 🛠️ Ambiente de Desenvolvimento
Para acompanhar a disciplina, você precisará das seguintes ferramentas:
| Ferramenta | O que é? | Recomendação |
| :--- | :--- | :--- |
| Editor de código | Ambiente onde você escreverá seu código. | [Visual Studio Code](https://code.visualstudio.com/) | 
| Compilador | Responsável por transformar o código em programa. | **Windows:** [w64devkit](https://github.com/skeeto/w64devkit/releases) <br> **Linux/macOS:** gcc/clang (já incluso) |
| Versionador | Controla e registra o histórico de alterações do código. | [Git](https://git-scm.com/) |

## 📂 Estrutura de Pastas
Este repositório está organizado da seguinte forma:
- **aulas/**: Contém os códigos utilizados nas aulas teóricas.
- **praticas/**: Contém os códigos das atividades práticas.

## 🚀 Fluxo de Trabalho Acadêmico
As atividades seguem o fluxo de trabalho baseado no modelo [GitFlow](https://www.atlassian.com/br/git/tutorials/comparing-workflows/gitflow-workflow).

### 1. Configuração Inicial (realizar apenas uma vez)
Execute estes passos para preparar seu ambiente:
1. **Fork**: Clique no botão `Fork`, no topo da página, para criar uma cópia deste repositório na sua conta GitHub.
2. **Clone**: Faça o clone o *seu fork* para a sua máquina local:
```bash
git clone https://github.com/SEU_USUARIO/apc-i-SEMESTRE.git
```
3. **Identificação**: Certifique-se que seu **nome** e **email** estejam configurados no Git:
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
``` 

### 2. Entrega de Atividades (repetir para cada prática)
Para cada nova atividade, siga o fluxo abaixo:
1. **Crie uma Issue**: Acesse a aba `Issues` no GitHub e clique no botão `New issue` para criar a prática usando o template correspondente.
2. **Crie uma branch**: Acesse a branch `develop` e crie uma nova branch.
3. **Desenvolva e teste**: Implemente os arquivos na pasta da prática e realize os testes.
4. **Envie para o GitHub**: Salve suas alterações e envie para o *seu fork*
5. **Solicite a revisão**: Acesse o *seu fork* no GitHub e crie um `pull request` direcionando para a branch `develop` do repositório do professor. 
> ⚠️ **Atenção!**<br>
> Se o check ✅ não aparecer no Pull Request, há erros de compilação ou  sintaxe que precisam ser corrigidos.

### 3. Feedback e Avaliação
Os Pull Requests podem receber os seguintes status:
- `aceito`: Indica que a atividade foi validada com sucesso.
- `revisao`: Indica que a atividade está sendo revisada pelo professor.
- `ajustes`: Indica que há modificações necessárias (ver comentários no PR).
