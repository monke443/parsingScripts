Quick scripts to parse SharpView output for users/groups/systems.

- Input for Powerusers command: "Get-DomainUser -Properties userprincipalname,memberof"
- Input for Powercomputer command "Get-DomainComputer -Properties name,operatingsystem"


### Example input users: 
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

### Example output users:
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

### Example input computers:
```
name                           : DC02
operatingsystem                : Windows Server 2019 Standard
name                           : DB01
operatingsystem                : Windows Server 2019 Standard
name                           : WEB01
operatingsystem                : Windows Server 2019 Standard
name                           : CLIENT03
operatingsystem                : Windows 10 Pro
name                           : CLIENT02
operatingsystem                : Windows 10 Pro
name                           : WEB03
operatingsystem                : Windows Server 2019 Standard
name                           : DEV02
operatingsystem                : pc-linux-gnu
name                           : DEV03
operatingsystem                : pc-linux-gnu
```


### Example output computers:
```
DEV02 -> pc-linux-gnu
DEV03 -> pc-linux-gnu
CLIENT02 -> Windows 10 Pro
CLIENT03 -> Windows 10 Pro
DB01 -> Windows Server 2019 Standard
DC02 -> Windows Server 2019 Standard
WEB01 -> Windows Server 2019 Standard
WEB03 -> Windows Server 2019 Standard
```
