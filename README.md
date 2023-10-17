# carros
 import * as leitor from "readline-sycn"

/// exercicio de enunciados ////
   //// exercicio 1
   let menu: boolean = true 
   while(menu ){
      let option = leitor.question('Informe o numero de 1 a 3')
    switch(option)
       case 1: 
         console.log('mensagem 1');
        break;

       case 2: 
        console.log('mensagem 2');
         break;

        case 3: 
       console.log('mensagem 3 ');
          break;
   }
 //// exercicio 2 
    let menu: boolean = true 
    while(menu){
        let option: String = leitor.question("informe uma cor ou digite")
    switch(option){
        case 'Amarelo' ; 
        console.log('Amarelo se lembra  primavera');
        break;
          case' Vermelho'
        console.log('Vermeçha mr lembra verão');
       break;
         case 'Verde'
         console.log('Verde me lembra floresta');
        break; 
         case 'Branco' 
          console.log('Branco me lembra casamento');
        break;
          case 'Sair'
          console.log('Saindo! ');
         break;
          default:
            console.log('Cor não consta no sistema.');
           break;

    }
    }   
      /// exercicio novo ///
          /// exemplos///
        export class carro{   
            consumo: number;
            combustível: number = 0;
            marca: string; 
            modelo: string;
            ano: number;

      constructor (consumo:  number,  marca:  string ,  modelo:  string,  ano: number);

        this.consumo = consumo;
        this.marca = marca;
        this.modelo = modelo;
        this.ano = ano;
        this.combustível = 0;

        }

        viajar(km){
           let viajar = km / this.consumo 
           if(viajar < this.combustível){
            console.log("Não é possível fazer essa viagem, abasteça seu carro!");
         } else {
            this.combustível -= viajar
            console.log('Sobrou $(this.conbustível} litros de gasolina ');
           }
        }
        

        ///getCombustível///
        checarTanque(): void{
          console.log('seu taque está com $ {this.combustível} litros de gasolina ');
        }
           getValudes(): void{
            console.log('seu carro faz: ${this.consumo} por lito de gasolina . ');
            console.log('o modelo do seu carro é: ${this.modelo} ');
            console.log('a marca do seu carro é: ${this.marca} '); 
            console.log('o ano do seu carro é: ${this.ano} ');
           }





        
