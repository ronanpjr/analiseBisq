1 - Mostrar a aba system do Sonar Graph destacando
- linhas de código
- cycle groups
- complex code


2 - Averiguar se interfaces gráficas estão separadas das classes que representam o modelo (padrão MVC) 

Para isso, vocês devem procurar entender a estrutura do sistema
Para sistemas web, provavelmente existirão classes que mapeiam as rotas (http://www....)
para classes/métodos específicos da aplicação. Normalmente essas classes são os Controladores/Controllers.
Para sistemas que não são Web, as interfaces gráficas geralmente são classes Java (Swing e AWT).
Neste caso, os eventos da interface (clicks em botões, por ex), são mapeados para Controladores e depois para
classes do domínio.

3 - Procurar no sistema se os padrões que vimos até o momento são usados


Para isso, um caminho inicial é ver se o nome do padrão aparece. Isso pode ser
feito usando a ferramenta Edit - Search in System.
Para cada padrão mostrar o código cliente que o usa
Refletir no sentido de julgar se a aplicação do padrão está correta
Construir um diagrama de classe para facilitar mostrar para a sala de aula (para isso para pelo menos dois padrões)
No mínimo 3 padrões por projeto

4 - Procurar por códigos-cliente que usam hierarquias de herança. 
Para isso, procure inicialmente por pacotes com o abstractness (métrica) alto
Olhe dentro do pacote e identifique a hierarquia (estude ela)
Gere uma visualização mostrado todas as dependências in para a classe abstrata/interface (código cliente)
Analisar o código cliente para ver como a interface/classe abstrata é usada (polimorfismo) 
procure identificar se a hierarquia é referente à algum padrão que já vimos
Também montar diagramas de classe para facilitar a explicação

5 - Identificar e mostrar quais são os pacotes com maior e menor número de dependências In e Out.
Para isso, analise a métrica Number of Incoming Dependencies e Number of Outgoing Dependencies 

6 - Ciclos. Mostrar quantos ciclos existem no sistema
Para isso, use o menu Cycle Groups do Sonar

Para o projeto de desenvolvimento:

1 - Apresentar o diagrama de classes do sistema que está sendo desenvolvido
2 - Apresentar o código das estruturas iniciais do projeto. O foco é a criação das classes que aparecem no diagrama de classes e suas relações
3 - Mostrar códigos-cliente que iniciam um determinado caso de uso (main)


