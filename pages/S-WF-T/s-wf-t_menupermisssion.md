---
title: Steps for Test Menu Permission
keywords: Steps for Test Menu Permission
sidebar: s-wf-t_sidebar
permalink: security-workflow-task/steps-for-test-menu-permission.html
folder: S-WT-T
hide_sidebar: false
comments: false
---

# Steps for Test Menu Permission

Firstly entered row in **ApplicationSettings**.

Set **SettingKey=Appcode.menu like nclgmgr.menu**

Set **SettingValue=Menu permission keys from menu definition of application**.

*E.g.: ID_mnu1Student,ID_Student,ID_NewStuPerson*

>Note: if ApplicationSettings is empty, its means all keys are available.

**Step.1** Check DBrole Active or Not.

*Active:* At Least one row available in DBrole

*Not Active:* If DBrole is Empty

![](/images/menuperdbrole.png)

**Step.2** If Dbrole **not active** then (No Need to check Dbrole)

If User is **Superadmin** then:

![](/images/menupersuperadmin.png)

Showing all **Tenant + Admin** i.e. **(Admin Behave=T & S)** Level menu's which keys are entered in **SettingValue** in **Applicationsettings**.

![](/images/menuperadminmenu.png)

If User is **not Superadmin** then:

![](/images/menupernotsuperadmin.png)

Showing only **Tenant**  i.e. **(Admin Behave= T)** Level menu's which keys are entered in **SettingValue** in **Applicationsettings**.

![](/images/menupertenant.png)

**Step.3** If DBrole **active** then :( Now Check Dbrole first)

Now need to create DbRole, We can create dbroles like this:

![](/images/menupernewrole.png)

Now Check Roleid in Users Table

**Case.1:**
 
If **roleid =2** in users table then:

**(a)**. if User is **Superadmin** then

Showing all **Tenant+Admin** i.e. **(Admin Behave = T & S)** Level menu's which keys are entered in **Permissionlist** in **Dbrole** and **Applicationsettings** (if keys are define in Applicationsettings. 

![](/images/menuperrolesuoeradmin.png)

![](/images/menuperrolemanagment.png)

**(b)**.If User is not **Superadmin** then

Showing Only **Tenant** i.e. **(Admin Behave = T)** Level menu's which keys are entered in **Permissionlist** in **Dbrole** and **Applicationsettings** (if keys are define in Applicationsettings).

![](/images/menuperrolenotsuperadmin.png)

![](/images/menupermenugroup.png)

**Case.2:**
 
If **roleid =1** in users table then:

**(a)**.If User is **Superadmin** then

Showing **Tenant+Admin** i.e. **(Admin Behave = T & S)** Level menu's which keys are entered in **SettingValue** in **Applicationsettings**.

![](/images/menuperrolesuperadmin.png)

![](/images/menupermenugroup1.png)

**(b)**.If User is not **Superadmin** then

Showing Only **Tenant** i.e. **(Admin Behave = T)** Level menu's which keys are entered in **SettingValue** in **Applicationsettings**.

![](/images/menuperrolenotsuperadmin1.png)

![](/images/menupermenugroup2.png)








