# Linguagem de programação Java
Revisão sobre a linguagem Java

## Tópicos de Estudos

* [Linguagem de programação Java](01.md)
  * Paradigmas de Programação
  * Modelo de Tipagem de dados
  * Modelo de construção da Linguagem  
  * Estilo de código
  * Versões
    * Java 1.8
      * Novas funcionalidades 
    * Java 11
      * Novas funcionalidades
    * Java 18
      * Novas funcionalidades
    * Java 19 
      * Novas funcionalidades
  * Conjunto de palavras reservadas
  * Ambiente de Desenvolvimento e Ferramentas
    * Documentação oficial
    * JDK
    * IDEs
      * Como criar um projeto Java em uma IDE
  * Mercado
    * Popularidade 
      * Tiobe
      * Survey da Stackoverflow 
      * Survey da Jetbrains 
    * Vagas e salários 
      * Survey da Stackoverflow 
      * Survey da Jetbrains  
    * Áreas de aplicações da linguagem Java 
      * Survey da Stackoverflow 
      * Survey da Jetbrains  
    * Principais bibliotecas/frameworks 
      * Survey da Stackoverflow 
      * Survey da Jetbrains  
* [Hello World](02.md)
  * Estrutura mínima de um código Java
  * Nome do arquivo e Extensão
  * Nome da classe
  * Método main
  * Escrever dados no console
  * Indentação de código
  * Delimitação de uma instrução
  * Delimitação de bloco de instruções
  * Compilação e Execução via linha de comando
* [Tipos de Dados e operadores](03.md)
  * Tipos de Dados
      Os tipos primitivos são boolean, byte, char, short, int, long, float e double
  * Declarações de variáveis
      As variaveis sao feitas geralmente no inicio do programa, exemplo:
      String carroModelo 1.

  * Nomes válidos para variáveis e boas práticas 
      São nomes simples e diretos, sempre deve ser utilizado o métudo camelcaze, Exemplo
      String exemploDeVariavel;
  * Atribuição de valores
      Acontece quando é definido o valor de uma variavel, exemplo:
      Int anoDeLançamento = 1990;

  * Operadores
    * Operadores aritméticos
        Os principais são:
          Soma +
          Subtração -
          Divisão /
          Multiplicação *

    * Operadores booleanos
        True ou False, Exemplos:
          boolean carroComProblema = true;

  * Conversão de tipos de dados
      É possivel pasar usando o comando "To(tipo de dado desejado) exmplo:"
        *ToDecimal
        *ToString
        *ToBoolean
        *ToChar
* [Saída de Dados](04.md)
  * Método System.out.println
      System.out.println é utilizado para exibir informações na tela, e pular uma linha em sequência
  * Método System.out.print
       System.out.println é utilizado para exibir informações na tela, e não pular uma linha em sequência
  * Exibir o valor de uma variável
      String modeloDeCarro = "Celta"
      System.out.println(modeloDeCarro)
  * Exibir o valor de um decimal  
      double numeroDecimal = 10.00
      System.out.println(numeroDecimal)
* Classe Math
  * Definição
      Classe que permite realizar operações de matematica expecificas.
  * Principais operações 
      math.randon
      Math.Abs
* String
  * Concatenação de String
    String modeloCarro1 = "Celta";
    System.out.println("Eu tenho um " + modeloCarro1 + " Turbo");

  * Principais operações sobre String
    -Concatenações e atribuições

  * Comparação de String 
    "macaco" == "leao"
  * Diferença entre String e caracter
    String é um conjunto de palavras, um char é apenas uma letra.
* Entrada de Dados
  * Classe Scanner
    * Obter um valor inteiro
        Scanner sc1 = new Scanner(System.in);
        int valorInteiro = 1990;
    * Obter um valor decimal
        Scanner sc1 = new Scanner(System.in);
        float valorDecimal = 19.209;
    * Obter um valor de texto 
        Scanner sc1 = new Scanner(System.in);
        String textoString = "Maria Silva";
