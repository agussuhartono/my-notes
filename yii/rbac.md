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

| Interface            | BaseManager      | DbManager      |
|----------------      |----------------  |-----------     |
| add                  | add              |                |
| remove               | remove           |                |
| update               | update           |                |
| removeAll            |                  | removeAll      |
| assign               |                  | assign         |
| revoke               |                  | revoke         |
| revokeAll            |                  | revokeAll      |
|                      |                  |                |
| getRole              | getRole          |                |
|                      | # isRole         |                |
| getRoles             | getRoles         |                |
| getRolesByUser       |                  | getRolesByUser |
| getChildRoles        |                  | getChildRoles  |
|                      | setDefaultRoles  |                |
|                      | getDefaultRoles  |                |
|                      | getDefaultRoleInstances |         |
| removeAllRoles       |                  | removeAllRoles |
|                      |                  |                |
| getPermission        | getPermission    |                |
| getPermissions       | getPermissions   |                |
| getPermissionsByRole |                  | getPermissionsByRole            |
| getPermissionsByUser |                  | getPermissionsByUser            |
|                      |                  | # getDirectPermissionsByUser    |
|                      |                  | # getInheritedPermissionsByUser |
| removeAllPermissions |                  | removeAllPermissions            |
|                      | # isPermission   |                |
|                      |                  |                |
| getRule              |                  | getRule        |
| getRules             |                  | getRules       |
|                      | _addRule_        | # addRule      |
|                      | _removeRule_     | # removeRule   |
|                      | _updateRule_     | # updateRule   |
|                      | createRule       |                |
|                      | # executeRule    |                |
|                      | # isRule         |                |
|                      |                  | removeAllRules |
|                      |                  |                |
| canAddChild          |                  | canAddChild    |
| addChild             |                  | addChild       |
| removeChild          |                  | removeChild    |
| removeChildren       |                  | removeChildren |
| hasChild             |                  | hasChild       |
| getChildren          |                  | getChildren    |
|                      |                  |                |
| getAssignment        |                  | getAssignment  |
| hasAssignments       |                  |                |
|                      | # hasNoAssignments |              |
| getAssignments       |                  | getAssignments |
| removeAllAssignments |                  | removeAllAssignments |
|                      |                  |                |
|                      | _getItem_        | # getItem      |
|                      | _getItems_       | # getItems     |
|                      | _addItem_        | # addItem      |
|                      | _removeItem_     | # removeItem   |
|                      | _updateItem_     | # updateItem   |
|                      | # isItem         |                |
|                      |                  | # populateItem         |
|                      |                  | removeAllItems         |
|                      |                  |                        |
| getUserIdsByRole     |                  | getUserIdsByRole       |
|                      |                  |                        |
|                      | # createItemRuleIfNotExist |              |
|                      |                  |   userHasPermission    |
|                      |                  | # checkAccessFromCache |
|                      |                  | # checkAccessRecursive |
|                      |                  |                        |
|                      |                  |                        |
|                      |                  | # getChildrenList      |
|                      |                  | # getChildrenRecursive |
|                      |                  | # detectLoop           |
|                      |                  |                        |
|                      |                  | invalidateCache        |
|                      |                  | loadFromCache          |
|                      |                  | - isEmptyUserId        |








