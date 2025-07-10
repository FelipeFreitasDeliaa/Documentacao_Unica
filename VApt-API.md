# **Documentação VApt - API**

## **Sobre**
Esse arquivo servirá como um guia para ajudar a manter os projetos padronizados.

## **Padrão de Nomenclatura**

| Categoria | Padrão |  Regras  |
|-----------|--------|--------- |
| **Variáveis** | `camelCase` | Primeiro nome inicia com letra minúscula, os seguintes com maiúscula sem separação o por espaços (ex: `variavelExemplo`, `camelCase`). |
| **Funções/Métodos** | `camelCase` | Mesmo padrão de variáveis (`variavelExemplo`, `camelCase`). |
| **Arquivos** | `CamelCase` |
Arquivos CamelCase Primeiro nome inicia em letra minúscula, os seguintes se iniciam com letra maiúscula sem separação sem separação por espaços (ex: `variableExample`, `camelCase`) |
| **Colunas**  | `SnakeCase` | Todo nome em minúsculo e separaçao por underline (ex: `coluna_exemplo`, `snake_case`) |
| **Idioma** | Inglês | -  |

## **Organização de Pastas**


| Categoria    | Padrão     | Observações |
|--------------|------------|-------------|
| Nomenclatura | Snake Case | Primeiro nome inicia em letra minúscula, os seguintes se iniciam com letra maiúscula sem separação sem separação por espaços (ex: `variableExample`, `camelCase`) |
| Idioma | Inglês | - |
---
```plaintext
raiz/
├── /dist                    
├── /prisma                 → Armazenar arquivos necessários para configuração do prisma
│   └── /migrations         → Armazena histórico de alterações no banco
├── /scripts                → Armazena scripts para o banco de dados
├── /src                    → Código principal para o uso da API, requisições, etc.
├── /test                   → Arquivos de teste da API
```

## **Padrão do Código**

|  Categoria | Diretriz  | Descrição |   
|------------|-----------|-----------|
| Escrita      | Inglês  | -         | 
| Comentários  | -       | Arquivos com nomes bem definidos, facilitando o entendimento do que o código faz | 

**Identação**:<br>
**Funções** -> Quebra de linha para o método<br>
Dentro do método inserir dois espaços e quebras de linhas para cada linha de código.<br>
Para condicionais, laços de repetições ou chamar outros métodos repita o padrão anterior.<br>
Abrir e fechar blocos no mesmo nivel de identação.

**SQL** -> Quebra de linha para tabelas.
dentro da classe inserir dois espaços ou um tab para cada coluna, quebras de linhas para separação.<br>
Abrir e fechar os blocos no mesmo nivel de identação.

## **Git**

| Tipo  | Nomenclatura  | Descrição  |
|-------|---------------|------------|
| Branch  | `issue-(id)` | Sendo id um valor numérico inteiro Ex: `issue-15`|
| Commit  | Conventional Commits:<br>`<tipo>: <descrição>`<br>Descrição em inglês, iniciando com verbo no presente simples  |  <ul><li>`test`: indica qualquer tipo de criação ou alteração de códigos de teste.</li><li>`feat`: indica o desenvolvimento de uma nova feature ao projeto.</li><li>`refactor`: usado quando houver uma refatoração de código que não tenha qualquer tipo de impacto na lógica/regras de negócio do sistema.</li><li>`style`: empregado quando há mudanças de formatação e estilo do código que não alteram o sistema de nenhuma forma.</li><li>`fix`: utilizado quando há correção de erros que estão gerando bugs no sistema.</li><li>`chore`: indica mudanças no projeto que não afetam o sistema ou arquivos de testes. São mudanças de desenvolvimento.</li><li>`docs`: usado quando há mudanças na documentação do projeto.</li><li>`build`: utilizada para indicar mudanças que afetam o processo de build do projeto ou dependências externas.</li><li>`revert`: indica a reversão de um commit anterior.</li></ul> 🔗 [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/)

## **Pull Request**

|  Categoria  | Diretriz / Padrão  | 
|-------------|--------------------|
| Descrição   |  Breve descrição de que o PR estará implementando ou resolvendo, podem ser feitas em português. |
| Título      | Nome da issue (branch) entre colchetes + descrição da implementação |
| Aprovação | Coordenador do projeto ou pessoa também relacionada à task |