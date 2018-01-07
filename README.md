# CNF-Resolution
Implements inference using Resolution, a proof by contradiction approach for Conjunctive Normal Form.

# Resolution

Resolution is a method of inference leading to a refutation theorem-proving technique for sentences in propositional logic  and first-order logic(FOL).

In other words, iteratively applying the resolution rule along with unification in a suitable way allows for inferencing whether a CNF statement is satisfiable or unsatisfiable.

Attempting to prove a satisfiable FOL statement as unsatisfiable may result in a nonterminating computation; this problem doesn't occur in propositional logic. Resolution works on statemets in Conjunctive Normal Form(CNF) and hence FOL statements are first converted to CNF.

Resolution is a complete and sound inference procedure because it works on CNF which is universal.

# Steps involved:

The overview of the whole process is as follows:

One query is picked at a time, it is negated and added to Knowledge base

Resolution inference is applied using the method of Set of Sets to prove the query by inferencing a contradiction.

# How to execute: 
Make sure Resolution.py and input.txt are in the same directory before running the script file. When you run the Resolution.py file, it reads input.txt and performs resoltion to prove the queries. The script generates output.txt which contains the True/False output for each query. True if a query can be infered from the Knowledge base and False if it cannot be.

# Input Format: 

NUMBER OF QUERIES<br>
QUERY 1<br>
...<br>
QUERY N<br>
NUMBER OF CNF SENTENCES IN THE KNOWLEDGE BASE<br>
CNF SENTENCE 1<br>
...<br>
CNF SENTENCE M<br>

where,<br>
Queries can be of the form: Father(John, Max)<br>
and CNF statements can be of the form : ~Parent(x,y) | Ancestor(y,z) | Ancestor(x,z)

# Output Format: 
For each query, the output denotes if that query can be inferred from the knowledge base or not, one query per line:<br>
ANSWER 1<br>
...<br>
ANSWER N<br>

where,<br>
each answer is either TRUE if it can be proved given the knowledge base, or FALSE if it cannot be.
