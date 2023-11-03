[[Automated Build]] enables [[Continuous Integration (CI)]]

Designed as part of [[eXtreme Programming (XP)]] practices

![[Pasted image 20231103145831.png]]![[Pasted image 20231103145854.png]]
>	#Example 
>	the example of prioritising a working mainline that a customer requires to make sure that the place can be moved in right away, right as other features that aren't as prioritised are being worked on

[[Continuous Integration (CI)]]] is a [[software development]] practice where members of a team integrate their work frequently, usually each person integrates at least daily (which potentially leads to multiple integrations per day).

Each integration is verified by an [[Automated Build]] (including [[Testing]]) to detect any integration errors as quickly as possible![[Pasted image 20231103150659.png]]
- Checkout code
- Write/change code
- Build & test locally
- Update (merge)
	- Retest if the mainline shows deviation from the working copy
- Commit changes
- Trigger [[Continuous Integration (CI)]]