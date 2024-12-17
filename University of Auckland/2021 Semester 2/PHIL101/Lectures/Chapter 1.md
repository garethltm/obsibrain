---
title: Chapter 1
updated: 2021-09-21T06:05:21.0000000+12:00
created: 2021-07-19T17:45:00.0000000+12:00
---

Chapter 1
Monday, 19 July, 2021
1:45 PM

21 July (Lecture 1)
<u>What is Truth?</u>
1 - True
0 - False

ꓥ - AND
| A   | B   | A ꓥ B |
|-----|-----|-------|
| 1   | 1   | 1     |
| 1   | 0   | 0     |
| 0   | 1   | 0     |
| 0   | 0   | 0     |

¬ - NOT
*Example:*
A - I am a cat
¬ A - I am not a cat
| A   | ¬ A |
|-----|-----|
| 1   | 0   |
| 0   | 1   |

→ - IF A then B

↔ - IFF -\> IF & only IF
*Example:*
IF A is TRUE then B is TRUE
IF A is FALSE then B is FALSE
| A   | B   | A → B | A ↔ B |
|-----|-----|-------|-------|
| 1   | 1   | 1     | 1     |
| 1   | 0   | 0     | 0     |
| 0   | 1   | 1     | 0     |
| 0   | 0   | 1     | 1     |

∨ - OR
⊻ - exclusive OR
| A   | B   | A ∨ B | A ⊻ B |
|-----|-----|---------------|-------|
| 1   | 1   | 1             | 0     |
| 1   | 0   | 1             | 1     |
| 0   | 1   | 1             | 1     |
| 0   | 0   | 0             | 0     |

![image1](../../../../resources/cdde30ed0d7949bc81b83d3772e1fe03.png)
26 July (Lecture 2)
<u>What is an ==argument==?</u>
- An ==argument== is a collection of statements. One, the ==conclusion==, should be logically supported by the rest, the ==premises.==
- What is logical support? For us, that the truth of premises is enough to guarantee the truth of the conclusion.
- We call this validity
- Example:
If it isn't a counter example (it is perfect) we can't look for a counter example & not find them - It is like saying I can't find my keys therefore they don't exist. We don't if we looked everywhere

An argument is valid iff there is no possibility that the conclusion is false when the premises are true

An argument is valid iff whenever the premises are true, so is the conclusion

Otherwise an argument is invalid

<u>Logical validity (VALIDITY)</u>
Logical validity means that when we are considering possibilities, we don't care about physics, common sense, word meaning, probability, experience, etc.

We only care what the premises say.

We care about some word meanings. Right now, these are:
AND, OR, IF, NOT

<u>Example Argument</u>
Andrew is human
Every human is green
Therefore Andrew is green
VALID

Andrew is in Auckland
Therefore Andrew is not in China.
INVALID - Auckland doesn't show any information about China. China could be a name of a car

Andrew is human.
Therefore Andrew is a mammal.
INVALID - not stated whether if a human is a mammal

Andrew is human.
If Andrew is human, he is kind
Therefore Andrew is kind.
VALID

Andrew is kind
If Andrew is human, he is kind
Therefor Andrew is human
INVALID

<u>What's next</u>
- Symbolising connectives
- Symbolising sentences
- Symbolising paragraphs

<u>Symbolisation</u>
How to find the Propositional Logic (PL) in an English sentence:
- We replace any simple proposition with a single capital letter by providing a "key" of useful propositions. E.g.,
  - R = It is raining
  - S = The sun shines
So "it is raining and the sun shines" becomes "R and S".
- We use the same key for an entire argument

<u>Connectives</u>  
We also need to represent the connectives. We have seen several types of connectives that join propositions. They roughly match some familiar words:
- Negations - "not", other negative words
- Conjunctions - "and", "but", "although", "also"
- Disjunctions - "or", "unless", "alternatively"
- Conditionals - "if", "when", "since"
- Bi-conditionals - "iff", "exactly when"

<u>Negation</u>
Negations include "not", the "n't" in "can't" and "don't", the "n" in "neither/nor", and many other subtle signs. The Negation symbol is "¬".

Rather than "not R", we write ¬R.

Negation does not add any parentheses.
What does ¬¬R mean?

<u>Conjunction</u>
Conjunctions include "and", "but", "although", "also", "while".
The Conjunction symbol is "ꓥ".

For "R and S", we write (R ꓥ S).

The parentheses are mandatory.
They prevent ambiguity.

<u>Disjunction</u>
Disjunction include "or", "alternatively", and "unless".
The Disjunction symbol is "v".

Rather than "R or S", we write (R v S).

The parentheses are mandatory.
Disjunctions are almost always inclusive
- Both disjuncts might be true.

