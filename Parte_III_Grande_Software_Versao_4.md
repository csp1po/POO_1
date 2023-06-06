# **Grande Software Versão 4**


## **Nada Permanece Igual**

![molly_buque_flores_233](../img_readme/molly_buque_flores_233.png)

**A mudança é inevitável**. Não importa o quanto você gosta do seu software agora, provavelmente ele mudará amanhã. E quanto mais difícil você tornar seu software alterado, mais difícil
será para responder **às necessidades de mudança do seu cliente**.


## **Loja de Instrumentos de Corda do Rick está se expandindo**

Logo após a venda de três guitarras para o grupo de rock Augustana, o negócio de guitarras do Rick está indo melhor do que nunca - e a ferramenta de busca que você construiu para ele é a base de seu negócio.

![software_e_o_maximo_234](../img_readme/software_e_o_maximo_234.png)

A figura abaixo mostra o diagrama de classe completo para o aplicativo de pesquisa de guitarras do Rick, exatamente como quando terminamos o **Grande Software Versão 3**. Cabe a você alterar este diagrama para que o Rick possa começar a vender bandolins, e sua ferramenta de pesquisa possa ajudar a encontrá-los também e que combinam com as preferências dos seus clientes, assim como ela já faz com as guitarras.

![diagrama_classes_versao3_235](../img_readme/diagrama_classes_versao3_235.png)



## Quais sugestões você teria para adicionar o suporte aos bandolins?

A figura abaixo mostra uma sugestão para dar suporte aos bandolins.

### Primeira alteração de projeto

![novo_diagrama_classes_app_236](../img_readme/novo_diagrama_classes_app_236.png)

1. Criação de uma classe base abstrata para as propriedades comuns de ``Mandolin`` e ``Guitar``.

2. Criação da classe ``Mandolin``.


> ### Classe Abstrata? (Algumas características)

> * As classes abstratas são alocadores de espaço para classes de implementação reais
> * A classe abstrata define o comportamento e as subclasses o implementam
> * Classe genérica onde não há objetos instanciados
> 

### Segunda alteração de projeto

Também será necessária a criação de uma classe para
as especificações dos bandolins (i.e. ``MandolinSpec``), apesar de sua semelhança com
``GuitarSpec``. Porém, há diferenças entre os instrumentos. Veja a figura abaixo.

![mandolin_spec_238](../img_readme/mandolin_spec_238.png)


### Terceira alteração de projeto:

As classes ``Spec`` são bem semelhantes que tal criarmos uma ``Spec`` abstrata também? Veja figura abaixo.

![instrument_spec_class_239](../img_readme/instrument_spec_class_239.png)


## **Analisando o diagrama completo**

Parece que todo o trabalho que fizemos nas versões 1, 2 e 3 valeu a pena. Conseguimos adicionar o suporte para bandolins à ferramenta de pesquisa do Rick. Aqui está o diagrama de classe completo.

![diagrama_classes_completo_versao4_240_241.png](../img_readme/diagrama_classes_completo_versao4_240_241.png)

> **Observação**: aqui está o princípio que nos levou a criar as classes abstratas ``Instrument`` e ``InstrumentSpec``.
> 
> 
> Sempre que você encontrar um comportamento comum em dois ou mais lugares, procure abstrair esse comportamento em uma classe e, em seguida, reutilize-o em classes comuns.

Guarde a tabela abaixo.

| Como chamamos em Python | Como chamamos em UML | Como mostramos em UML |
|--- |--- |--- |
| Classe Abstrata | Classe Abstrata | Nome da Classe em Itálico |
| Relacionamento (Relação) | Associação | ![associacao](../img_readme/associacao.png) |
| Herança | Generalização | ![heranca](../img_readme/heranca.png) |
| Agregação | Agregação | ![agregacao](../img_readme/agregacao.png) |





## Grande Software Versão 4 da aplicação

### Implemente as alterações necessárias para a Loja do Rick

1. Implemente o diagrama de classes que demonstra o modelo de expansão da aplicação do Rick com a inclusão da classe ``Mandolin``

2. Após a implementação analise o Diagrama de Classes e Código implementados e aponte os problemas encontrados nessa forma de implementação.

3. Teste o sistema

