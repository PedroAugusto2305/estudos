# 1. Lógica Formal

## 1.1 Sentenças, Representação Simbólica e Tautologias

- Uma sentença (ou proposição) é uma frase que pode ser apenas verdadeira ou falsa.

**Exemplo:**
1. Dez é menor que sete. (é uma sentença porque é falsa)
2. Como vai você? (é uma pergunta, não pode ser considerado nem verdadeiro nem falso)

#### Conectivos e Valores-Verdade

- Conectivos **e** (∧) chamada também de conjunção, **ou** (∨) chamada também de disjunção.
- "Se sentença 1, então sentença 2", A denota a sentença 1 e B denota a sentença 2, então a sentença composta deve ser denotada por A ⟶ B *(A implica B)*, a seta (⟶) é o conectivo lógico de **implicação** e indica que a verdade de A implica ou leva à verdade de B.
    - Exemplo: a sentença "Fogo é uma condição necessária para fumaça", pode ser reformulada para "Se há fumaça, então há fogo" ou seja é o mesmo que A ⟶ B ou B ⟶ A, A implica em B, Se B então A.
- Conectivo de **equivalência** é denotado pelo símbolo (↔). A expressão A ↔ B é a abreviação de (A ⟶ B) ∧ (B ⟶ A). Essa sentença pode ser lida da seguinte forma: "A se, e somente se, B".
- Esses conectivos são chamados convectivos Binários. pois unem duas expressões a fim de produzir uma terceira.
- A negação é um *conectivo unário* pois atua em uma única expressão para produzir outra. A negação de A ou A' pode ser lida como "não A" ou "A é falsa" ou "A não é verdade"

Assim como em linguagens de programação, devemos seguir algumas *regras de sintaxe* (regras sob as quais as cadeias são válidas), por exemplo:
- A))∧ ∧ ⟶ BC não é uma cadeia válida.
- Expressões que formam cadeias válidas são chamadas de **fórmulas bem-formuladas** ou **wffs (well-formed formulas)**. A fim de reduzir o número de parênteses necessários em uma wff, estipulamos uma ordem na qual os conectivos são aplicados. Esta "ordem de precedência" é:
1. Conectivos dentro de parentêses, dos mais internos para os mais externos.
2. ' (negação)
3. ∧∨ (conjunção e disjunção)
4. ⟶ (implicação)
5. ↔ (equivalência)

Isto significa que a expressão *A ∨ B'* significa *A ∨ (B')* e não *(A ∨ B)'*. Analogamente, *A ∨ B ⟶ C* siginica *(A ∨ B) -> C* e não *A ∨ (B ⟶ C)*

- O número total de linhas de uma tabela-verdade pode ser descrito por 2ⁿ

#### Tautologias

- Uma wff *(A ⟶ B) ↔ (B' ⟶ A')*, cujos valores-verdade são sempre verdadeiros é chamada de **tautologia**. 
- Uma wff como *(A ∧ A') ⟶ (B ∨ B')*, cujos valores-verdade são sempre falsos é chamda de uma **contradição**.
- Quando uma wff composta na forma *P ↔ Q* é uma tautologia, como no primeiro exemplo, os valores-verdade de P e Q conseferem todas as colunas da tabela-verdade. Neste caso, *P* e *Q* são chamadas de **wffs equivalentes** e denotadas por *P ⇔ Q*. Desta forma *P ⇔ Q* indica um fato, a saber: a wff particular *P ↔ Q* é uma tautologia.
- 