Spam filters analyze the text of emails & classify them into Spam & Ham
## SpamAssassin Features
- Mentions Generic Viagra
- Online Pharmacy
- Mentions millions of dollar
- Phrase: impress...girl
- From: starts with many numbers
- Subject is all CAPITALS
- [[2024 Semester 1/COMPSCI345 - Human-computer Interaction/Hypertext Markup Language (HTML)|Hypertext Markup Language (HTML)]] has a low ratio of text to image area
- 100% guaranteed
- Claims you can be removed from the list
- 'Prestigious Non-Accredited Universities'
#compsci361example ![[Pasted image 20240429133740.png]]

## Aim
We want it as a [[Supervised Learning]] task because things are becoming better, we don't want to constantly create new rules all time

## [[Spam Filtering]] as [[Supervised Learning]]
Collect a large number of e-mails, get users to label them
![[Pasted image 20240429133849.png]]
You can apply [[Linear Regression]], [[classification]], etc.
- ($\huge y\tiny {i}\normalsize = 1$):
	- if email $i$ is $spam$
- ($\huge y\tiny {i}\normalsize = 0$):
	- if email $i$ is $not\ spam$
- Extract features of each email ([[bag-of-words]]) - similar to [[Shallow NLP]]
	- ($\huge x\tiny {ij}\normalsize = 1$):
		- if word/phrase $j$ is in email $i$
	- ($\huge x\tiny {ij}\normalsize = 0$):
		- if word/phrase $j$ is not in email $i$
## Feature Representation for [[Spam Filtering]]
Are there better features than [[bag-of-words]]?
- We can add [[bigrams]]