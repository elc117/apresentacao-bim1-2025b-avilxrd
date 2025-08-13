# Efeitos colaterais (side effects)
Na computação, dizemos que algo possui algum efeito colateral caso haja algum outro efeito observável que não seja o seu efeito primário (ler os argumentos e retornar).<br>

### O que pode ser um efeito colateral? 
- Modificar uma variável não local, variável local estática ou um argumento passado por referência
- Lançar erros ou exceções
- Entrada/saída de dados
- Chamar outras funções com efeitos colaterais

### Qual o problemas dos efeitos colaterais?
Na presença de efeitos colaterais, o comportamento de um programa pode variar de acordo com o uso. <br>
Entender e _debugar_ uma função com efeitos colaterais requer um entendimento do contexto. <br>

### Paradigmas x Efeitos colaterais
O paradigma adotado interfere diretamente no uso dos efeitos colaterais, um ótimo exemplo é na comparação entre os paradigmas **Imperativo** e **Declarativo**.
- Imperativo: utiliza os efeitos colaterais ao seu favor, pois funciona através da atualização do estado de um sistema.
- Declarativo: diferentemente da anterior, a programação declarativa apenas relata o estado do sistema, sem efeitos colaterais.

O paradigma funcional busca minimizar/eliminar os efeitos colaterais. A falta desses efeitos facilita a *verificação formal* do programa. <br>

A linguagem Haskell elimina os efeitos colaterais, como os de E/S e outras computações "stateful" (mantém informações sobre o estado). Isso é feito através da substituição por **Mônadas**. <br>

- Mônada: uma maneira de estruturas os cálculos como uma sequência de etapas, onde cada etapa não produz apenas um valor, mas também informações extras sobre a computação, como falhas potenciais, não determinismo, efeitos colaterais.

# Fontes
- [Paradigmas de Programação: Uma Abordagem Comparativa - **5.2 Efeitos Colaterais**](https://leandromoh.gitbooks.io/tcc-paradigmas-de-programacao/content/5_paradigma_funcional/52_efeitos_colaterais.html)

- []