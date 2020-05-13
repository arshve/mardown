### Eg.

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

---

\\192.168.100.129\SharedFolder\QA\1.Quality Assurance\1.QA SunFish HR\3.SAT Form\SAT-2020
\\192.168.100.129\SharedFolder\QA\2.Documentation\3. Misc\Selenium Tutorial\1. SF6 HR Automation Test Data

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

### Subject : _Selenium 14 May - 18 May_

TCK2001-0543231

> Employee Info

- [ ] Edit Employee Custom Field
- [ ] Edit Employee Check List
- [ ] Edit Employee Skills
- [ ] Edit Employee Interest
- [ ] Edit Employee Document Controlt
  > Employee > Employee Letter
- [ ] Add Employee Letter
- [ ] Edit Employee Letter
- [ ] Delete Employee Letter
  > Employee > Employee Report
- [ ] View Report Based on Criteria
- [ ] View Employee Survey Report
- [ ] View Data Auhorization Log

---

### Subject : _Selenium 05 May - 15 May_

TCK2001-0543228

> Employee Info

- [x] Add Employee
- [x] Delete Employee
  > Setting > Employee Setting
- [x] Add Document Management
- [x] Edit Document Management
- [x] Delete Document Management
  > Setting > Employee Setting > Survey
- [x] Add Survey Setting
- [x] Edit Survey Setting
- [x] Delete Survey Setting
- [x] Add Survey Library
- [x] Edit Survey Library
- [x] Delete Survey Library

---

### Subject : _Selenium 13 Apr - 17 Apr_

TCK2002-0548712

> Organization > Organization Report

- [x] View Vacant Position Report
- [x] View Job Grade Report
- [x] View Cost Center Position Report **[Save Filter]** **[Email This Report]**
- [x] View Position List Report

---

### Subject : _Selenium 6 Apr - 9 Apr_

TCK2002-0548711

> Setting > Organization Setting > Job Family Level

- [x] Edit Job Family Level - [A123 edited]
  > Setting > Organization Setting > Job Family
- [x] Add Job Family
- [x] Edit Job Family
  > Organization > Organization Structure
- [x] View Organization Structure **Option Check**
  > Organization > Company Policy
- [x] Add Company Policy
- [x] Edit Company Policy

---

### Subject : _Selenium 30 Mar - 3 Apr_

TCK2002-0548710

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

### Subject : _Selenium 23 Mar - 27 Mar_

TCK2002-0548709

> Setting > Organization Setting > Job Grade

- [x] Add Job Grade
- [x] Edit Job Grade
- [x] Delete Job Grade
  > Setting > Organization Setting > Job Grade Category
- [x] Add Job Grade Category
- [x] Edit Job Grade Category
- [x] Delete Job Grade Category

---

### Subject : _Selenium 9 Mar - 20 Mar_

TCK2002-0548708

> Setting > Organization Setting > Company

- [x] Add Company
- [x] Edit Company
- [x] Delete Company
  > Setting > Organization Setting > Organization Structure
- [x] Edit Department
- [x] Edit Position _[Kurang Targeting Position di Dalam Organization]_
  > Setting > Organization Setting > Job Title
- [x] Edit Job Title

---

### Learn Selenium : _21 Feb - 6 Mar_

> Done Script

<details>
<summary> Script Class </summary>

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

<class name="source.dataon.employee.employee_information.TAddEmployee"/>
<class name="source.dataon.employee.employee_information.TDeleteEmployee"/>
<class name="source.dataon.setting.employee_setting.document_management.TAddDocument"/>
<class name="source.dataon.setting.employee_setting.document_management.TUpdateDocument"/>
<class name="source.dataon.setting.employee_setting.document_management.TDeleteDocument"/>
<class name="source.dataon.setting.employee_setting.survey.survey_library.TAddSurveyLibrary"/>
<class name="source.dataon.setting.employee_setting.survey.survey_library.TUpdateSurveyLibrary"/>
<class name="source.dataon.setting.employee_setting.survey.survey_library.TDeleteSurveyLibrary"/>
<class name="source.dataon.setting.employee_setting.survey.survey_setting.TAddSurveySetting"/>
<class name="source.dataon.setting.employee_setting.survey.survey_setting.TUpdateSurveySetting"/>
<class name="source.dataon.setting.employee_setting.survey.survey_setting.TDeleteSurveySetting"/>


```
