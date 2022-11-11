<h1 align="center">:books: CYK Algorithm for CFG in CNF :books:</h1>


## Algorithm :pencil:
The CYK algorithm is a decision algorithm for CFG (context-free grammar) in CNF (Chomsky normal form). This determines whether or not give string of length n is generated by a CFG. The algorithm is applied by filling a table with n rows and n columns. The pseudocode is:

### -Input: 
A grammar G in CNF and a string of n terminals w = a1,a2 ... an.

### -Initialize:
j=1. For each i, 1 ≤ i ≤ n,

Xij = Xi1: set of variables A such that **A -> ai** is a production of G.
  
### -Repeat:
j = j + 1. For each i, 1 ≤ i ≤ n-j+1 

Xij = set of variables A such that **A -> BC** is a production of G, with B ∈ Xik and C ∈ Xi+k,j-k, considering all k such that 1 ≤ k < j - 1.
  
### -Until: 
j=n.

### -Output: 
w ∈ L(G) if and only if S ∈ X1n.


# Application Manual :notebook:
## First Screen

You have to follow this link: https://nuxt-examples-c5g9kwu80-alejandro945.vercel.app/

Then, you will see something like this
![imagen](https://user-images.githubusercontent.com/80568091/201343169-d0609682-f31d-4c32-b90a-053974c5e2e6.png)

In the field 'word', you have to put the chain of characters you want to process. **Example: abaab**

In the field 'amount of producers', you have to put the total number of producers that you have in the problem. **In this case we need 2**

**Make sure you fill these fields correctly** :heavy_exclamation_mark:

Finally, press the button to generate the table in the second screen.

## Second Screen

In this screen you have a table with the producers and the productions

![imagen](https://user-images.githubusercontent.com/80568091/201343858-3e0c8356-66dc-4eff-bd36-4295723b0f56.png)

To fill the table, you have to type the productions one by one, I mean, when you write one, press enter in your keyboard and then write the next

Once you finish, press the button ![imagen](https://user-images.githubusercontent.com/80568091/201345166-cdfc7840-a117-4c58-8ad8-0216bac13ac7.png)

**You have to receive a response of the algorithm**

In case that the chain belongs to the grammar, the response is:

![imagen](https://user-images.githubusercontent.com/80568091/201345330-cd7a6fb6-0941-43c5-98f2-341daddfb47f.png)

The table result show us the productions to use to generate the chain step by step. In the final column and the first row, we can see the final response

### In case that the chain doesn't belong to the grammar you will see this

![imagen](https://user-images.githubusercontent.com/80568091/201346640-c6fb64a0-a042-49b0-837c-84a556134451.png)




# Tools used to create this project:
* Vue.js
* TypeScript
* Ruby







  
  

  
  
 
