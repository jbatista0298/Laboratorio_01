# Laboratorio_01
UTFPR - Sistemas Microcontrolados

Professor: Hugo Vieira Neto

Estudante: João Batista


EXERCÍCIO 3

1. Digitar código em Assembly do Exemplo 3
 
       ;Foi implementado na área de trabalho com o nome LAB1
   

2. Construa a aplicação e transfira o código executável resultante para o simulador.
   
       ;2.1 - Para torna o projeto ativo, pressione o botão direito sobre LAB1 e clique em "Set as Active".
   
       ;2.2 - Para construir a aplicação, pressione o botão direito sobre LAB1 e clique em "Make".
   
       ;2.3 - Para iniciar a simulação, Ctrl+D ou Clique no ícone verde "Download and Debug".
   

3. Abra a janela Registers 1 no simulador.

       ;Caso a janela não abra automaticamente, Entre no menu "View", em seguida "Register" e "Register1".


4. Execute o programa passo-a-passo no simulador, observando simultaneamente as janelas Register 1 e Disassembly

       ;Para realizar esse procedimento, defina algumas interrupções. Na janela Disassembly clique 
       ;ao lado das instruções em que deseja pausar. Para continuar pressione F5, ou no ícone "Go".
   
   
5. Para cada instrução executada observe na janela Registers 1:
   
   5.1 O resultado da operação no registrador Rd. Como valores negativos são codificados?

       ;Para identificação de valores negativos a função MOVS e MVNS são recomendada, pois alterão o estado das flags,
       ;no simulador o campo APSR da janela Register1, apresenta o N como identificação "Negative condition flag".
       
   5.2 O efeito da operação no registrador APSR (flags). É possível visualizar os estados individuais dos flags?
     
       ;Sim, no campo APSR temos as condições: N (Negative), Z (Zero), C (Carry), V (Overflow), Q e GE.
       
   5.3 O valor do registrador PC. Como o PC está relacionado à janela Disassembly?

       ;Está relacionado a segunda coluna do Disassembly, que refere-se ao endereço da instrução.

6. Observe na janela Disassembly, linha a linha:

   6.1 Os endereços da memória de código em que cada instrução foi alocada pelo ligador.
   
       ;MOV R0, #0x55         ---------> 0x40
       ;MOV R1, R0, LSL #16   ---------> 0x44
       ;MOV R2, R1, LSR #8    ---------> 0x48
       ;MOV R3, R2, ASR #4    ---------> 0x4c
       ;MOV R4, R3, ROR #2    ---------> 0x50
       ;MOV R5, R4, RRX       ---------> 0x54






