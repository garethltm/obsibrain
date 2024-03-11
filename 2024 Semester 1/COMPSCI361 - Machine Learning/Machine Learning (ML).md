- Using computers to automatically detect patterns in data and use these to make prediction or decisions
- Most useful when
	- We want to automate something a human can do
	- We want to do things a human can't do (looking through 1TB of data)

>>[[Machine Learning (ML)]] is the field of study that gives the computer the ability to learn without being explicitly programmed
>
>>A computer is said to learn from experience E with respect to
>>	some class of task T and
>>	performance measure P,
>>if its performance at tasks in T, as measured by P, improved with experience E

#compsci361example
- Problem - Self-Driving Cars
	- T: Driving on public highway using vision sensors
	- P: Average distance travelled before an error/crash
	- E: A sequence of images and steering commands recorded while observing a human driver

## Applications
- learning patterns to recommend to the user

1. Spam Filtering
2. Credit card fraud detection
3. Product recommendation
4. Motion capture
5. OCR
6. Speech recognition
7. Face recognition
8. Object detection
9. Sports analytics
10. Medical imaging
11. Self-driving cars
12. Image annotation
13. Discovering new cancer subtypes
14. Protein folding prediction
15. Drug discovery
16. Chess/ GO/ Starcraft/ ...
17. ...

## Goal
- In [[Machine Learning (ML)]]:
	- What we care about is the test error
#compsci361example 
- The [[training error]] is practice on the exam
- The test error is the actual exam
Goal: Do well on actual exam but not the practice one

Memorization vs learning:
- Can do well on training data by memorizing it
- You have only learned if you can do well in new situations