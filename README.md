# HDLbits_Countbcd
Build a 4-digit BCD (binary-coded decimal) counter. Each decimal digit is encoded using 4 bits: q[3:0] is the ones digit, q[7:4] is the tens digit, etc. For digits [3:1], also output an enable signal indicating when each of the upper three digits should be incremented.

# Entity: top_module 
- **File**: code_pratice.v

## Diagram
![Diagram]([top_module.svg](https://github.com/CJ2002002/HDLbits_Countbcd/blob/main/top_module.svg) "Diagram")
## Ports

| Port name | Direction | Type   | Description |
| --------- | --------- | ------ | ----------- |
| clk       | input     |        |             |
| reset     | input     |        |             |
| ena       | output    | [ 3:1] |             |
| q         | output    | [15:0] |             |

## Processes
- unnamed: ( @(posedge clk) )
  - **Type:** always

## Instantiations

- cnt_1: decade_cnt
- cnt_2: decade_cnt
- cnt_3: decade_cnt
- cnt_4: decade_cnt