<u>Exclusive Disjunction</u>
Sometimes a disjunction won't allow both options.
We only care if this is on logical, not physical or social grounds.

If we used exclusive disjunction we would write (R ⊻ S).

We will not be using this symbol much in this course.

<u>Conditionals</u>
Conditionals/ Implications include "if", "when", "since".
The Conditional symbol is "→", or 'arrow'.

For "if R then S", we write (R→S).

Conditionals are for predictions, causation, the results of rules/laws, and logical implication.
The order of the letters matters for conditionals.
![image2](../../../../resources/66f40e02fc894313a4c9f70c75ec9ce2.png)

![image3](../../../../resources/dd15de34dd024bb6b07a93e959014be4.png)

![image4](../../../../resources/6d6a2dc48f164a51bf900a722f11f757.png)

![image5](../../../../resources/f8ae82548af64f8d9834eff1354534af.png)

![image6](../../../../resources/d7b50be9c7d4413d8eb4b0aae48dd324.png)

![image7](../../../../resources/8a549970c36b4b1da4a85a2361423fa1.png)

Commas are generally showing where brackets start or stop.
![image8](../../../../resources/3fa14a8f91794bdbba8f5398bcbc88e3.png)
A different comma example
![image9](../../../../resources/b4ea465ee1d149c4855905e329b1a155.png)

<u>Realistic Symbolisation</u>
A paragraph is just a number of statements

Find the key atomic statements, then translate each sentence as its own formula

