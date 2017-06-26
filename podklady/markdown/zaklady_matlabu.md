# Základy Matlabu
## Podmínka IF
Následuje příklad na kterém je demonstrováno jak využívat *if, else, elif* v Matlabu.
```Matlab
% conditions
add_all = false;
add_only_b = true;

% used variables
a = 3;
b = 2;
c = 1;

% "if, elseif, else" conditions
if add_all == true
    d = a + b + c
elseif add_only_b == true
    d = a + b
else
    d = a
end
```
