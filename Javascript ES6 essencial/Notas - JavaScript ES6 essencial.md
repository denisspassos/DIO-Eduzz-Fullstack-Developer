# JavaScript ES6: Essencial

- TypeScript
    - Um superset de JavaScript. Adiciona funcionalidades que o JS não tem por padrão (interfaces, enuns, generics...). 
    - Dá pra fazer checagem de tipos (num construtor, por exemplo), visto que JS permite você enviar qualquer tipo de dado pra uma variável (tipagem fraca e dinâmica).

- Flow
    - Semelhante ao TS em relação à checagem de tipos. Como se fosse uma versão simplificada do TS.

## Funções de primeira classe e ordem maior
- Função de primeira classe: 
    - A função pode ser atribuída a uma variável ou a uma estrutura de dados;
    - Pode ser passada por argumentos;
    - Pode ser retornada por outras funções.

## Closure
- Também coonhecido como escopo léxico. 
- É a capacidade de uma função lembrar do ambiente em que ela foi criada.

## Currying
- Capacidade da função retornar uma (sub)função para cada parâmetro recebido.

## Hoisting
- A declaração da varíavel ou função é "subida/içada", você pode chamar ela antes de declará-la.
- Se fizer com váriável, de início dá undefined. 
- Se fizer com função, ela vai "subir" inteira e funcionar.

## Imutabilidade
- O valor da variável não se afeta pelas operações

## Tipos e variáveis

    // escopo global
    
    {
    // escopo de bloco
    }
    
    function test(){
    // escopo de função
    }

- var
- let:
    - Escopo de bloco
- const
    - Escopo de bloco