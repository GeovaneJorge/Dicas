# Dicas de desenvolvimento
Dicas de desenvolvimento


Não podemos deixar de mencionar as estruturas de controle que
ajudam o programa a “tomar decisões”. O if executa um bloco de código
após verificar se a condição é verdadeira:
if ($idade >= 18) {
echo “Você é maior de idade.”;
} else {
echo “Você ainda é menor de idade.”;
}

Os laços de repetição do PHP são for, while e do...while. Cada um tem
suas próprias características e pode ser usado de acordo com as
necessidades do programa.

Laço for
Quando você sabe quantas vezes precisa repetir uma ação, o laço for é
a melhor opção. A inicialização, a condição de repetição e o incremento
são os três passos pelos quais ele funciona. Vamos analisar um exemplo:
for ($i = 0; $i < 5; $i++) {
echo “Este é o número $i<br>“;
}
Nesse exemplo, o PHP imprimirá a frase cinco vezes, mudando o valor
$i para cada repetição. O laço começa com $i = 0, vai até $i se menor
que 5, e incrementa o valor de $i em 1, a cada vez que $i é menor que 5.
Simples, direto e extremamente eficaz quando você sabe os limites de
repetição.

Laço while

Por outro lado, quando você não sabe exatamente quantas vezes o
código precisa ser repetido, você pode usar o while, porque ele tem
uma condição que especifica até quando o código deve ser executado.
Observe o código a seguir:
$contador = 0;
while ($contador < 5) {
echo “Contando: $contador<br>“;
$contador++;
}

O código será executado enquanto a variável $contador for menor
que 5. Portanto, até que essa condição deixe de ser verdadeira, o
laço continuará executando as instruções dentro dele. O segredo do
while é que, caso a condição nunca seja satisfeita, ele poderá rodar
indefinidamente.

Laço do...while

O do...while é semelhante ao while, mas possui uma diferença, isto é, ele
garante que o código dentro do laço será executado pelo menos uma
vez, mesmo que a condição seja falsa desde o início. Isso ocorre porque
a primeira execução precede a verificação da condição. Veja:
$numero = 6;
do {
echo “Número: $numero<br>“;
$numero++;
} while ($numero <= 5);
Mesmo que $numero comece como 6 (maior que 5), o laço vai rodar
uma vez, porque a verificação só é feita no final da instrução.
Os laços de repetição são ferramentas ideais para tarefas como revisar
uma lista de produtos ou repetir uma ação com base em interações
de usuário. Lembre-se sempre de que, em qualquer um deles, a chave
é ter certeza de que a condição de término será alcançada em algum
momento. Senão, você pode acabar criando um “loop infinito” e travar
sua aplicação.
