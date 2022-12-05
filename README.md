# Compilador Tiny e TM
 Compiler Construction: Principles and Practice
 Kenneth C. Louden  

### 📋 Pré-requisitos
`gcc`
`make`

### :paperclip: Instalação
`sudo apt install gcc -y`
`sudo apt install make -y`
  
### :paperclip: Running
Com o repositório aberto no terminal 
`make all`

:clapper: [Vídeo Demonstrativo](https://github.com/maricimara98/compilador-Tiny-e-TM/blob/main/teste.mp4)

Exemplo para fins de demostração `teste.tny`
~~~
{ Caso de teste: }

read x; 

while (x < 5)
    write x;
	x := x + 1
endwhile
~~~

Primeiro compile no Tiny
`./tiny teste.tny`

Isso gerar um arquivo tm de mesmo nome.
Execute no TM

`./tm teste.tm`

~~~
TM  simulation (enter h for help)...
Enter command: g
~~~
Para caso de teste informe x = 1

~~~
Enter value for IN instruction: 1

OUT instruction prints: 1
OUT instruction prints: 2
OUT instruction prints: 3
OUT instruction prints: 4
HALT: 0,0,0
Halted
~~~

---
### Para visualizar todas as opções

~~~help

TM  simulation (enter h for help)...
Enter command: h
Commands are:
   s(tep <n>      Execute n (default 1) TM instructions
   g(o            Execute TM instructions until HALT
   r(egs          Print the contents of the registers
   i(Mem <b <n>>  Print n iMem locations starting at b
   d(Mem <b <n>>  Print n dMem locations starting at b
   t(race         Toggle instruction trace
   p(rint         Toggle print of total instructions executed ('go' only)
   c(lear         Reset simulator for new execution of program
   h(elp          Cause this list of commands to be printed
   q(uit          Terminate the simulation
Enter command:
~~~



---
por [Jucimara Pereira](https://gist.github.com/maricimara98) 😊
