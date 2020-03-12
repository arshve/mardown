### Eg.
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
---

URL: 192.168.101.155/sf6
- Account: suksesgroup_mysql --> my sql (HR&ERP-Single Base)
- superadmin: suksesgroup_mysql / suksesgroup_mysql/ password123
- User Admin: suksesgroup_mysql / USR_001 /Pass1234!"

gordon/password123
 - [Sf1](http://192.168.0.112)
 - [Sf2](http://192.168.0.170)
 - [Sf3](http://192.168.0.185)
 - [Sf4](http://192.168.101.155)

---

### Learn Selenium       : *21 Feb - 6 Mar*

### Subject              : *Selenium 9 Mar - 20 Mar*
> Setting > Organization Setting > Company
- [x] Add Company
- [x] Edit Company
- [x] Delete Company  
> Setting > Organization Setting >  Organization Structure
- [x] Edit Department 
- [x] Edit Position *[Kurang Targeting Position di Dalam Organization]*
> Setting > Organization Setting > Job Title
- [x] Edit Job Title 
---
	
### Subject              : *Selenium 23 Mar - 27 Mar*
> Setting > Organization Setting > Job Grade
- [x] Add Job Grade 
- [x] Edit Job Grade
- [x] Delete Job Grade 
> Setting > Organization Setting > Job Grade Category
- [x] Add Job Grade Category
- [x] Edit Job Grade Category 
- [x] Delete Job Grade Category 
---

### Subject              :  *Selenium 30 Mar - 3 Apr*
> Setting > Organization Setting > Cost Center
- [x] Add Cost Center  
- [x] Edit Cost Center
- [x] Delete Cost Center
> Setting > Organization Setting > Job Family Grade
- [x] Edit Job Family Grade
> Setting > Organization Setting > Job Status
- [x] Add Job Status
- [x] Edit Job Status
- [x] Delete Job Status
---

### Subject              :  *Selenium 6 Apr - 9 Apr*
> Setting > Organization Setting > Job Family Level
- [x] Edit Job Family Level 
> Setting > Organization Setting > Job Family
- [x] Add Job Family
- [x] Edit Job Family 
> Setting > Organization Setting > Organization Structure
- [ ] View Organization Structure
> Organization > Company Policy
- [x] Add Company Policy **[Field Revisi]** **[Baru Satu Skenario]** **[-filter]**
- [x] Edit Company Policy **[Field Revisi]** **[Organization Unit]**
---

### Subject              :  *Selenium 13 Apr - 17 Apr*
> Organization > Organization Report
- [x] View Vacant Position Report   
- [x] View Job Grade Report
- [x] View Cost Center Position Report **[Save Filter]** **[Email This Report]**
- [x] View Position List Report
---

> Done Script
```JAVA
<class name="source.dataon.setting.organization_setting.company.TAddCompany"/>
<class name="source.dataon.setting.organization_setting.company.TUpdateCompany"/>
<class name="source.dataon.setting.organization_setting.company.TDeleteCompany"/>

<class name="source.dataon.setting.organization_setting.organization_structure.TUpdateDepartement"/>
<class name="source.dataon.setting.organization_setting.organization_structure.TUpdatePosition"/>
<class name="source.dataon.setting.organization_setting.job_title.TUpdateJobTitle"/>

<class name="source.dataon.setting.organization_setting.job_grade.TAddJobGrade"/>
<class name="source.dataon.setting.organization_setting.job_grade.TUpdateJobGrade"/>
<class name="source.dataon.setting.organization_setting.job_grade.TDeleteJobGrade"/>

<class name="source.dataon.setting.organization_setting.job_grade_category.TAddJobGradeCategory"/>
<class name="source.dataon.setting.organization_setting.job_grade_category.TUpdateJobGradeCategory"/>
<class name="source.dataon.setting.organization_setting.job_grade_category.TDeleteJobGradeCategory"/>

<class name="source.dataon.setting.organization_setting.cost_center.TAddCostCenter"/>
<class name="source.dataon.setting.organization_setting.cost_center.TUpdateCostCenter"/>
<class name="source.dataon.setting.organization_setting.cost_center.TDeleteCostCenter"/>

<class name="source.dataon.setting.organization_setting.organization_structure.job_status.TAddJobStatus"/>
<class name="source.dataon.setting.organization_setting.organization_structure.job_status.TUpdateJobStatus"/>
<class name="source.dataon.setting.organization_setting.organization_structure.job_status.TDeleteJobStatus"/>

<class name="source.dataon.setting.organization_setting.organization_structure.job_family_grade.TUpdateJobFamilyGrade"/>
<class name="source.dataon.setting.organization_setting.job_family_level.TUpdateJobFamilyLevel"/>

<class name="source.dataon.setting.organization_setting.job_family.TAddJobFamily"/>
<class name="source.dataon.setting.organization_setting.job_family.TUpdateJobFamily"/>

<class name="source.dataon.organization.company_policy.TAddCompanyPolicy"/>
<class name="source.dataon.organization.company_policy.TUpdateCompanyPolicy"/>

<class name="source.dataon.organization.organization_report.TViewVacantPositionReport"/>
<class name="source.dataon.organization.organization_report.TViewJobGradeReport"/>
<class name="source.dataon.organization.organization_report.TViewCostCenterReport"/>
<class name="source.dataon.organization.organization_report.TPositionListReport"/>

```

	
	 
	 
	
	  

	
	 
	
	 
	 
	 
    
	
	 
	
	 
	
