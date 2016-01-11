# marsrover-zup
Solução do Problema Mars Rovers em Ruby on Rails

Eu usei RSpec para testes de unidade junto com guarda e guarda-rspec para o teste contínuo. Eu usei Rake para a execução de tudo.

Temos 3 tarefas Rake: 

 rake -T
rake batch        # Executa o aplicativo no modo batch.
rake interactive  # Executa o aplicativo no modo interativo.
rake spec         # Executa os exemplos de código rspec.

O modo batch será executada a entrada de exemplo a partir da especificação.
O modo interativo vai esperar a entrada do usuário, que pode ser ou digitado no terminal ou dirigida a partir da linha de comando com atribuições.
A rspec executa todos os testes de unidade.

$ rake batch
=> 1 3 N 5 1 E

# plateau.txt
5 5
1 2 N
LMLMLMLMM
3 3 E
MMRMMRMRRM


$ rake interactive < plateau.txt
=> 1 3 N 5 1 E



$ rake interactive
5 5
1 2 N
LMLMLMLMM
3 3 E
MMRMMRMRRM
<Control-D>
=> 1 3 N 5 1 E



