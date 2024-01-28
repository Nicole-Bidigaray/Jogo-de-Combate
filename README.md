# Jogo de Combate

## Introdução

Jogo de Combate feito com Python no Projeto 2 da Rocketseat das aulas de POO.

## Sobre o desafio

### Herança
Herança é um princípio de POO onde uma classe (chamada de classe filha) herda propriedades e métodos de outra classe (chamada de classe pai ou classe mãe).

No código, Heroi e Inimigo são classes filhas que herdam da classe pai Personagem. Isso é evidente na linha super().__init__(nome, vida, nivel), onde ambas as classes chamam o construtor da classe Personagem. Isso permite que Heroi e Inimigo usem propriedades (nome, vida, nivel) e métodos (como exibir_detalhes, receber_ataque, atacar) definidos na classe Personagem.

### Encapsulamento
Encapsulamento é a prática de ocultar detalhes internos de uma classe e expor apenas o necessário ao exterior. Isso é feito para prevenir acesso direto aos dados da classe, o que pode proteger a integridade dos dados.

No código, os atributos __nome, __vida, __nivel, __habilidade, e __tipo são exemplos de encapsulamento, indicados pelo uso de dois sublinhados (__). Isso torna esses atributos privados, significando que eles não podem ser acessados diretamente fora da classe. Em vez disso, fornece métodos públicos como get_nome, get_vida, get_nivel, get_habilidade e get_tipo para acessá-los, o que é uma prática de encapsulamento.

### Polimorfismo
Polimorfismo é a habilidade de chamar o mesmo método em diferentes objetos e cada um deles responder de maneira diferente. Em termos simples, diferentes classes podem definir métodos que parecem iguais, mas comportam-se de maneira diferente.

O polimorfismo no código é mais sutil. Ele pode ser visto na sobreposição (override) do método exibir_detalhes nas classes Heroi e Inimigo. Ambas as classes estendem esse método da classe Personagem, adicionando informações específicas (__habilidade para Heroi e __tipo para Inimigo). Esse é um exemplo de polimorfismo, onde um mesmo método (exibir_detalhes) tem comportamentos diferentes dependendo da classe em que é chamado.

Além disso, a classe Heroi introduz um novo método ataque_especial, que não existe na classe pai Personagem. Isso não é exatamente polimorfismo, mas mostra como a herança pode ser usada para estender a funcionalidade de uma classe base.

Resumindo, o código demonstra herança na relação entre Personagem, Heroi e Inimigo, encapsulamento nos atributos privados, e polimorfismo na sobreposição do método exibir_detalhes.
