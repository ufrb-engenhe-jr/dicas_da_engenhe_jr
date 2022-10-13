# JavaScript
<div width=900 align="center">
  <img margin="auto" height="300px" src="https://www.portalgsti.com.br/media/uploads/marcomascarenhas/javascript.png"/>
</div>

# PlayList

<a href="https://www.youtube.com/playlist?list=PLHz_AreHm4dlsK3Nr9GVvXCbpQyHQl1o1">Curso Grátis de JavaScript e ECMAScript para Iniciantes</a>: curso oferecido pela canal
curso em vídeo, com o professor Guanabara.

# Mais informações
- <a href="https://devdocs.io/javascript/"> Documentação da linguagem</a>
- <a href="https://www.programiz.com/javascript/online-compiler/"> Compilador de javascript</a>
- <a href="https://nodejs.org/en/download/">Baixar node</a>

# Códgo

      const soma = (a,b)=> a + b
      const sub = (a,b) => a - b

      var lista = [{name:"jeovane"}, {name:"Quele"},{name:"Vinicios"}, ]

      console.log(soma(1,2));
      console.log(sub(1,2));
      console.log(lista.map((e)=>e.name))
      

# Exercicios

<a href="https://github.com/ufrb-engenhe-jr/dicas_da_engenhe_jr/blob/main/Lista%201.pdf">Lista 1 </a>


# Solução 

2 - Calculadora: Criar uma função em javascript que receba dois valores e 
retorne o resultado da soma, subtração, divisão e multiplicação.


        const calculadora = (a,b)=>{
            return [a+b,a-b,a/b, a*b]
        }

        console.log(calculadora(1,2))
        

3 – Map (javascript): dado o array de objetos faça com que seja mostrado no 
console.log apenas o nome e idade dos usuários.


        const dado = [
         {
         id:"1",
         name:"Bartolomeu Santos",
         idade:36,
         created_at:"2022_03_1"

         },
         {
         id:"2",
         name:"Maria Mesote",
         idade:45,
         created_at:"2022_02_1"

         },
         {
         id:"1",
         name:"Juliana Silva",
         idade:36,
         created_at:"2018_03_1"

         }
         ]

         console.log(dado.map((e)=>{
             return e.name + " " + e.idade
         }))

4 – Usando o conhecimento da questão 2 e 3 faça: criar uma função 
que recebe o tipo da operação e um array “dado”, e retorne a média
das idades dos usuários e quantos usuários estão cadastrados.


          const response = (arr)=>{
              let mediaIdade = 0

              arr.map((e)=>{
                  mediaIdade+=e.idade
              })
              const contUser = arr.length
              mediaIdade = mediaIdade/contUser

              return "Media é "+ mediaIdade + " e a quantidade de user é "+contUser

          }


          const dado = [
           {
           id:"1",
           name:"Bartolomeu Santos",
           idade:36,
           created_at:"2022_03_1"

           },
           {
           id:"2",
           name:"Maria Mesote",
           idade:45,
           created_at:"2022_02_1"

           },
           {
           id:"1",
           name:"Juliana Silva",
           idade:36,
           created_at:"2018_03_1"

           }
           ]

           console.log(response(dado))

