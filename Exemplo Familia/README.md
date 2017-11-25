# Família
Para a base de dados família, irei mostrar alguns comandos para descobrir quem é pai de quem, quem é irmão ou até mesmo quem é avô e neto.

## Árvore Genealógica
![Árvore Genealógica](familia.PNG)

### Pais
gerou(kelly, lucas). <br />
false. <br />
gerou(kelly, maria). <br />
true. <br />

### Buscar todos os filhos de um pai
gerou(cleber, X). <br />
X = maria ; <br />
X = bruna. <br />
É obrigatório que a constante "X" esteja escrito em maiuscula. Como essa consulta pode gerar vários resultados, click no ponto e virgula para ir mostrando todos os resultados da consulta.

### Buscar os pais de um filho
gerou(X, maria). <br />
X = kelly ; <br />
X = cleber. <br />

### Verificar se um é irmão do outro
gerou(X, julia), gerou(X, pedro). <br />
X = maria . <br />
No caso de uma dupla verificação que nem esse, a virgula é como se fosse o "AND" na programação, ou seja, para que um seja irmão do outro as duas preposições tem que ser verdadeiras.

### Buscar os avós de um neto
gerou(X, Y), gerou(Y, pedro). <br />
X = kelly , <br />
Y = maria ; <br />
X = cleber , <br />
y = maria . <br />
A Lógica para descobrir quem são os avós são assim: X -> Y -> pedro, ou seja, X gerou Y e Y gerou pedro. Logo os avós de pedro são todos os resultados de X.