(sometimes it's easier to combine sentences into one formula, or split a sentence into multiple formulas, but generally start with one formula per statement)

Example:
![image10](../../../../resources/9b725cd25eca4e058a59aa6ef0c01568.png)
![image11](../../../../resources/20c4d419904344e5b6f4324d162cae40.png)
![image12](../../../../resources/ff36d7edd0d74b62a6e96b78d2e01e3f.png)
![image13](../../../../resources/9cb9d172003448749aa0101f65c9644f.png)
![image14](../../../../resources/5d204f6d6ab14c7fa03902b1cea435f7.png)

Example:
![image15](../../../../resources/330053c6a78440c0b2697accbe9f9be7.png)
![image16](../../../../resources/2398ff54efdb4303afc714b12bf7c64b.png)
![image17](../../../../resources/bdcf0050f97f4fd4905cd1c196064d51.png)

<u>Does ESP exist?</u>
![image18](../../../../resources/f8da77d42d6d4787be9dec8a91f4edfd.png)
![image19](../../../../resources/985c5c02ff1c4710a386411b13eb5c66.png)
28 July (Lecture 3)
Some Notions
An argument can have one of two logical statuses:
- Valid - it's impossible for the premises to be true and the conclusion false
- Invalid - not valid

A collection of statements can be related logically in one of two ways:
- Consistent - it's possible they can all be true at once
- Inconsistent - it's impossible they can all be true

A pair of Statements can be related logically in one of three ways:
- Equivalent - they have the same truth in every possibility
- Contradictory - they have different truth values in every possibility
- Independent - can be the same, can be different. (don't care about this term)

A Statement can have one of three logical statuses:
- Logical Truth - true in every possibility
- Logical Falsehood - false in every possibility
- Contingent - possibly true, possibly false

<u>Example:</u>
Are these statements consistent?
1.  Belinda is a cat
2.  Belinda can fly
TRUE

How about these two?
1.  I am a tree
2.  I am married to a cat
FALSE

Is this statement true? false? contingent?
1.  Either Jeremy likes ice cream, or they don't like ice cream, or they don't exist.
TRUE
2.  Jeremy likes ice cream, but they don't like cold food.
CONTINGENT

How about these two?
1.  Isabella is both happy and sad, at the same time.
CONTINGENT
2.  Isabella is in Auckland and in London at the same time.
CONTINGENT

Are these statements contradictory?
1.  Belinda is a cat
2.  Belinda is a dog
No

How about these two?
1.  Belinda is a cat
2.  Belinda is not a cat
Yes

Are these statements equivalent?
1.  All ravens are black - TRUE
2.  No non-black things are ravens - TRUE

How about these two?
1.  2 + 2 = 4 - ALWAYS TRUE
2.  This sentence contains words - ALWAYS TRUE

Is this statement true? False? Contingent?
1.  Every 3-sided square is a zebra - TRUE, there is no counter example of a 3-sided square that is not a zebra. No proof of a 3-sided square.
2.  No blue thing is colourless - TRUE

| p   | q   | p ꓥ q | p → q | q   |
|-----|-----|-------|-------|-----|
| 0   | 0   | 0     | 1     | 0   |
| 0   | 1   | 0     | 1     | 1   |
| 1   | 0   | 1     | 0     | 0   |
| 1   | 1   | 1     | 1     | 1   |

| p   | q   | p   | p ∨ q | q   |
|-----|-----|-----|-------|-----|
| 1   | 1   | 1   | 1     | 1   |
| 1   | 0   | 1   | 1     | 0   |
| 0   | 1   | 0   | 1     | 1   |
| 0   | 0   | 0   | 0     | 0   |

![image20](../../../../resources/a2e50ceafcce471bb076151cf48503d2.png)

![image21](../../../../resources/1b32259642ad4e8e8d8e71b5412813b8.png)
2 August (Lecture 4)
<u>Symbolising</u>
![image22](../../../../resources/7de042c6535d45489937974582cd75e5.png)

![image23](../../../../resources/d63af56390d648ceb4064394d0fac9fc.png)
![image24](../../../../resources/d53a2e436b6b452f8cc0d0651ba6c044.png)
Valid argument as first row is all True

Check for counter examples
![image25](../../../../resources/d0770b7aab66492a91effd30d13ee1e3.png)

![image26](../../../../resources/d8152a04e0d3499dad470aec67c8c44e.png)
![image27](../../../../resources/28798a22e93342d29272b26ddd4021fc.png)

![image28](../../../../resources/9caf312c57d44abe890626b3fc9e3d61.png)
![image29](../../../../resources/4a2d891af38645c7be05d4f90e79e91b.png)

![image30](../../../../resources/89ea084874664c85a7ab46df814326b9.png)

![image31](../../../../resources/13e73dd219ea47c2941db9affa1c882b.png)
![image32](../../../../resources/c94d3fe0b9d8438cb66f9428c5197ed7.png)

<u>Arguments</u>
![image33](../../../../resources/778534802faf44238cca3ca1f2f5b3e4.png)

<u>Valid</u>
![image34](../../../../resources/ca307f90bda2453a92f007ba490242fa.png)

<u>Counter-examples</u>
![image35](../../../../resources/80488dc1e7e24991b3d1069ab5da3022.png)
![image36](../../../../resources/b6a8a9fa620f4a4c8b72925ec5a421bf.png)
4 August (Lecture 5)
![image37](../../../../resources/0decbf9bb19643b0a4c1672947fe8198.png)
![image38](../../../../resources/c1b95eba91da41aeb9368bc4c1156fcb.png)
![image39](../../../../resources/8be3b4e4a66c4aabbbb5412c4902c4b2.png)

![image40](../../../../resources/73f92d47f0ba46d8b9c1b51409be1e29.png)

![image41](../../../../resources/cbf8826be28e434da84f5bda49280c48.png)
11/8/2021
![image42](../../../../resources/9af6c589062d4460a1b1952934f9251e.png)
![image43](../../../../resources/583fe65bc9c745abaa46af1108a92ac9.png)
![image44](../../../../resources/9a93936d84cb4da1aadb0efd49aadee0.png)
![image45](../../../../resources/48cff078425140cfac7cdbf296b18ba7.png)
![image46](../../../../resources/13b11f193f254dc986569d54ee95d5ad.png)
![image47](../../../../resources/4f7bcef1e24d4fe9b9aa79a3df6c266e.png)
![image48](../../../../resources/6cc3fb2552f44a998d2b195016574a77.png)
9 August (Lecture 6)
<u>Truth trees</u>
![image49](../../../../resources/c51ee27079f44c4fb8c0c910862c24f2.png)

![image50](../../../../resources/9a1820d1528245fe8312ab909b93f7be.png)
![image51](../../../../resources/58824ef461fc49299ed74caa8816081e.png)
OR
![image52](../../../../resources/7b04af64c3c046bb99467a3044c24ea6.png)
![image53](../../../../resources/e759c7eef98d4f429a35f80c091eab94.png)

![image54](../../../../resources/95f3fea562d049479983d00eb5661fc6.png)
![image55](../../../../resources/06326d3b3564461c901c45b900df11f9.png)

Counter-Examples
![image56](../../../../resources/c768dae328c44abe92e12e17613b2d1b.png)

![image57](../../../../resources/3e9cad8fbcbb46778a7fc0b669cc6891.png)
![image58](../../../../resources/8844f57968994eb495e5870e8de99e43.png)
![image59](../../../../resources/4e16aafec02849348fac5a4d7577dc5a.png)

![image60](../../../../resources/612ede0de119454490ee6b2da1fc2c6e.png)
![image61](../../../../resources/e7d521f3b2fa44e0a48918ea48c05db8.png)
![image62](../../../../resources/d7d0e07870f24a68a513f0b0c04f99be.png)

![image63](../../../../resources/1e98e5bb23994e0aadfef1f80af5a557.png)
![image64](../../../../resources/2fb0849739cc42f18aa75c8837d1fd31.png)
![image65](../../../../resources/ace00f0547eb4ca9802367610fe76cd6.png)

![image66](../../../../resources/6a11a0ee8cc642a2b9d85e68d6722f17.png)
![image67](../../../../resources/dcc611c381f8495581cf139b8e54d1f1.png)
![image68](../../../../resources/607defbd646649ffb6cc5d867c04a964.png)

<u>Summary</u>
![image69](../../../../resources/761ce210ed17485895c4554e45ab4711.png)

<u>Rules</u>
![image70](../../../../resources/219665526bdc4579bb7dd9a464101603.png)
11 August (Lecture 7)
![image71](../../../../resources/93be11a6438e438eae22a37e29353a9b.png)
![image72](../../../../resources/9827e62c475c4bdfbcbae7440dbc2a88.png)
![image73](../../../../resources/510994d987234b639f2565ee26660e86.png)

![image74](../../../../resources/049bac1106d54a6f8a1abebe65a79149.png)
![image75](../../../../resources/497a1cc6b335486ba4c70e5dd2cda372.png)

![image76](../../../../resources/b4de9c732078402c8fb0672eff1a855f.png)

![image77](../../../../resources/5acb3a2e556b40819e072ed9cb36065c.png)

![image78](../../../../resources/617271598ffb4db5b2d33476475b7f59.png)

![image79](../../../../resources/507369847c51446e9574e82252d99df6.png)

![image80](../../../../resources/4bab50e5d69a486ca385bf8407feba39.png)

Universe is expanding example:
![image81](../../../../resources/effdeb7ab52244e5b520635b8b993f5c.png)
![image82](../../../../resources/7f5f17bdb8c7457faf16ebca0c13f2c6.png)
16 August (Lecture 8)
![image83](../../../../resources/48746881e2f34e91a7fd326c43831389.png)

![image84](../../../../resources/31aa3313d03248cdbe5fa25c6fcb5cd7.png)
![image85](../../../../resources/258429060ce04c9598f92e80b6bb63a3.png)
![image86](../../../../resources/451c44aa2b824c708ad92cc6b31e1613.png)

![image87](../../../../resources/05cc2e39d9f44611b0e2eb2129fe53ef.png)
![image88](../../../../resources/789540387c504911bb9838911cad1cc8.png)
![image89](../../../../resources/9b8e4080f526482b9b046c07bc106922.png)

![image90](../../../../resources/a42c0cec2c1a4db9bd9ee02692b61e91.png)
![image91](../../../../resources/770665cc169f4cc79fed4faec163a81c.png)
![image92](../../../../resources/15c2b3cf731441da8491cd8c0082d1df.png)
![image93](../../../../resources/25c10cfc74bd4576a0eb9cc70189536b.png)
Check Predicates Notes:
18 August (Lecture 9)
![image94](../../../../resources/0129ed46fe9941559e69df61ddf6a525.png)
![image95](../../../../resources/87496c0bb4ec41df815f5e5c22012108.png)
Check Predicates Notes:

23 August (Lecture 10)
![image96](../../../../resources/231b143b983e4311a5b663b203bd0daf.png)

![image97](../../../../resources/9903f6ebaf6a4edb99a86d48fbcb9f1f.png)
![image98](../../../../resources/fb6e83964f52462aa0df3e93e508f147.png)

![image99](../../../../resources/25c9a3ed5fe34d619df8a21fa9ecab22.png)
![image100](../../../../resources/47b7d88d5c654b89875eb5bd761944ff.png)

25 August (Lecture 11) - optional
![image101](../../../../resources/96cccc4212054fd19565a39fc055f232.png)

![image102](../../../../resources/6680c6d32b254c9eac40c626bf4b2a14.png)

![image103](../../../../resources/c848e8044b274017a5e11c9940cb2124.png)

![image104](../../../../resources/197242519ce642a9944e54aaafc7b1d9.png)

Green
![image105](../../../../resources/7f09f878b5fd4a4b88e3867e4a915609.png)
Human
![image106](../../../../resources/f4ead2f90b84445292bc53c4b5bd704d.png)
Andrew
Yes, it is a Logical Truth

; is basically a sentence break

But can be written as AND

![image107](../../../../resources/db54fde97f154d828c8ac2300a7c35c0.png)

![image108](../../../../resources/696b6c891fba4962ab0f820b97f6085c.png)

![image109](../../../../resources/e9f4baf502734e60b078c0d99b8af2f8.png)

No row all premises true and conclusion false
Valid
Not a Logical truth

\<- p = 1, q = 0
COUNTER EXAMPLE
Invalid

Don’t pick arrows first as they branch

Tautology is all true
Contradiction is all false

Negated conclusion to proof argument is invalid

If see unless u can just change it to OR
