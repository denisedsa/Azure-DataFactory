# 🚀 Projeto: Github e Azure Devops para Versionamento e Backup com Azure DevOps

Este repositório foi criado como parte do desafio **"GitHub e Azure DevOps para Versionamento e Backups"** da [DIO](https://www.dio.me/). Aqui você encontrará a aplicação prática dos conhecimentos sobre **Git, Azure Repos e Azure Pipelines**, simulando um fluxo real de desenvolvimento com controle de versão e automação.

---

## 🎯 Objetivos

* Criar um repositório versionado com Git
* Usar o Azure DevOps como plataforma de versionamento e integração contínua
* Simular um fluxo de desenvolvimento com criação de branches e Pull Requests
* Automatizar tarefas com pipeline (CI)
* Registrar e documentar todo o processo como parte de um portfólio técnico

---

## 🛠️ Tecnologias e Ferramentas

* Git
* Azure DevOps (Repos e Pipelines)
* Visual Studio Code
* Terminal / Git Bash
* Linguagem usada: HTML (exemplo base)

---

## 📂 Estrutura Inicial

```
projeto-versionamento/
├── index.html
└── README.md
```

---

## 📌 Etapas da Atividade

### ✅ 1. Criar o projeto no Azure DevOps

* Acesse: [https://dev.azure.com](https://dev.azure.com)
* Crie um novo projeto com repositório Git

### ✅ 2. Clonar o repositório localmente

```bash
git clone https://dev.azure.com/SEU_USUARIO/projeto-versionamento/_git/projeto-versionamento
cd projeto-versionamento
```

### ✅ 3. Adicionar arquivos e versionar

```bash
echo "<h1>Projeto com Azure DevOps</h1>" > index.html
git add .
git commit -m "Adiciona arquivo HTML base"
git push origin main
```

### ✅ 4. Criar branch de desenvolvimento

```bash
git checkout -b dev
echo "<p>Alteração feita na branch dev.</p>" >> index.html
git add .
git commit -m "Adiciona parágrafo na branch dev"
git push origin dev
```

### ✅ 5. Criar Pull Request via Azure DevOps

* Acesse **Repos > Branches**
* Clique em `dev > New Pull Request`
* Faça o merge para a `main`

### ✅ 6. Criar Azure Pipeline (CI)

* Acesse **Pipelines > Create Pipeline**
* Escolha o repositório
* Use a configuração YAML abaixo:

```yaml
trigger:
- main

pool:
  vmImage: 'ubuntu-latest'

steps:
- script: echo "Pipeline executado com sucesso!"
  displayName: 'Executar Script de Teste'
```

### ✅ 7. Validar execução do pipeline

* Após merge na `main`, o pipeline será executado automaticamente
* O log da execução ficará disponível na aba **Pipelines**

---

## 📸 Prints do Processo

> ✅ **Inclua prints como estes no seu repositório:**

1. Tela do Azure DevOps com o repositório criado
2. Terminal com commits realizados
3. Pull Request criada e mergeada
4. Pipeline rodando automaticamente
5. Resultado do pipeline com sucesso

Você pode colocar esses prints em uma pasta `./prints` e linkar aqui com Markdown:

```markdown
![Tela do Repositório](./prints/repositorio.png)
![Pipeline Executado](./prints/pipeline.png)
```

---

## 💭 Insights e Aprendizados

* Aprendi a estruturar um fluxo básico de versionamento usando Azure DevOps
* Reforcei a importância de boas práticas com Git (commits, branches e PRs)
* Compreendi como pipelines automatizados podem melhorar a entrega contínua (CI)
* Entendi como o Azure DevOps pode ser uma alternativa robusta ao GitHub

---

## 🌱 Possibilidades de Evolução

* Configurar deploy automático (CD) com Azure Web App ou GitHub Pages
* Integrar testes automatizados no pipeline
* Trabalhar com múltiplos ambientes (dev/stage/prod)
* Espelhar repositório no GitHub como backup adicional

---

## 🧪 Como Executar o Projeto Localmente

```bash
git clone https://dev.azure.com/SEU_USUARIO/projeto-versionamento/_git/projeto-versionamento
cd projeto-versionamento
code .
```

📌 Aprendizados

Este projeto me ajudou a entender na prática como aplicar versionamento e automações no ciclo de desenvolvimento. Aprendi a importância de manter um histórico limpo, trabalhar com branches e garantir a segurança dos dados com backups automatizados.

```

•	💼 https://www.linkedin.com/in/denise-almeida-6192a428/
