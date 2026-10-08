# QA Automação Web — Selenium Java | PetLov

Projeto independente de portfólio em Qualidade de Software e Automação de Testes Web, desenvolvido com **Java, Selenium WebDriver, JUnit 5 e Selenide**, utilizando a aplicação PetLov.

## 🎯 Objetivo

Aplicar práticas de automação Web em um projeto de QA, cobrindo fluxos da aplicação e demonstrando:

- automação de testes funcionais;
- validações de formulários;
- testes de cenários positivos e negativos;
- reutilização de código;
- modelagem de massa de testes;
- uso de hooks;
- organização e manutenção da suíte de testes;
- registro de evidências das execuções.

## 🧪 Tecnologias e versões

| Tecnologia | Versão |
|---|---|
| Java / JDK | 21 |
| Selenium WebDriver | 4.49.0 |
| JUnit 5 | 5.14.4 |
| Selenide | 7.18.2 |
| Maven | Gerenciador de build |
| Maven Surefire | 3.2.5 |

## 📋 Pré-requisitos

Antes de executar o projeto, tenha instalado:

- JDK 21;
- Maven;
- Git;
- uma IDE compatível, como **Visual Studio Code** ou **IntelliJ IDEA**;
- navegador Google Chrome.

Verifique Java e Maven pelo terminal:

```bash
java -version
mvn -version
```

## ▶️ Como executar

### VS Code

1. Clone o repositório:

```bash
git clone https://github.com/MarianaCaetanoCosta/Qax_SeleniumJava_PetLov.git
```

2. Abra a pasta do projeto no VS Code.
3. Instale as extensões **Extension Pack for Java** e **Maven for Java**.
4. Aguarde o Maven carregar as dependências.
5. Execute os testes pela opção de execução dos testes do VS Code ou pelo terminal:

```bash
mvn test
```

### IntelliJ IDEA

1. Clone o repositório.
2. Abra a pasta do projeto ou o arquivo `pom.xml`.
3. Confirme o uso do **JDK 21** em `Project Structure`.
4. Aguarde o IntelliJ IDEA importar as dependências do Maven.
5. Execute os testes pela classe de teste ou pela janela **Maven > Lifecycle > test**.

Também é possível executar pelo terminal integrado:

```bash
mvn test
```

### Terminal / Maven

Na raiz do projeto, execute:

```bash
mvn test
```

O Maven compila o projeto, resolve as dependências e executa os testes configurados pelo JUnit 5/Surefire.

## 🧪 Testes e cobertura

A suíte contempla cenários relacionados ao cadastro da aplicação PetLov, incluindo:

- cadastro de ponto de doação;
- validações de formulário;
- validação de e-mail inválido;
- cadastro com dados de teste;
- validações de mensagens e resultados esperados.

A estrutura também demonstra **reuso de código, hooks, modelagem de massa de testes e utilização de Selenide** para otimizar a automação.

Para executar toda a suíte:

```bash
mvn test
```

Os resultados gerados pelo Maven ficam no diretório `target/surefire-reports` após a execução.

## 📁 Estrutura do projeto

```text
Qax_SeleniumJava_PetLov/
├── .github/
├── .vscode/
├── build/
├── src/
│   ├── main/
│   └── test/
├── .gitignore
├── pom.xml
└── README.md
```

- `src/main/`: código de apoio da aplicação/testes.
- `src/test/`: classes e recursos da automação.
- `.vscode/`: configurações auxiliares para desenvolvimento no VS Code.
- `pom.xml`: configuração do Maven e dependências do projeto.
- `target/`: arquivos gerados durante a execução; não faz parte do código-fonte necessário para reproduzir os testes.

## 📸 Evidências

### Cadastro de ponto de doação

![Cadastro Ponto de Doação](target/imagens/CadastroPontoDeDoacao.jpg)

### Formulário de cadastro

![Formulário de Cadastro](target/imagens/Cadastro.jpg)

### Cadastro concluído

![Cadastro Concluído](target/imagens/CadastroRealizadocomSucesso.jpg)

## 📌 Contexto

Projeto desenvolvido durante formação prática em automação de testes com Fernando Papito.

O repositório é mantido como **projeto independente do portfólio**, representando a experiência com automação Web utilizando Selenium e Java e complementando os demais projetos de QA da autora.
