<header>

<!--
  <<< Author notes: Course header >>>
  Read <https://skills.github.com/quickstart> for more information about how to build courses using this template.
  Include a 1280×640 image, course name in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Next to "About", add description & tags; disable releases, packages, & environments.
  Add your open source license, GitHub uses the MIT license.
-->

# Habilitando o Code Scanning para deixar seu código seguro

_Assegurar a segurança do código fonte das aplicações é um passo essencial no desenvolvimento de software moderno. Neste curso você ira aprender como usar o Github Code Scanning para identificar, resolver e previnir padrões inseguros de código._

</header>

<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
  TBD-step-1-notes.
-->

## Passo 1: Ativar o code scanning

👋 Olá! Bem-vindo ao curso Introdução ao Code Scanning!

Vamos começar!

Neste primeiro passo, vamos aprender mais sobre o CodeQL e como utilizá-lo para proteger o seu código fonte.

**O que é o code scanning do GitHub**: _[Code scanning](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/about-code-scanning)_ é uma funcionalidade que permite que equipes de desenvolvimento integrem ferramentas de teste de segurança no processo de desenvolvimento de software. Isso é feito por meio do GitHub Actions. Com o code scanning, você pode integrar diversos tipos de ferramentas, incluindo SAST, segurança para containers e infraestrutura como código.

**O que é SAST?**:
**SAST (Static Application Security Testing)** é uma abordagem para identificar vulnerabilidades de segurança no código fonte, analisando-o de forma estática em busca de padrões no código, ou seja, sem executá-lo. Essa técnica permite detectar problemas como falhas de injeção, validação inadequada de dados e outros riscos antes mesmo que o software seja executado.

**O que é o CodeQL**: _[CodeQL](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/about-code-scanning-with-codeql)_ é uma ferramenta de análise estática que ajuda a identificar vulnerabilidades de segurança, como injeção de SQL, cross-site scripting entre outros problemas de segurança que possam ser descobertos pelo padrão do código.

### :keyboard: Atividade: Ativar o code scanning default

Primeiro, vamos ativar o code scanning em nosso repositório.

1. Abra uma nova aba no navegador e execute os passos na segunda aba enquanto lê as instruções aqui.
2. Navegue até a aba **Settings** (Configurações) no topo do seu novo repositório.
3. No menu à esquerda, em **Security** (Segurança), selecione **Code security** (Segurança de código).
4. Role até a seção intitulada **Code scanning**. Para este curso, vamos focar na análise com CodeQL.
5. Clique no menu suspenso **Set up** (Configurar) e escolha **Default** (Padrão).

   ![enable-code-scanning-default.png](/images/enable-code-scanning-default.png)

Vamos dar uma olhada nas opções de configuração na janela modal:

- **Languages to analyze (Linguagens a serem analisadas):** Estas são as linguagens que serão escaneadas pelo CodeQL. Neste caso, vamos analisar em `Python`. *O CodeQL também suporte analises de Github Actions maliciosas, mas não vamos utilizar neste momento.*
- **Query suites (Pacotes de consultas):** As [consultas](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/about-code-scanning-with-codeql#about-codeql-queries) do CodeQL são agrupadas em pacotes chamados "suites". Esta seção permite escolher qual pacote utilizar. Vamos deixar definido como **Default** para este exercício. Para mais informações, consulte "[Sobre CodeQL queries](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/about-code-scanning-with-codeql#about-codeql-queries)".
- **Events (Eventos):** Esta seção define quando o CodeQL deve realizar a varredura. Neste caso, ele está configurado para escanear em qualquer pull request ou push para a branch `main`.

   ![codeql-default-configuration-box.png](/images/codeql-default-configuration-box.png)

6. Clique em **Enable CodeQL** (Ativar CodeQL).
7. Aguarde cerca de 20 segundos e, em seguida, atualize esta página (aquela de onde você está seguindo as instruções). O [GitHub Actions](https://docs.github.com/en/actions) atualizará automaticamente para o próximo passo.

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---
Precisa de ajuda?:
- [Manda para gente!](https://github.com/fguisso/introducao-ao-code-scanning/discussions)
- [Github Skills: Post in our discussion board](https://github.com/orgs/skills/discussions/categories/introduction-to-codeql) &bull; 

&copy; 2023 GitHub • [Código de Conduta](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) • [Licença MIT](https://gh.io/mit)

</footer>
