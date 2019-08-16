# CostAnalysis
This respository holds the raw compiled data for the experiments on cost analysis of logic encryption methods

## Benchmarks  
The following benchmarks were used for the analysis experiments.

|Combinational Circuits<br>(ISCAS '85)|Sequential Circuits<br>(ITC '99)|
|:---:|:---:|
|c432 |b04|
|c499 |b05|
|c880 |b07|
|c1355|b11|
|c1908|b12|
|c2670|b13|
|c3540|b14|
|c5315|b15|
|c6288|b21|
|c7552|b22|

ISCAS '85 benchmarks were obtained from [http://www.pld.ttu.ee/~maksim/benchmarks/iscas85/verilog/](http://www.pld.ttu.ee/~maksim/benchmarks/iscas85/verilog/).  
ITC '99 benchmarks were acquired from [https://github.com/squillero/itc99-poli](https://github.com/squillero/itc99-poli).  

## Method naming convension  
The encryption methods are listed using the following naming convensions.

<table>
  <tr>
    <td colspan="2" align="center"><b>Combinational</b></td>
    <td colspan="2" align="center"><b>Sequential</td>
  </tr>
  </tr>
    <td align="center"><b>Methods</b></td>
    <td align="center"><b>Code</b></td>
    <td align="center"><b>Methods</b></td>
    <td align="center"><b>Code</b></td>
  </tr>
  <tr>
    <td>Random</td>
    <td>RN</td>
    <td>Random</td>
    <td>RN</td>
  </tr>
  <tr>
    <td>Logic Cone based</td>
    <td>CB</td>
    <td>Encrypt Flip-Flop</td>
    <td>EF</td>
  </tr>
  <tr>
    <td>SLL</td>
    <td>SL</td>
    <td>Chain based</td>
    <td>CB</td>
  </tr>
  <tr>
    <td>Key Interdependency</td>
    <td>KD</td>
    <td>Deep State</td>
    <td>DS</td>
  </tr>
  <tr>
    <td>Hardware Enlightening</td>
    <td>HT</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>E2LEMI</td>
    <td>EL</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Cyclic</td>
    <td>CR</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>SRCLock</td>
    <td>RC</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>SARLock</td>
    <td>SR</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>AntiSAT</td>
    <td>NR</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>TTLock</td>
    <td>TR</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>SFLL-HD<sup>h</sup></td>
    <td>FR</td>
    <td></td>
    <td></td>
  </tr>
</table>

Note - SR, NR, TR and FR are compound schemes with SL (k=32)


## File description  
Each file corresponds to a single benchmark and contains two sheets -  
1. Area overhead
2. Power overhead

Each row in a sheet corresponds to an encryption method.  
Each column in a sheet corresponds to a key size. A total of four key sizes (32, 64, 128, and 256) were used.  
For each benchmark, cost (area/power), encryption method and key size, the entry corresponds to the overhead value (in percentage) over the unencrypted circuit.


## Contact
For questions, contact [Yasaswy Kasarabada](kasarayv@mail.uc.edu).



