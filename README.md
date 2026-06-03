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
