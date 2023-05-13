# Mini_Zoologico

Crie um programa em Java que implemente uma hierarquia de classes para representar diferentes tipos de animais em um zoológico.
A classe abstrata Animal deve ser a classe base, que contém atributos como id (identificador), nome, idade e peso. Todo animal deve ser capaz de crescer (mudar a idade anualmente), comer (cada vez que come, aumenta uma unidade de peso) e fazer atividades físicas (perde 2 unidades de peso). Todo animal também deve conter o método abstrato familia que irá imprimir a família biológica de cada classe de animal.

A partir da classe Animal, crie duas subclasses abstratas: Mamífero e Ave. A classe Mamífero deve ter um atributo adicional para a quantidade de pelos e a classe Ave deve ter um atributo para a envergadura das asas.

A classe Mamífero deve conter o método alimentação que retorna do que ele se alimentou da última vez (crie um atributo "String alimento" para armazenar essa informação. Inicialize como uma String vazia no construtor da classe Animal) e a classe Ave contém o método ehVoador que diz se a ave em questão plana ou voa(crie um novo atributo "boolean voa" pra armazenar essa informação. True se voa, false se não voa).

Em seguida, crie duas subclasses para cada uma dessas classes. Para a classe Mamífero, criem as classes Leao e Lobo. Para a classe Ave, criem as classes Pato e Águia, em cada uma sobrescreva o método ehVoador para retornar se a ave plana ou voa (pato plana e águia voa).

Cada uma dessas subclasses deve ter seus próprios atributos e métodos específicos:

Na classe Leao, crie um atributo "private int vacinas" que indica quantas vacinas o leao tomou e um método "getVacinas()" que retorna este atributo

Na classe Lobo, crie um atributo "private boolean ehAlpha" que indica se aquele lobo é o alfa da alcatéia ou não. Crie um método "getElAlpha()" que retorna este atributo.

Na classe Pato, crie um atributo "private String corPenas" que indica a cor dominante do pato. Crie um método "getCorPenas()" que retorne esse atributo

Na classe Aguia, crie um atributo "private boolean gerouFilhos" que indica se essa águia gerou filhos. Crie um metodo "getGerouFilhos()" que retorna este atributo.

Finalmente, crie na sua Main duas funções em um menu. A função inserir animais e remover animais.

Crie um arraylist de Animal na main()

A função inserir pergunta qual dos 4 animais o usuário deseja inserir. Ao selecionar, crie o objeto Animal instanciado como o a classe selecionada e adicione ao vetor Animal (ex.: Animal a = new Leao(...))

A função remover recebe dois parâmetros, um id e o ArrayList de Animal. O id do animal que deseja ser removido do ArrayList é usado para identificá-lo. Percorra o ArrayList de animais tentando achar o id passado como parâmetro e remova do ArrayList. Imprima as informações do animal removido. São elas: id, idade, nome, pelos ou envergadura(veja se a classe se aplica ao atributo), e a informação exclusiva de cada classe (vacinas se o removido for leao, ehAlpha se o removido for lobo, corPenas se o removido for Pato, gerouFilhos se o removido for águia)
