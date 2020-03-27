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
| getRule        |                | getRule |
| getRules       |                | getRules |
| canAddChild    |                | canAddChild |
| addChild       |                | addChild |
| removeChild    |                | removeChild |
| removeChildren |                | removeChildren |
| hasChild       |                | hasChild |
| getChildren    |                | getChildren |
| assign         |                | assign |
| revoke         |                | revoke |
| revokeAll      |                | revokeAll |
| getAssignment        |          | getAssignment |
| hasAssignments       |          | getAssignments |
| getAssignments       |          | |
| getUserIdsByRole     |          | getUserIdsByRole |
| removeAll            |          | removeAll |
| removeAllPermissions |          | removeAllPermissions |
| removeAllRoles       |          | removeAllRoles |
| removeAllAssignments |          | removeAllAssignments |
|                | _getItem_      |           |
|                | _getItems_     | # getItems|
|                | _addItem_      |           |
|                | _addRule_      | # addRule |
|                | _removeItem_   |           |
|                | _removeRule_   | # removeRule |
|                | _updateItem_   |              |
|                | _updateRule_   | # updateRule |
|                | createRule     | |
|                | setDefaultRoles |  |
|                | getDefaultRoles |  |
|                | getDefaultRoleInstances     |  |
|                | # executeRule               |  |
|                | # hasNoAssignments          |  |
|                | # isPermission              |  |
|                | # isRole                    |  |
|                | # isItem                    |  |
|                | # isRule                    |  |
|                | # createItemRuleIfNotExist  |  |
|                |               |   userHasPermission |
|                |               | # checkAccessFromCache |
|                |               | # checkAccessRecursive |
|                |               | # getItem              |
|                |               | # addItem              |
|                |               | # removeItem           |
|                |               | # updateItem           |
|                |               | # populateItem         |
|                |               | getRolesByUser         |
|                |               | getChildRoles          |
|                |               | getPermissionsByRole   |
|                |               | getPermissionsByUser   |
|                |               | # getDirectPermissionsByUser     |
|                |               | # getInheritedPermissionsByUser  |
|                |               | # getChildrenList                |
|                |               | # getChildrenRecursive           |
|                |               | # detectLoop           |
|                |               | removeAllItems         |
|                |               | removeAllRules         |
|                |               | invalidateCache        |
|                |               | loadFromCache          |
|                |               | - isEmptyUserId        |








