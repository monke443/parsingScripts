Quick scripts to parse SharpView output for users/groups/systems.

Input for Powerusers command: "Get-DomainUser -Properties userprincipalname,memberof"
Input for Powercomputer command "Get-DomainComputer -Properties name,operatingsystem"


### Example input: 
```
memberof                       : {CN=dev,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Janet.Richards@cowmotors-int.com
memberof                       : {CN=dev,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Jordan.Edwards@cowmotors-int.com
memberof                       : {CN=dev,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Arthur.Smith@cowmotors-int.com
memberof                       : {CN=dev,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Clive.Hurst@cowmotors-int.com
memberof                       : {CN=dev,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Irene.Rose@cowmotors-int.com
memberof                       : {CN=hr,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Ronald.Jones@cowmotors-int.com
memberof                       : {CN=hr,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Mandy.Phillips@cowmotors-int.com
memberof                       : {CN=it,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Terence.Ford@cowmotors-int.com
memberof                       : {CN=it,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Sandra.Webster@cowmotors-int.com
memberof                       : {CN=it,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Philip.Shah@cowmotors-int.com
memberof                       : {CN=it,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Brian.Cole@cowmotors-int.com
memberof                       : {CN=it,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Harriet.Howard@cowmotors-int.com
memberof                       : {CN=it,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Bernard.Arnold@cowmotors-int.com
memberof                       : {CN=it,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Abigail.Lewis@cowmotors-int.com
memberof                       : {CN=it,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Deborah.Smith@cowmotors-int.com
memberof                       : {CN=management,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Vincent.Shah@cowmotors-int.com
memberof                       : {CN=management,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Laura.Thomas@cowmotors-int.com
memberof                       : {CN=management,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Eric.Smith@cowmotors-int.com
memberof                       : {CN=management,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Gavin.Williams@cowmotors-int.com
memberof                       : {CN=management,CN=Users,DC=cowmotors-int,DC=com}
userprincipalname              : Jay.Bailey@cowmotors-int.com
```

### Example output:
```
Arthur.Smith -> dev
Clive.Hurst -> dev
Nicole.Lewis -> dev
Ronald.Smith -> dev
Sam.Swift -> dev
Wendy.White -> dev
Malcolm.Richards -> hr
Mandy.Phillips -> hr
Owen.George -> hr
Ronald.Jones -> hr
Sean.Pearce -> hr
Trevor.Sheppard -> hr
Abigail.Lewis -> it
Bernard.Arnold -> it
Lynne.Hughes -> it
Philip.Shah -> it
Sandra.Webster -> it
Terence.Ford -> it
Bradley.Foster -> management
Eric.Smith -> management
Wendy.Burns -> management
Andrea.Davies -> sales
Carol.West -> sales
Elizabeth.Walker -> sales
Holly.Graham -> sales
Nigel.Marshall -> sales
Ricky.Ward -> sales

```
