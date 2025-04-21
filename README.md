# 🔢 Somador Síncrono de 3 Bits - Logisim

Este projeto implementa um **somador síncrono de 3 bits** usando o simulador **Logisim**. O circuito soma dois números de 3 bits, armazena o resultado em um registrador sensível a clock, e exibe a saída em um display de 7 segmentos.

## 📚 Descrição do Projeto

### Componentes do circuito:

![image](https://github.com/user-attachments/assets/af6df517-8b7d-4d6f-9829-2225c7371302)


1. **Somador de 3 Bits**
   - Um meio somador (Half Adder - HA) para o bit menos significativo (LSB)
   - Dois somadores completos (Full Adders - FA) para os bits restantes

2. **Registrador de 3 Bits**
   - Implementado com 3 Flip-Flops tipo D
   - Armazena o resultado da soma a cada transição positiva do clock

3. **Conversor de 7 Segmentos**
   - Decodifica o valor de 3 bits do registrador para exibição num display de 7 segmentos
   - Cada saída (a-g) é implementada com base em expressões booleanas simplificadas

## 🔁 Funcionamento

1. O usuário fornece dois números binários de 3 bits (A e B).
2. O somador calcula a soma A + B.
3. O resultado é enviado para um registrador de 3 bits.
4. A cada pulso de clock, o valor é armazenado no registrador.
5. A saída do registrador é conectada ao conversor de 7 segmentos, que exibe o resultado da soma.

## 🛠️ Requisitos

- [Logisim (clássico)](http://www.cburch.com/logisim/)
- [Logisim Evolution](https://github.com/logisim-evolution/logisim-evolution)

## 🧪 Como Executar

1. Abra o Logisim.
2. Carregue o arquivo `.circ` fornecido (ex: `3Bits V 01.circ`).
3. Insira valores binários de entrada para A e B.
4. Ative o clock para registrar a saída da soma.
5. Observe o valor no display de 7 segmentos.

## 💡 Lógica do Conversor de 7 Segmentos

O conversor utiliza expressões booleanas simplificadas para cada segmento do display com base na tabela verdade dos valores de 0 a 7.

Exemplo para o segmento `a`:

