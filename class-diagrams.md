# Class Diagram  
```
+----------------------+
| ClassName            |
+----------------------+
| - attribute1 : Type  |
| - attribute2 : Type  |
+----------------------+
| + method1() : Type   |
| + method2() : Type   |
+----------------------+
```

- `+` → public  
- `-` → private  
- `#` → protected  
- `: Type` → return type or attribute type  

## Relationships between classes  
|Relation type | UML symbol | Explanation                     |  
|:-------------|:-----------|:--------------------------------|  
|Association   | simple line `──`     | One class uses another          |  
|Dependency    | dotted line `--->`   | One class depends on another    |  
|Aggregation   | dotted line `◊──`    | One class uses another and can delete it |  
|Inheritance   | hollow arrow `──▷`   | Child class inherits from parent class |  
|Composition   | dotted line `◆──`    | One class must contain another (strong link) |  

### Example:  
```
+----------------------+
|      Payment         |
+----------------------+
| - amount : double    |
+----------------------+
| + perform()          |
+----------------------+
           ▲
           |
+----------------------+         +-----------------------+
| CardPayment          |         | CashPayment           |
+----------------------+         +-----------------------+
| - cardNumber : String|         |                       |
+----------------------+         +-----------------------+
| + perform()          |         | + perform()           |
+----------------------+         +-----------------------+
```