# Aula-16

O programa tem em seu struct o molde do que é o Cliente (nome, idade e sexo).
Dentro da função main tem um vetor capaz de armazenar até 100 clientes e variáveis para acumular as contagens e idade e logo em seguida ele tenta abrir o arquivo "clientes.csv" utilizando a operação "r" (read) que serve para leitura.

O primeiro fgets vai ler a primeira linha onde fica o Nome, Idade e Sexo e vai ignorá-la. O while vai ler as próximas linhas até o arquivo acabar (NULL).

O sscanf vai ser uma função que quebra a linha do texto, nesse formato "%[^;];%d;%c" o programa vai ler o texto até o ";", vai pular o mesmo, ler a idade pula o outro ";" e le o caractere (sexo).

Ao ler com sucesso as 3 informações o programa vai somar a idade ao total geral; verificar se é homem ou mulher, incrementa o contador daquele gênero e soma a idade no grupo correspondente; passa para a próxima posição do vetor, no caso, o próximo cliente. Depois que o laço termina, o arquivo é fechado com "fclose(arquivo);"


Após tudo isso o programa irá exibir o relatório e as estatísticas.
No printf é possível observar "%-25s | %-5d | %-4c\n" servem para que o nome, idade e sexo agrupem sempre os espaços atribuídos na tela, alinhados à esquerda, deixando na forma de uma tabela organizada.

O "?" e o ":" são um if/else abreviados.
"qtd_M > 0 ? (soma_idade_M / qtd_M) : 0" = Quantidade de homens é maior que 0? Se sim divida a soma das idades pela quantidade, senão o valor é 0.
