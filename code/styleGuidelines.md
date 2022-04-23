## Server-side guidelines

***ALL SERVER SIDE CODE IS TO BE WRITTEN IN JAVA***

This policy might change in the future, but it remains for now.

It is reccomended that you follow [these Java conventions](https://www.oracle.com/technetwork/java/codeconventions-150003.pdf) 
with the following modifications:
  1. Tab is to be set to 4 spaces and to be used as the standard indent. Wherever the manual says to use
8 spaces, use two tabs. 
  2. Maximum line length is to be capped at 100 characters, including whitespae
  3. Use two lines between methods
  4. If you think it would improve readability, include a coment line of '=' with a section title to 
seperate methods of similar functionality, like below:
```java
//============ Setters and getters =============

/*code*/

//============ Ship Module Damage ==============
```
  5. If a control statmement (if, for, while, etc) only has one line in the braces, you may compress
it to one line like below:
```java
if (onFire) {extingquish();}

for (int i = 0; i < shipCount; i++) {ships[i].printStatus();}
```
  6. Point 5 applies to trivial setters and getters too. For trivial methods, put whatever space 
between them looks the cleanest,
```java
public void getHealth(){return health;}
public void takeDamage(int d){health -= d;}
```
  7. The point is to prioritize readability, so you may stray from these guidelines if you believe
it improves readability. Code style will be reviewed before a merge is accepted. 

## Client-Side guidelines

Clientside development is a bit further out, and I'm out of practice with HTML/CSS and whatever language 
we'll use to communicate with the server. For now, my only prescription is to follow whatever standard
style is reccomended for the language. 