* Fluxo de Controle
  * Estruturas de Decisões
    * if-else-then
        Utilizado para realizer validações, exemplo:
          int numeroUm = 10;
          int numeroDois = 90;
          if (numeroDois > numeroUm){
            system.out.println("Entrou na validação");
          }
    * switch
        Utilizado para validar o que fazer com um resultado recebido, exemplo:
        int valor = 10;
          switch(valor){
            case 4:
              System.out.println("Não vai entrar aqui");
              [breake;]
            case 7:
              System.out.println("Não vai entrar aqui");
              [breake;]
            case 10:
              System.out.println("Vai entrar aqui");
              [breake;]
          }
  * Estruturas de Repetições
    * for
        Utilizado para fazer repetiçoes, exemplo:
          for(int i = 100;i < 100; i++){
            System.out.println("Vai repetir ate i for maior que 100");
          }

    * while
        Utilizado para fazer repetições tambem, exemplo:
          Int valor = 10;
            while(valor < 100){
              System.out.println("Vai repetir ate i for maior que 100");
              i++;
            }

    * do-while 
        Utilizado para fazer repetições tambem, exemplo:
          Int valor = 10;
          do{
            System.out.println("Vai repetir ate i for maior que 100");
              i++;
          }while(valor < 100);

    * Comandos break e continue
        Utilizado para controlar o fluxo do seu programa.
          int valorUm = 100;
          int valorDois = 200;

          if(valorUm > valorDois){
            break
          }
    *  Arranjos e Matrizes

      Definição matemática
      Difinição matemárica de arranjo: "Agrupamentos formados com p elementos de um conjunto de n elementos"
      Difinição matemárica de matriz: "Matriz é uma tabela organizada em linhas e colunas no formato m x n"
      Declaração de arranjos
        String[] carros = {"Volvo", "VW", "Ford", "Fiat"};
      Declaração de matrizes
        int[][] tab = new int[2][2];
      Percorrer arranjos
        String[] carros = {"Volvo", "VW", "Ford", "Fiat"};
        for(String carro : carros){
          //para cara carro
        }
      Percorrer matrizes
        int[][] tab = new int[10][9];
        for(int i = 0; i < 10; i++)
          for(int j = 0; j < 9; j++) tab[i][j] = i*j; 
      Linha a linha
        int[][] tab = new int[10][9];
        for(int i = 0; i < 10; i++)
      Coluna a coluna
        int[][] tab = new int[10][9];
        for(int i = 0; i < 10; i++)
          for(int j = 0; j < 9; j++) tab[i][j] = i*j; 
      Em diagonal
          for(i=M-1; i>=0; i--){
            for(j=N-1; j>=0; j--){
      Utilizar arranjos e matrizes como parâmetros de métodos
      Utilizar arranjos e matrizes como retorno de métodos
      Tratamento de Exceções

      Definição O tratamento de exceções é feito para tratar casos inesperados no código.
      Exceções comuns
      Divisão por zero ArithmeticException: / by zero;
      Conversão de tipos de dados inválidos
      Acessar uma posição inválida em um arranjo ArrayIndexOutOfBoundsException;
      Acessar uma String nula
      Bloco para capturar uma exceção
      try {
      //código a ser exec
      } catch (Exception e) {
      //executa caso der erro;
      } finally {
      //executa de qualquer forma no final;
      }
      Métodos estáticos

      Estrutura de declaração de um método estático
      public static void teste () {
      }
      Nomes válidos e boas práticas
      Parâmetros
      Retorno
      Utilização de métodos estáticos
      Disponíveis na mesma classe
      Disponíveis em outra classe/arquivo.
      Recursão
      Classe

      Definição É a estrutura de um objeto que possui e atributos e métodos;

      Representação de classe e objeto na UML image

      Diferença entre classe e objeto Classe é a estrutura e o objeto é o conteúdo estruturado pela classe;

      Atributos São as propriedade da classe como: nome, idade e etc..

      Métodos São as funções, as ações executadas pela classe.

      Construtor É a primeira função executada pela classe que pode inicializar o objeto.

      Objeto É o conteúdo estruturado de uma classe com dados;

      Inicialização de um objeto

        pessoa pes = new Pessoa();
      Utilização de um objeto

        pes.nome = "Henry";
      Comparação de objetos
      pes1.equals(pes2); //retorna true ou false
      Método toString
      Visibilidade de atributos e métodos
      Público
        public String nome;
      Privado
        private String nome;
      Sobrecarga de métodos
      @Override
      public void teste(){
      }
      Sobrecarga de construtores Uma classe java pode conter mais de um construtor podendo fazer com que o objeto possa ser criado de jeitos diferentes, como por exemplo com a passagem parametros ou sem.
      Pacotes

      Definição São utilizados para fazer a organização de classes.

      Representação de pacotes na UML image
      Definição de um pacote em uma classe São utilizados para fazer a organização de classes.

      Importando uma classe de um pacote diferente É impossível importar classes para outro pacote

      Visibilidade de classes, atributos e métodos

      Default/Pacote
      Pacote default

      import package;
      Importar uma classe em um pacote default
      import package.pacote;
      Escopo de classe e objeto

      Definição O escopo de uma classe são os limites de até onde serta funcionalidade tem efeito sobre a aplicação.
      Palavra reservada static
      São métodos que não tem nenhuma dependencia de objetos e não dependem de nenhum conteúdo.
      Herança

      Definição Permite que as classes java possuam uma estrutura onde podem ocorrer classes pais e filhas que podem herdar comportamentos.

      Representação de herança na UML image
          ![ClasseMamifero](https://user-images.githubusercontent.com/104472351/190501546-0a9c0667-3c5a-46d5-a309-76ce5188ec47.jpg)

    *  Criação de uma classe que realiza herança

      public class Pessoa {
        public String nome;
        public String cpf;
      }

      public class Aluno extends Pessoa {
        public Aluno(String nome, String cpf){
        super(nome, cpf)
        }
      }




  * Sobreescrita de métodos
      Com a sobrescrita, conseguimos especializar os métodos herdados das superclasses, alterando o seu comportamento nas subclasses por um mais específico.

      ___________________________________
      |          <<interface>>           |
      |            Animal                |
      |__________________________________|
      |        cacar() :String          |
      |                                 |
      |_________________________________|

                    ^
                   / \
                    | 
                    |
                    |

      ___________________________________
      |             Reptil               |
      |                                  |
      |__________________________________|
      |                                  |
      |                                  |
      |_________________________________ |
      |                                  |
      |           cacar():String         |
      |__________________________________|                                  

  * Polimorfismo
      Polimorfismo significa "muitas formas", é o termo definido em linguagens orientadas a objeto, como por exemplo Java, C# e C++, que permite ao desenvolvedor usar o mesmo elemento de formas diferentes
    * Conversão de tipos 
        int i = 64;
        String aChar = new Character((char)i).toString();
  * Visibilidade de atributos e métodos
      Em Java, a visibilidade padrão de classes, atributos e métodos está restrita a todos os membros que fazem parte de um mesmo pacote
     * Protegido
        Sua principal finalidade é auxiliar no processo de extensão (herança) da classe. Em princípio, um campo/método protected poderia muito bem ser privado: ele trata de detalhes de implementação, mas não do contrato da classe
  * Palavra reservada super 
      A palavra reservada super é utilizada para fazer referencia a métodos ou atributos da super classe
     * Encadeamento de construtor 
            public Honda(String motor, String modelo, double preco){
            super(modelo, preco);
            }
     * Encadeamento de método
          super.metodo().
* Interface
  * Definição
      A interface é um recurso muito utilizado em Java, bem como na maioria das linguagens orientadas a objeto, para “obrigar” a um determinado grupo de classes a ter métodos ou propriedades em comum para existir em um determinado contexto, contudo os métodos podem ser implementados em cada classe de uma maneira diferente.
     * Representação de interface na UML
          
     
  * Criação de uma classe que implementa uma interface
    interface IReajuste
        {
            double Reajuste();
        }
  * Sobreescrita de métodos
    double ReajusteTeste()
        {
            double Reajuste();
        }
  * Polimorfismo
      Polimorfismo denota uma situação na qual um objeto pode se comportar de maneiras diferentes ao receber uma mensagem
    * Conversão de tipos 
        double i = 42.0;
        String str = Double.toString(i);
* Classe abstrada
  * Definição
     * Representação de classe abstrata na UML
        ![image](https://user-images.githubusercontent.com/104472351/190501444-1571976c-809b-4fb0-8128-616ac4bdd1ee.png)
  * Criação de uma classe que extende uma classe abstrata
      public class ContaPoupanca extends Conta {

      @Override
      public void imprimeExtrato() {
        System.out.println("### Extrato da Conta ###");

        SimpleDateFormat sdf = new SimpleDateFormat("dd/MM/aaaa HH:mm:ss");
        Date date = new Date();

        System.out.println("Saldo: "+this.getSaldo());
        System.out.println("Data: "+sdf.format(date));

      }
    }

  
* Coleções 
  * Definição
  * List e Arraylist 
    * Aplicações
    * Declaração
    * Utilização
      * Adicionar elementos
      * Acessar elementos
      * Atualizar elementos 
      * Remover elementos 
  * Map e HashMap
    * Aplicações 
    * Declaração
    * Utilização
      * Adicionar elementos
      * Acessar elementos
      * Atualizar elementos 
      * Remover elementos 
* Tipo Enumerado
  *  Definição
     * Representação de tipos enumerados na UML
* Representação de tempo
  * Classe Date
  * Classe Calendar
  * API Date/Time Java 8
    * LocalDate
    * LocalTime
    * LocalDateTime
    * Period
    * Duration
    * Formação de Date/Time 
* Modificador final
  * Definição
    * Representação de final no diagrama UML 
  * Modificador final em uma variável
    * Variável  de tipo primitivo
    * Objeto 
  * Modificador final em um atributo
    * Atributo primitivo
    * Objeto 
  * Modificador final em um método
  * Modificador final em uma classe
* Objeto imutável
  * Definição
  * Aplicações
  * Como criar um objeto imutável
  * Como modificar um objeto imutável 
* Tipos Genéricos
  * Definição
     * Representação de tipos genéricos na UML
  * Criação de classes com tipos genéricos
  * Inicialização de objetos com tipos genéricos  
* Testes Unitários
  * TDD
  * JUnit
    * Adicionar JUnit no projeto Java
  * Teste assertEquals
  * Teste assertTrue/assertFalse
  * Teste assertNull/assertNull
  * Teste assertArrayEquals  
  * Teste fail
  * Teste capturar uma exception
* JDBC
  * Definição
  * Driver de conexão 
  * Como adicionar o driver de conexão no projeto Java
  * Criação de uma conexão com o banco de dados
    * Classe DataManager
    * String de conexão
      * Banco SQLite
      * Banco MySql
      * Banco Postgre 
    * Classe Connection
  * Enviar instruções SQL
    * Classe Statement
    * Classe PreparedStatment   
  * Consultar registros no banco de dados
    * Classe ResultSet
    * Obter um registro
    * Obter uma coleção de registros
  * Bloco de instruções try-with-resources
  * Captura de exceções
    * Driver não encontrado
    * Conexão inválida
    * Tabela não encontrada
    * Registro não encontrado
    * Erro ao inserir/atualizar
    * Erro ao consultar
  * Design Patterns
    * Singleton Factory para criação de conexões   
      * Representação na UML
    * DAO para manipular dados de uma tabela   
      * Representação na UML

## Listas de Exercícios

[SCHEIBEL, Glaucio. Exercícios de Programação](https://github.com/glaucioscheibel/exercicios)

[Beecrowd](https://www.beecrowd.com.br/judge/pt/)

[Leetcode](https://leetcode.com)

[HackerRank](https://www.hackerrank.com)

[Exercism](https://exercism.org/tracks/java)



## Referências Bibliográficas

FURGERI, SÉRGIO. Java 8 Ensino Didático: Desenvolvimento e Implementação de Aplicações. Saraiva Educação SA, 2018.

Schildt, Herbert. Java para iniciantes. Bookman Editora, 2015.

Finegan, Edward, and Robert Liguori. OCA Java SE 8: Guia de Estudos para o Exame 1Z0-808. Bookman Editora, 2018.

Bloch, Joshua. Java Efetivo: 3a edição. Alta Books Editora, 2019.

Martin, Robert C. Código limpo: habilidades práticas do Agile software. Alta Books, 2019.

Fowler, Martin. UML Essencial: um breve guia para linguagem padrão. Bookman editora, 2014.
