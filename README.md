# Curso de desenvolvimento web com ES6, Typescript e Angular 4

### Arrow Function  
* Por que usar ?  

### TypeScript  
* O que é ?  
Atua como uma expansão da linguagem javascript. Com o TypeScript podemos escrever nossos códigos com inferência de tipo, também fornece suporte a criação de classes e interfaces. 

* Inferência de tipos  
let mensagem: string = 'Seja bem vindo'  
let quantidade: number = 10  
let estudandoAngular: boolean = true  
let listaDeFrutas: Array<string> = ['Uva', 'Banana', 'Abacaxi']  
let notasDasProvas: Array<number> = [7, 5, 8, 9]

### Orientação a Objetos com TypeScript  
* O que é ?  
Tem como principal objetivo trazer objetos da vida real para programação

* Classes x Objetos  
Classe define características de um objeto. Geramos objetos a partir de classes

* Atributos x métodos  
Atributos são características e métodos são ações/comportamentos

* Criando e instanciando classes
```js
class Carro {
    private modelo: string
    private numeroDePortas: number
    private velocidade: number = 0
    
    constructor() {
        
    }

    public acelerar(): void {
        this.velocidade += 10
    }

    public parar(): void {
        this.velocidade = 0
    }

    public velocidadeAtual(): number {
        return this.velocidade
    }
}
```

* Constructor  
Mesmo que não esteja implicitamente escrito na classe o interpretador procura por ele, se não acha simplesmente ignora.
O constructor é responsável por receber os parâmetros enviados no momento de instanciação da classe

* Interface  
* O que é ?  
Funcionam como contratos. Definem métodos e atributos que devem ser implementados nas classes.

* Criando Interface
```js
export interface IConcessionaria {
    fornecerHorariosDeFuncionamento(): string
}
```

* Generics  
* O que é ?  
Permite que componentes, classes ou métodos sejam reutilizáveis.  

* Exemplo:  
```js
export interface IAdd<Type> {
    add(object: T): boolean
}

import { IAdd } from './IAdd'

export class Add<T> implements IAdd<T> {
    add(object: T): boolean {
        return 'Adicionado com sucesso.'
    }
}
```



