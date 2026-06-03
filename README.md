# caixa-branca-nickolas
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
