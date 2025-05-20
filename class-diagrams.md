# Diagramme de classe
```bash
+----------------------+
| NomClasse |
+----------------------+
| - attribut1 : Type |
| - attribut2 : Type |
+----------------------+
| + méthode1() : Type |
| + méthode2() : Type |
+----------------------+
```

- `+` → public
- `-` → private
- `#` → protected
- `: Type` → type de retour ou type d’attribut

## Relations entre les classes 
|Type de relation|Symbole UML|Explication|
|:---|:---|:---|
|Association|simple trait `──`|Une classe utilise une autre|
|Dépendance|trait pointillé `--->`|Une classe dépend d’une autre|
|Aggregation|trait pointillé `◊──`|Une classe utilise une autre et peut la supprimer|
|Héritage|flèche creuse `──▷`|Classe enfant hérite d’une classe mère|
|Composition|trait pointillé `◆──`|Une classe contient obligatoirement l’autre (fort lien)|