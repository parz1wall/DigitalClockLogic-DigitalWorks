<h1 align="center">DigitalClockLogic-DigitalWorks</h1>

<p align="center"> Esse projeto... </p>

## Tabela de conteúdos
<!-----ts----->
  * [sobre](#sobre)
    * [instalação](#instalação)
    * [Funcionalidades](#instalação)
  * [funcionamento](#funcionamento)
    * [Estrutura Digital](#funcionamentoDigital)
    * [Contadores Assincornos](#contadores-Assincronos)
 
  
  



# sobre
<P>Como todo desenvolvedor iniciante, um dos primeiros estudos é o raciocínio lógico. Assim como em trabalhos escolares e práticas de raciocínio lógico, o desafio foi criar um relógio 100% digital utilizando apenas flip-flops, portas lógicas e números binários.</P>

<br>


## instalação

```bash
1- Faça o download do simulador Digital Works
$ Arquivo: _______

3- Faça o download do projeto
$ Arquivo: _______

4- Abra o projeto utilizando o simulador
```
<br>

## Funcionalidades

- [x] Start/Stop
- [x] Clear
- [x] Adicionar horas e minutos
- [x] Exibição em formato AM/PM e 24 horas

# Funcionamento

<p>Cada módulo tem a função de contar até um valor específico. Por exemplo, os módulos dos segundos realizam a contagem de 0 até 59 segundos (60 valores). Após atingir o máximo da contagem, o módulo das dezenas dos segundos emite um pulso para o módulo das unidades dos minutos, adicionando um valor ao display de 7 segmentos. Os módulos dos minutos seguem o mesmo processo dos segundos. Após atingir o máximo da contagem, um pulso é enviado para o módulo das horas, aumentando assim as horas.

A contagem é armazenada em binário, onde cada flip-flop do circuito armazena um bit. Em seguida, cada sequência de bits é decodificada para ser apresentada nos displays de 7 segmentos.</p>

## Estrutura Digital 

<p>São empregados circuitos sequenciais, como os flip-flops, para armazenar os bits de cada contador.</p>

### O que é um circuito sequencial?

<p>Enquanto o bloco básico de um circuito combinacional é a porta lógica, nos circuitos sequenciais, o elemento fundamental é o latch ou o flip-flop (circuito biestável). A principal vantagem dos circuitos sequenciais é sua capacidade de memória.

Os latches ou flip-flops são compostos por portas lógicas (NAND ou NOR). A interconexão desses flip-flops resulta em circuitos lógicos sequenciais utilizados para armazenamento de dados, temporização, contagem e sequenciamento.

Circuitos lógicos sequenciais são caracterizados pela realimentação das saídas para as entradas, conhecida como estado interno. Isso faz com que as condições atuais das entradas e do estado interno determinem a condição futura da saída.</p>

<p align="center">
  <img alt="Readme" title="Readme" src="./imagens/Capturar.PNG"/> 
 </p>

<br></br>
 
 ### FLip-Flop JK

<br></br>

 <p align="center">
  <img alt="Readme" title="Readme" src="./imagens/3.PNG"/> 
 </p>

<br></br>

## Contadores Assíncronos 

<p>Contadores são diversos Flip-flop ligados entre eles, onde cada flip-flop vai armazenar um bit do nosso valor numérico. </p>

<p align="center">
  <img alt="Readme" title="Readme" src="./imagens/4.PNG"/> 
 </p>

<br></br>

<p>No exemplo, podemos contar até o número 15, o que equivale a 2^4 (16 valores de 0 a 15).

A cada pulso do nosso clock "CP0", ocorre uma alteração no estado do primeiro Flip-Flop JK. Assim, ao iniciar, temos 0000; após o primeiro pulso, obtemos 0001; depois 0010; e assim por diante, até atingir o máximo, que seria 1111.</p>

<br>

### Contador modulo 6 e contador BCD 

















