## 🔄 Diferença entre Branch e Feature

Na prática, a diferença entre **branch** e **feature** é mais uma questão de uso do que de conceito.

- **Branch** é uma ramificação do código onde você pode trabalhar isoladamente, sem afetar o código principal, que normalmente está nas branches `main` ou `master`.
- Uma **feature** (funcionalidade) geralmente é desenvolvida em uma branch separada, chamada *feature branch*. Ou seja, a branch é o espaço onde você cria ou altera funcionalidades.
  
### Fluxo comum de desenvolvimento:

1. Você cria uma **branch** (normalmente a partir da `develop`) para desenvolver uma **feature**.
2. Trabalha nela adicionando funcionalidades e fazendo alterações.
3. Quando a feature está pronta e testada, a branch é mesclada (merge) na `develop`.
4. Depois que várias features são concluídas e testadas na `develop`, o código é mesclado para a branch principal, que pode ser a `main` ou `master`.

**Resumindo:**  
- **Branch** é o "local" de trabalho.  
- **Feature** é o que você está desenvolvendo dentro dessa branch.