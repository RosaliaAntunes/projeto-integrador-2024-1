# Instruções de uso

Aqui, você deve elaborar um "guia" para **usuários**. Explique como a interface gráfica deve ser utilizada.
nome: Um campo para o nome da matéria.

primeira_nota: Um campo para armazenar a nota do primeiro bimestre.

segunda_nota: Um campo para armazenar a nota do segundo bimestre.

terceira_nota: Um campo para armazenar a nota do terceiro bimestre.

quarta_nota: Um campo para armazenar a nota do quarto bimestre.

media_notas: Um campo para armazenar a média das notas, calculada automaticamente a partir das notas dos quatro bimestres. Este campo é configurado como opcional (blank=True) e possui um valor padrão de 0.

Além disso, o método save() é sobrescrito para calcular automaticamente a média das notas antes de salvar o objeto no banco de dados. Esse método realiza a soma das quatro notas e divide por 4 para obter a média. No entanto, existe um problema potencial com a operação de divisão na linha self.media_notas = (self.primeira_nota + self.segunda_nota + self.terceira_nota + self.quarta_nota) / 4. O resultado dessa divisão será um número decimal e, como media_notas é um campo IntegerField, isso resultará em uma perda de precisão, já que os números decimais serão truncados para inteiros. Para corrigir isso, você pode converter os valores para float antes de realizar a divisão, garantindo que o resultado seja um número decimal.