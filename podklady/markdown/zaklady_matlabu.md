# Základy Matlabu
Poznámky:

* Řádek v Matlabu nezakončený středníkem vypíše svůj výsledek do konzole - to je výhodné pro zobrazení/schování průběžných výsledků.
* Pro komentář v Matlabu stačí napsat  *%*. V tomto tutoriálů jsou komentáře psány ve formě *%% komentář %* z důvodu koretního zvýraznění syntaxu.

## Podmínka IF
Následuje příklad na kterém je demonstrováno jak využívat *if, else, elif* v Matlabu.
```Matlab
%% condtions %
add_all = false;
add_only_b = true;

%% used variables %
a = 3;
b = 2;
c = 1;

%% "if, elseif, else" conditions %
if add_all == true
    d = a + b + c
elseif add_only_b == true
    d = a + b
else
    d = a
end
```
## Smyčka FOR
Následující ukázky se vztahují k rovnici
$\forall i \in \{2,\ldots,10\}.\ a_i = a_{i-1} + a_{i-2}$.
V následujícím příkladu jsou pomocí *for* smyčky dopočítány hodnoty *a* až do 10.
```Matlab
a = zeros(10,1); %% array for results %
a(1:2) = [1 1]; %% initial conditions %
for i = 3:10 
    a(i) = a(i-1) + a(i-2); %% do the stuff %
end
a %% print output %
```
## Smyčka WHILE
Následující ukázka se vztahuje ke stejné úloze jako ta pro smyčku FOR.
```Matlab
a = zeros(10,1); %% array for results %
a(1:2) = [1 1]; %% initial conditions %
i = 3;
while i <= 10
    a(i) = a(i-1) + a(i-2);
    i = i + 1;
end
a %% print output %
```



