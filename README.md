<h1 align="center">GitHub Explorer</h1>

<div align="center">
<img src="assets/preview-github-explorer.gif" alt="Github Explorer">
</div>

<p>&nbsp;&nbsp;</p>

### 💻 Projeto
Aplicativo para salvar repositórios do GitHub, visualizar detalhes e lista de issues. Projetado pela Rocketseat no bootcamp GoStack.

### ⚙️ Tecnologias
As tecnologias utilizadas neste projeto foram:
- ReactJS
- TypeScript
- Styled-Components
- HTML

### 📖 Aprendizado
- Condicionar a exibição de um elemento a existência de valor em uma variável:

  ```
  {inputError && <Error>{inputError}</Error>}
  ```
  Utilizando a sintax de uma expressão lógica, o JavaScript só continua a execução do código caso a primeira condição seja verdadeira, fazendo o componente *Error* ser exibido apenas se a variável *inputError* for *truthy*, ou seja, se ela existir.

- Passar uma propriedade para um *Styled Component* somente se existir valor em uma variável:

  ```
  <Form hasError={!!inputError} onSubmit={handleAddRepository}>
  ```
  Negando uma variável com ! obtemos o oposto do seu valor booleano. Negando novamente com outro ! temos o equivalente booleano da variável verificada. Assim, podemos passar como propriedade a existência de uma variável não booleana em vez do seu valor.

- Estilizar elementos encadeados com *Styled Components*:

  ```
  a {
    display: flex;
    align-items: center;
    transition: transform 0.2s;

    & + a {
      margin-top: 16px;
    }

    &:hover {
      transform: translateX(10px);
    }
  }
  ```
  Com *Styled Components*, podemos estilizar com facilidade e alta legibilidade elementos HTML aninhados. Utilizando a sintax semelhante a de bloco de código com ```{ }``` obtemos uma semântica parecida também, em que um elemento dentro de outro representa o mesmo aninhamento das tags do HTML. Os atributos dentro do bloco de chaves afeta apenas aquele elemento que segue àquelas condições de encapsulamento.
