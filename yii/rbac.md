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

| Interface | BaseManager |
|-----------|-------------|
| add       |             | 
| remove    | |
| update | |
| getRole | |
| getRoles | |
| getRolesByUse | |
| getChildRoles | |
| getPermission | |
| getPermissions | |
| getPermissionsByRole | |
| getPermissionsByUser | |
| getRule | |
| getRules | |
| canAddChild | |
| addChild | |
| removeChild | |
| removeChildren | |
| hasChild | |
| getChildren | |
| assign | |
| revoke | |
| revokeAll | |
| getAssignment | |
| hasAssignments  | |
| getAssignments  | |
| getUserIdsByRole | |
| removeAll        | |
| removeAllPermissions | |
| removeAllRoles    | |
| removeAllAssignments | |
|----------------------|----------|
