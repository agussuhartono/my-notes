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
| addChild | | |
| removeChild | | |
| removeChildren | | |
| hasChild | | |
| getChildren | | |
| assign | | |
| revoke | | |
| revokeAll | | |
| getAssignment | | |
| hasAssignments  | | |
| getAssignments  | | |
| getUserIdsByRole | | |
| removeAll        | | |
| removeAllPermissions | | |
| removeAllRoles    | | |
| removeAllAssignments | | |
|  | getItem abstract| |
|  | getItems abstract| |
|  | addItem abstract| |
|  | addRule abstract| |
|  | removeItem abstract| |
|  | removeRule abstract|  |
|  | updateItem abstract| |
|  | updateRule abstract| |
|  | createRule | |
|  | setDefaultRoles |  |
|  | getDefaultRoles |  |
|  | getDefaultRoleInstances | |
|  | executeRule protected | |
|  | hasNoAssignments protected | |
|  | isPermission protected |  |
|  | isRole protected | |
|  | isItem protected | |
|  | isRule protected | |
|  | createItemRuleIfNotExist protected |  |
| | | userHasPermission |
| | | checkAccessFromCache protected |

