Design Review for Yii-RBAC


There some object that manage by RBAC Manager

Identity / User
Role
Permision
Rule

But on Yii2 RBAC Manager have method with bad name i.e add(), remove(), addChild(). 
On Yii3, the name seen more good.

Next, following topic is for Yii3   

The method list of RBAC Manager

| Interface      | BaseManager    | DbManager |
|----------------|----------------|-----------|
| add            | add            | |
| remove         | remove         | |
| update         | update         | |
| getRole        | getRole        | |
| getRoles       | getRoles       | |
| getRolesByUse  |                | |
| getChildRoles  |                | |
| getPermission  | getPermission  | |
| getPermissions | getPermissions | |
| getPermissionsByRole |          | |
| getPermissionsByUser |          | |
| getRule        |                | |
| getRules       |                | |
| canAddChild    |                | |
| addChild       | | |
| removeChild    | | |
| removeChildren | | |
| hasChild       | | |
| getChildren    | | |
| assign         | | |
| revoke         | | |
| revokeAll      | | |
| getAssignment  | | |
| hasAssignments | | |
| getAssignments | | |
| getUserIdsByRole | | |
| removeAll        | | |
| removeAllPermissions | | |
| removeAllRoles    | | |
| removeAllAssignments | | |
|                | _getItem_   | |
|                | _getItems_   | |
|                | _addItem_    | |
|                | _addRule_    | # addRule |
|                | _removeItem_ | |
|                | _removeRule_ |  |
|                | updateItem abstract| |
|                | updateRule abstract| |
|                | createRule | |
|                | setDefaultRoles |  |
|                | getDefaultRoles |  |
|                | getDefaultRoleInstances | |
|                | # executeRule | |
|                | # hasNoAssignments | |
|                | # isPermission |  |
|                | # isRole | |
|                | # isItem  | |
|                | # isRule  | |
|                | # createItemRuleIfNotExist  |  |
|                |               |   userHasPermission |
|                |               | # checkAccessFromCache |
|                |               | # checkAccessRecursive |
|                |               | # getItem |
|                |               | # addItem |
|                |               | # removeItem |
|                |               | # updateItem |


