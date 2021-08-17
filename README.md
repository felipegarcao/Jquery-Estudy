#  O Que é Jquery ?

### Jquery é um Biblioteca do JavaScript Ja Foi Bastante Utilizada Antigamente, mas com a evolução do JavaScript caiu Bastante de Uso, Porem estou Estudando para Entender como ele Realmente Funciona, e Não ficar Completamente Perdido quando for Pegar Um Projeto que Utiliza Jquery.
<br />

# Primeiro Passos

- $("Elemento").hide() - Ira Esconder o Elemento Passado

- .show() - Exiba os elementos correspondentes.

```

$(".titulo").hide() // por Padrão ira estar Escondido

setTimeout(() => {

}, 2000)

```

- $.noConflict();  caso eu esteja Utilizando um FrameWork, Que o $ e retirar o possível conflitos. Apos Utilizar ele vai acontecer um Erro no console, porque é preciso passar Invés de $, Jquery(".titulo")....


# Eventos

- $(".titulo").click() - Para Eventos de Click
  
- $(".titulo").mouseenter() - Evento para Passar o Mouse Por Cima

- $(".titulo").mouseleave() - Evento de Saida, por Exemplo selecionei o titulo, vou passar o mouse por cima, apos retirar essa função Dispara

- $(".titulo").dbclick() - Para Capturar Eventos de Dois Click

# Animação

## Exemplos: 


~~~ javascript

  // efeitos Transaction Recebe como Parâmetro, Números, tags ja Definidas como por exemplo 'slow' e 'fast'

      $("#button1").click(() => {
        $("#square").fadeOut(3000); // ao clicar no elemento Selecionado ele Ira Sumir, com um Efeito de Transição
      }); 

      $("#button2").click(() => {
        $("#square").fadeIn(3000); // ao clicar no elemento ele ira aparecer com um efeito de transição
      }); 

      $("button").click(() => {
        $("#square").fadeToggle() // para usar os dois de cima, se não tiver aparecendo vai aparecer e vice versa
      })

      $("#button").click(() => {
        $("#square").fadeTo(2000, 0.6) // ele Recebe como Parâmetro a duração e quantidade de opacidade, ele funciona como findIn e o findout
      })

~~~