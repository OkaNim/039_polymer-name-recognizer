Polymer names such as 'poly(ethylene oxide)' and 'PEO' can be recognized.<br>
Polymer sample codes such as 'P1' can be also recognized.<br>
<br>
<br>
## How to use
Please create the script such as 039_test.py in /src and run.<br>
```
python 039_test.py
```
<br>
----- 039_test.py -----<br>
import src_039_recognize_polymer_name_240426 as src_039<br>
<br>
<br>
toks = ["in", "polystyrene-block-poly", '(', "ethylene", "oxide", ')', '(', "PS-b-PEO", ')', "bottlebrush", "block", "copolymers", '(', "BBCP", ')', "upon", "The", "BBCPs", "are", "soluble", "in", "organic", "solvents", "."]<br>
tags = src_039.main(toks)<br>
<br>
<br>
print("\ntags\n", tags)<br>
print("\n\n")<br>
-------------------<br>
<br>
<br>
The BIOES tags are outputted for every token as follow:<br>
tags<br>
 ['O', 'B', 'I', 'I', 'I', 'E', 'O', 'S', 'O', 'O', 'O', 'O', 'O', 'S', 'O', 'O', 'O', 'S', 'O', 'O', 'O', 'O', 'O', 'O']<br>
<br>
<br>
