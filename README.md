# CostAnalysis
This respository holds the raw compiled data for the experiments on cost analysis of logic encryption methods

## Benchmarks  
The following benchmarks were used for the analysis experiments.

|Combinational Circuits||Sequential Circuits|
|ISCAS '85 benchmarks||ITC '99 benchmarks|
|:--------------------:||:-----------------:|
|c432 ||b04|
|c499 ||b05|
|c880 ||b07|
|c1355||b11|
|c1908||b12|
|c2670||b13|
|c3540||b14|
|c5315||b15|
|c6288||b21|
|c7552||b22|

ISCAS '85 benchmarks were obtained from [http://www.pld.ttu.ee/~maksim/benchmarks/iscas85/verilog/](http://www.pld.ttu.ee/~maksim/benchmarks/iscas85/verilog/).  
ITC '99 benchmarks were obtained from [https://github.com/squillero/itc99-poli](https://github.com/squillero/itc99-poli).  

## Method naming convension  
The encryption methods are listed using the following naming convensions.

|Methods|Code|
|:------|:---|
|Random|RN|
|SLL|SL|
|LCB|CB|
|KeyDep|KD|
|AntiHT|HT|
|E2LEMI|EL|
|Cyclic|CR|
|SRCLock|RC|
|SARLock|SR|
|AntiSAT|NR|
|TTLock|TR|
|SFLL-HD<sup>h</sup>|FR|
|Encrypt flip-flop|EF|
|Chain based|CB|
|Deep State|DS|


## File description  
Each file corresponds to a single benchmark and contains two sheets -  
1. Area overhead
2. Power overhead

Each row in a sheet corresponds to an encryption method.  
Each column in a sheet corresponds to a key size. A total of 4 key sizes 32, 64, 128, and 256 were used.  
For each benchmark, cost (area/power), encryption method and key size, the entry corresponds to the overhead value (in percentage) over the unencrypted circuit.


## Contact
For questions, contact [Yasaswy Kasarabada](kasarayv@mail.uc.edu).



