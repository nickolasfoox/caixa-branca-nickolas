# caixa-branca-nickolas
INTRODUÇÃO

Essa atividade visa verificar erros e corrigir os erros com o metodo de caixa branca.

@startuml

start

:Nó 1: Inicializa SQL e chama conectarBD();

try

  :Nó 2: Monta Query SQL por concatenação;
  
  :Nó 3: Cria Statement e executa Query;
  
  while (Nó 4: rs.next()?) is (Sim)
  
    :Nó 5: Atribui nome e result = true;
    
  endwhile (Não)
  
catch (Exception e)

  :Nó 6: Catch Vazio (Abafa o erro);
  
end try

:Nó 7: Return result;

stop

@enduml

Número de Nós (N): 7

Número de Arestas (E): 9 (Considerando o fluxo padrão e os desvios de exceção mapeados para o catch).

Número de Componentes Conexos (P): 1 (O método é um programa único/isolado).

V(G) = E - N + 2P

V(G) = 9 - 7 + 2(1)

V(G) = 2 + 2

V(G) = 4

CONCLUSÃO

O teste funcional é nescessário para virificar principalmente erros de segurança.

A maior dificuldade foi a analise do codigo onde tive que buscar mais conhecimentos sobre o codigo de forma geral.
A correção do codigo visto que foi nescessário rever cada erro e exercer o conhecimento para corrigilos sem criar novos erros.

O impacto da correção do codigo foi corrigir possiveis erros de segurança.

A qualidade do software é importante principalmente para evitar fraudes e vazamento de dados.
