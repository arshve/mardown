Menu +[TASK](https://github.com/arshve/mardown/blob/master/Task.md)+ +[Repo Input](https://github.com/arshve/mardown/blob/master/Repo%20Input.md#Insert-Multiple-input-To-Right-Box)+ +[Repo Button](https://github.com/arshve/mardown/blob/master/Repo%20Button.md)+ +[Repo Documentation](https://github.com/arshve/mardown/blob/master/Repo%20Documentation.md)+ +[Repo Select By](https://github.com/arshve/mardown/blob/master/Repo%20Select%20By.md)+ +[Repo Select](https://github.com/arshve/mardown/blob/master/Repo%20Select.md)+ +[ModulSF List](https://github.com/arshve/mardown/blob/master/ModulSF6.md)+

### Eg.

Mind Hunter
Project X

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

---

\\192.168.100.129\SharedFolder\QA\1.Quality Assurance\1.QA SunFish HR\3.SAT Form\SAT-2020
\\192.168.100.129\SharedFolder\QA\2.Documentation\3. Misc\Selenium Tutorial\1. SF6 HR Automation Test Data

<details>
<summary> Script </summary>

Reset Tag   : ?resetapp=1&recache=1&resetctag=1&forcegen=1 <br>
Comp Id     : ?sfid=sys.sec.sfinfo&sfchid=sys.sec.func._xdump&param=REQUEST.scookie <br>
Cek Server CF/Lucee : http://192.168.102.149/sf6/lucee/admin/web.cfm <br>

#### Scheduler <br>
> DSN schedule task <br>
dev mode = dbSF6_SaaS_DEVELOPMENT <br>
test mode = dbSF6_SaaS_TESTING <br>
release mode = dbsf6_saas

Scheduler 1 : ?sfid=sys.sec.cron.careerschedule&dsn=dbSF6_SaaS_TESTING&coid=83&currentdt=yyyy-mm-dd <br>
Scheduler 2 : ?sfid=sys.sec.cron.careerschedule&dsn=dbSF6_SaaS_TESTING&compid=83&currentdt=yyyy-mm-dd <br>
Cek Error Sys: https://sfid.dataon.com/sf6/index.cfm?sfid=sys.sec.viewlog&logpath="sferr.dataon1.20200826.expression_sfid_nas_dpx_20200826154458_616.htm"

</details>

<details>
<summary> Account </summary>

#### Sukses Group

URL: 192.168.101.155/sf6

- Account: suksesgroup_mysql --> my sql (HR&ERP-Single Base)
- superadmin: suksesgroup_mysql / suksesgroup_mysql/ password123
- User Admin: suksesgroup_mysql / USR_001 /Pass1234!"

#### Test Mode

|    UserName     |  Password   | Etc.        |
| :-------------: | :---------: | ----------- |
|     gordon      | password123 |             |
|   superadmin    |  Pass1234!  |             |
| shallistera1990 | password123 | Shallis     |
|     USR_003     | password123 | Lindsay     |
|     farvan      | password123 | Evan        |
|      ryan       | password1234| Ryan        |
|      rifqi      | password123 | Rifqi       |
|     arsenal     | password123 | Invoker     |
|     abdul98     | password123 | Abdul Soleh |
|     kiryu       | password123 | Kiryu Coco  |
|     coco        | password123 | Coco Kiryu  |
|     ryan123     | password123 | Ryan[TH]    |
|   THPRM200004   | Farvan123!  | Jane[TH]    |

#### Release Mode

|  UserName  |   Password   | Etc.     |
| :--------: | :----------: | -------- |
|   gordon   | password123  |          |
| superadmin | password123  |          |
|  ryan1990  | password123  | Ryan     |
| rifqi1992  | password123  | Rifqi    |
| raihan1990 | password123  | Raihan   |
|    jane    | Password123! | Jane[TH] |

#### Online

##### BizNet

> sfid.dataon.com

dataon1
| UserName | Password | Etc. |
|:---------------:|:-----------:|----------|
| gordon |d4t40n123 | |
| abdul1990 |password123 | Abudul Mina |
| dataon1 |d4t40n1234\$ |SuperAdmin|

##### NBC

> sf.dataon.com / sfdemo.dataon.com

dataon
| UserName | Password | Etc. |
|:---------------:|:-----------:|----------|
| gordon |password123 | |
| a.1990 |password123 | A.Enrica |
| adrian |password123 |Admin[Th]|

##### Great Day

> [Great Day](https://app.greatdayhr.com/app-dev/login#/home2) / [sfdemo.dataon.com](http://192.168.102.170/sf6/) /
> [Great Day Stagging](https://app.greatdayhr.com/artifacts/staging/feature-feat-training-noncalendar/#/login2)

|     Account     | UserName |   Password   | Etc.     |
| :-------------: | :------: | :----------: | -------- |
| suksesgroup-dev | USR_001  |  Pass1234!   | GreatDay |
|   suksesgroup   | USR_001  |  Pass1234!   | SF6      |
|   dataon1-dev   |  gordon  | Password123! | GreatDay |
|     dataon1     |  gordon  | Password123! | SF6      |

Stagging Acc
| Account | UserName | Password | Etc. |
|:---------------:|:-----------:|:-----------:|----------|
| suksesgroup-dev-gd https://api.greatdayhr.com/staging5 | USR_001 | Pass1234! | GreatDay Stagging|
| dataon1-dev-gd https://api.greatdayhr.com/staging5 | gordon | Password123! | GreatDay Stagging|

suksesgroup-dev-gd|https://api.greatdayhr.com/staging5
dataon1-dev-gd|https://api.greatdayhr.com/staging5

[GreatDay APK](https://app.greatdayhr.com/artifacts/dist/develop/android/apk/)

#### GreatDay Push Notif link

[Push Notif](http://192.168.102.170/sf6/index.cfm?sfid=sys.sec.cron.resourcebooking_schedule&dsn=dbSF_SUKSESGROUP&company_id=16487&instance=suksesgroup&cocode=suksesgroup&category_code=001&dev)

<br />
Shared Folder
user : dataon\farid.ramadhan
pass : S7j6h65g4*&^^%$

<br />
BugTest PAss
t0^1#APA\*g4V

</details>

- [Sf1](http://192.168.0.112)
- [Sf2](http://192.168.0.170)
- [Sf3](http://192.168.0.185)
- [Sf4](http://192.168.101.155)


---
### Subject : _Selenium June
TCK2106-0650391

>  Setting > Performance Setting > Competency Library
      
- [x] Add Competency Library type Category
- [x] Edit Competency Library type Category
- [x] Delete Competency Library type Category
- [x] Add Competency Library type Question Based on Job Family
- [x] Add Competency Library type Question Based on Job Title
- [x] Edit Competency Library type Question Based on Job Family
- [x] Edit Competency Library type Question Based on Job Title
- [x] Delete Competency Library type Question Based on Job Family
- [x] Delete Competency Library type Question Based on Job Title
- [x] Upload Competency Library
>  
- [x] Competency Matrix by Job Family
- [x] Competency Matrix by Job Title
- [ ] Competency Matrix by Job Family set Configure with Excel "Yes"
- [ ] Competency Matrix by Job Title set Configure with Excel "Yes"

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.performance_setting.competency_library.TAddCompetencyLibrary"/>
<class name="source.dataon.setting.performance_setting.competency_library.TUpdateCompetencyLibrary"/>
<class name="source.dataon.setting.performance_setting.competency_library.TDeleteCompetencyLibrary"/
<class name="source.dataon.setting.performance_setting.competency_library.TUploadCompetency"/>
<class name="source.dataon.setting.performance_setting.competency_library.TCompetencyMatrix"/>

```

---

</details>

TCK2106-0650391

>  Setting > Performance Setting > Performance Period Setting
      
- [x] Add Performance Period dengan Period Component "Appraisal", set Configure Main Filter Position
- [x] Add Performance Period dengan Period Component "Appraisal", set Configure Main Appraisal Library
- [x] Add Performance Period dengan Period Component "Org Unit Kpi", set Configure Main Filter Organization Unit
- [x] Add Performance Period dengan Period Component "Org Unit KPI", set Configure Main KPI Library
- [x] Add Performance Period dengan Period Component "Personal KPI", set Configure Main Filter Position
- [x] Add Performance Period dengan Period Component "Personal KPI", set Configure Main KPI Library
- [x] Add Performance Period dengan Period Component "Competency", set Configure
- [x] Add Performance Period dengan Period Component "Task" dan "Feedback"

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.performance_setting.performance_period.TPerformancePeriodAppraisal"/>
<class name="source.dataon.setting.performance_setting.performance_period.TPerformanceOrgUnitKPI"/>
<class name="source.dataon.setting.performance_setting.performance_period.TPerformancePersonalKPI"/>
<class name="source.dataon.setting.performance_setting.performance_period.TPerformanceCompTask"/>
			
```
</details>

---
### Subject : _Selenium May

TCK2105-0644797 <br>
TCK2105-0644798

>  Setting > Performance Setting > KPI Library
      
- [x] Add KPI Library type Category
- [x] Edit KPI Library type Category
- [x] Delete KPI Library type Category
- [x] Add KPI Library type Question
- [x] Edit KPI Library type Question
- [x] Delete KPI Library type Question
- [x] Upload KPI Library

>  Setting > Performance Setting > Appraisal Library
      
- [x] Add Appraisal Library type Category
- [x] Edit Appraisal Library type Category
- [x] Delete Appraisal Library type Category
- [x] Add Appraisal Library type Question
- [x] Edit Appraisal Library type Question
- [x] Delete Appraisal Library type Question
- [x] Upload Apprisal Library

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.performance_setting.kpi_library.TAddKPICategory"/>
<class name="source.dataon.setting.performance_setting.kpi_library.TUpdateKPICategory"/>
<class name="source.dataon.setting.performance_setting.kpi_library.TDeleteKPICategory"/>
<class name="source.dataon.setting.performance_setting.kpi_library.TAddKPIQuestion"/>
<class name="source.dataon.setting.performance_setting.kpi_library.TUpdateKPIQuestion"/>
<class name="source.dataon.setting.performance_setting.kpi_library.TDeleteKPIQuestion"/>

<class name="source.dataon.setting.performance_setting.kpi_library.TUploadKPILibrary"/>

<class name="source.dataon.setting.performance_setting.appraisal_library.TAddAppraisalCategory"/>
<class name="source.dataon.setting.performance_setting.appraisal_library.TUpdateAppraisalCategory"/>
<class name="source.dataon.setting.performance_setting.appraisal_library.TDeleteAppraisalCategory"/>
<class name="source.dataon.setting.performance_setting.appraisal_library.TAddAppraisalQuestion"/>
<class name="source.dataon.setting.performance_setting.appraisal_library.TUpdateAppraisalQuestion"/>
<class name="source.dataon.setting.performance_setting.appraisal_library.TDeleteAppraisalQuestion"/>
		
<class name="source.dataon.setting.performance_setting.appraisal_library.TUploadAppraisalLibrary"/>

```
</details>

---
### Subject : _Selenium Maret

TCK2104-0637770 <br>
TCK2104-0637795

>  Reimbursement > Claim Cancellation Request
      
- [x] Reimbursement Upload
- [x] Add Claim Cancellation Request
- [x] Edit Claim Cancellation Request
- [x] Delete Claim Cancellation Request

>  Reimbursement > Claim Form
      
- [x] Add Claim Form dengan menggunakan Type Of Claim used GST Setting
- [x] Edit Claim Form dengan menggunakan Type Of Claim used GST Setting
- [x] Delete Claim Form dengan menggunakan Type Of Claim used GST Setting
>  
- [x] Add Claim Form dengan menggunakan Exchange Rate Loss Compensation
- [x] Edit Claim Form dengan menggunakan Exchange Rate Loss Compensation
- [x] Delete Claim Form dengan menggunakan Exchange Rate Loss Compensation

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.reimbursement.reimbursement_upload.TReimbursementUpload"/>
<class name="source.dataon.reimbursement.cancel_claim_form.TAddCancelClaimRequest"/>
<class name="source.dataon.reimbursement.cancel_claim_form.TUpdateCancelClaimRequest"/>
<class name="source.dataon.reimbursement.cancel_claim_form.TDeleteCancelClaimRequest"/>

<class name="source.dataon.reimbursement.claim_form.ERLC.TAddClaimForm"/>
<class name="source.dataon.reimbursement.claim_form.ERLC.TUpdateClaimForm"/>
<class name="source.dataon.reimbursement.claim_form.ERLC.TDeleteClaimForm"/>

<class name="source.dataon.reimbursement.claim_form.GST.TAddClaimForm"/>
<class name="source.dataon.reimbursement.claim_form.GST.TUpdateClaimForm"/>
<class name="source.dataon.reimbursement.claim_form.GST.TDeleteClaimForm"/>

```
</details>

---
### Subject : _Selenium Maret

TCK2001-0543247

>  Setting > Reimbursement Setting > Type of Claim
      
- [x] Add Type of Claim (Claim Category Allowance and select Claim Rule
- [x] Edit Type of Claim (Claim Category Allowance and select Claim Rule
- [x] Delete Type of Claim(Claim Category Allowance
>  
- [x] Add Type of Claim (Claim Category Expense)
- [x] Edit Type of Claim (Claim Category Expense)
- [x] Delete Type of Claim (Claim Category Expense)

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.reimbursement_setting.type_of_claim.TAddTypeofClaim"/>
<class name="source.dataon.setting.reimbursement_setting.type_of_claim.TUpdateTypeofClaim"/>
<class name="source.dataon.setting.reimbursement_setting.type_of_claim.TDeleteTypeofClaim"/>

```
</details>

---
### Subject : Selenium 01 Mar -31 Mar 2021

TCK2001-0543252

>  Reimbursement > Claim Form
      
- [x] Add Claim Item
- [x] Edit Claim Item
- [x] Delete Claim Item
>  
- [x] Add Claim Form
- [x] Edit Claim Form
- [x] Delete Claim Form

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.reimbursement.claim_form.TAddClaimItem"/>
<class name="source.dataon.reimbursement.claim_form.TAddClaimItem"/>
<class name="source.dataon.reimbursement.claim_form.TAddClaimItem"/>

<class name="source.dataon.reimbursement.claim_form.TAddClaimItem"/>
<class name="source.dataon.reimbursement.claim_form.TDeleteClaimItem"/>
<class name="source.dataon.reimbursement.claim_form.TUpdateClaimItem"/>

```
</details>

---
### Subject : _Selenium 01 Des - 04 Des 2020_

TCK2001-0543247

>  Setting > Reimbursement Setting > Destination
      
- [x] Add Destination
- [x] Edit Destination
- [x] Delete Destination

>  Setting > Reimbursement Setting > Exchange Rate Loss Compensation

- [x] Add Exchange Rate Loss Compensation
- [x] Edit Exchange Rate Loss Compensation
- [x] Delete Exchange Rate Loss Compensation

>  Setting > Reimbursement Setting > GST Setting

- [x] Add GST Setting
- [x] Edit GST Setting
- [x] Delete GST Setting

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.reimbursement_setting.TAddDestination"/>
<class name="source.dataon.setting.reimbursement_setting.TUpdateDestination"/>
<class name="source.dataon.setting.reimbursement_setting.TDeleteDestination"/>

<class name="source.dataon.setting.reimbursement_setting.erl_compensation.TAddERLComp"/>
<class name="source.dataon.setting.reimbursement_setting.erl_compensation.TUpdateERLComp"/>
<class name="source.dataon.setting.reimbursement_setting.erl_compensation.TDeleteERLComp"/>

<class name="source.dataon.setting.reimbursement_setting.GST.TAddGST"/>
<class name="source.dataon.setting.reimbursement_setting.GST.TUpdateGST"/>
<class name="source.dataon.setting.reimbursement_setting.GST.TDeleteGST"/>

```
</details>

---

### Subject : _Selenium 10 Nov - 11 Nov 2020_

TCK2001-0543250

>  Reimbursement 
      
- [x] Generate Reimbursement Balance
- [x] Update Payment Process

>  Reimbursement > Generate Reimbursement Balance

- [x] Edit Reimbursement Balance Maintenance
- [x] Delete Reimbursement Balance Maintenance

>  Reimbursement > Reimbursement Interface

- [x] Interface Process View
- [x] Reimbursement Interface Result
- [x] Update Payment Process
- [x] View Doctor and Hospital List

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.reimbursement_interface.TInterfaceProcess"/>
<class name="source.dataon.reimbursement_interface.TReimbursementInterfaceResult"/>
<class name="source.dataon.reimbursement.TUpdatePaymentProcess"/>

<class name="source.dataon.reimbursement.TViewDoctorHospitalList"/>
<class name="source.dataon.reimbursement.TGenerateReimbursementBalance"/>
<class name="source.dataon.reimbursement_balance_maintenance.TEditReimbursementBalanceMaintenance"/>
<class name="source.dataon.reimbursement_balance_maintenance.TDeleteReimbursementBalanceMaintenance"/>

```
</details>

---

### Subject : _Selenium 28 Sep - 02 oct 2020_

TCK2009-0587797

>  Setting > Reimbursement Setting > Reimbursement Type

- [x] Add Reimbursement Type
- [x] Edit Reimbursement Type
- [x] Delete Reimbursement Type
  
>   Setting > Reimbursement Setting > Type Of Claim

- [x] Edit Type of Claim
- [x] Delete Claim Rule Setting

##### Script

<details>
<summary> Script Class </summary>

```JAVA
<class name="source.dataon.setting.reimbursement_setting.reimbursement_type.TAddReimbursementType"/>
<class name="source.dataon.setting.reimbursement_setting.reimbursement_type.TUpdateReimbursementType"/>
<class name="source.dataon.setting.reimbursement_setting.reimbursement_type.TDeleteReimbursementType"/>	
```
</details>


---

### Subject : _Selenium 14 Sep - 18 Sep 2020_

TCK2001-0543251

> Reimbursement > Reimbursement Report

- [x] View Reimbursement Interface Result
- [x] View Reimbursement Payment Lag Time
- [x] View Employee Reimbursement Request
- [x] View Reimbursement Balance Report
- [x] View Reimbursement Balance and Usage Report
- [x] View Reimbursement Cancellation Request Report

> Reimbursement > Reimbursement Upload

- [ ] Reimbursement Upload

##### Script

<details>
<summary> Script Class </summary>

```JAVA
<class name="source.dataon.setting.reimbursement_report.TViewReimbursementInterfaceResult"/>
<class name="source.dataon.setting.reimbursement_report.TViewReimbursementPaymentLagTime"/>
<class name="source.dataon.setting.reimbursement_report.TViewReimbursementBalanceReport"/>
<class name="source.dataon.setting.reimbursement_report.TViewReimbursementRequest"/>
<class name="source.dataon.setting.reimbursement_report.TViewReimbursementBalanceUsageReport"/>
<class name="source.dataon.setting.reimbursement_report.TViewReimbursementCancellReqReport"/>	
```
</details>

---

### Subject : _Selenium 08 Sep - 11 Sep 2020_

TCK2001-0543249

> ReimbursementMy > Reimbursement Balance

- [x] My Reimbursement Balance

> Reimbursement > Reimbursement Request

- [x] Add Reimbursement Request
- [x] Edit Reimbursement Request (Draft)
- [x] Delete Reimbursement Request (Draft)

> Reimbursement > Reimbursement Cancellation Request

- [x] Add Reimbursement Cancellation Request
- [x] Edit Reimbursement Cancellation Request (Draft)
- [x] Delete Reimbursement Cancellation Request (Draft)

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.reimbursement.TMyReimbursementBalance"/>

<class name="source.dataon.setting.reimbursement_request.TAddReimbursementRequest"/>
<class name="source.dataon.setting.reimbursement_request.TUpdateReimbursementRequest"/>
<class name="source.dataon.setting.reimbursement_request.TDeleteReimbursementRequest"/>

<class name="source.dataon.setting.reimbursement_cancel_request.TAddReimbursementCancelRequest"/>
<class name="source.dataon.setting.reimbursement_cancel_request.TUpdateReimbursementCancelRequest"/>
<class name="source.dataon.setting.reimbursement_cancel_request.TDeleteReimbursementCancelRequest"/>
				
```
</details>

---

### Subject : _Selenium 31 Aug - 03 Sep 2020_

TCK2001-0543244

> Setting >Reimbursement Setting > Type Of Claim

- [x] Add Type of Claim
- [x] Edit Type of Claim
- [x] Delete Type of Claim

> Setting > Reimbursement Setting > Claim Rule Setting

- [x] Add Claim Rule Setting
- [x] Edit Claim Rule Setting
- [x] Delete Claim Rule Setting

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.reimbursement_setting.type_of_claim.TAddTypeofClaim"/>
<class name="source.dataon.setting.reimbursement_setting.type_of_claim.TUpdateTypeofClaim"/>
<class name="source.dataon.setting.reimbursement_setting.type_of_claim.TDeleteTypeofClaim"/>
				
<class name="source.dataon.setting.reimbursement_setting.claim_rule_setting.TAddClaimRuleSetting"/>
<class name="source.dataon.setting.reimbursement_setting.claim_rule_setting.TUpdateClaimRuleSetting"/>
<class name="source.dataon.setting.reimbursement_setting.claim_rule_setting.TDeleteClaimRuleSetting"/>		

```
</details>

---

### Subject : _Selenium 20 Jul - 24 Jul 2020_

TCK2005-0567957

> Training > Training Report

- [x] View Training Feedback Report
- [x] View Training Evaluation Report
- [x] View Training Record Report
- [x] View Mandatory Training Report
- [x] View Training Waiting List Report
- [x] View Training Budget Report
- [x] View Training Request Report
- [x] View Quiz Report

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.training.training_report.TTrainingFeedbackReport"/>
<class name="source.dataon.training.training_report.TTrainingEvaluationReport"/>
<class name="source.dataon.training.training_report.TTrainingRecordReport"/>
<class name="source.dataon.training.training_report.TMandatoryTrainingReport"/>
<class name="source.dataon.training.training_report.TTrainingWaitingListReport"/>
<class name="source.dataon.training.training_report.TTrainingBudgetReport"/>
<class name="source.dataon.training.training_report.TTrainingRequestReport"/>
<class name="source.dataon.training.training_report.TELearningQuizReport"/>

```
</details>

---

### Subject : _Selenium 13 Jul - 17 Jul 2020_

TCK2005-0567956

> Training > Training Report

- [x] View Training Cost Report
- [x] View Training Event Report
- [x] View Training Course Report
- [x] View Training Attendance Report
- [x] View Training Hours Report

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.training.training_report.TTrainingEventReport"/>
<class name="source.dataon.training.training_report.TTrainingCourseReport"/>
<class name="source.dataon.training.training_report.TTrainingCostReport"/>
<class name="source.dataon.training.training_report.TTrainingAttendanceReport"/>
<class name="source.dataon.training.training_report.TTrainingHoursReport"/>

```
</details>

---

### Subject : _Selenium 6 Jul - 10 Jul 2020_

TCK2005-0567955

> Training > Training Evaluation

- [x] Update Training Feedback
- [x] Update Training Evaluation
- [ ] Update Catalogue Update

> Training > My E-Learning

- [x] Add E-Learning Request
- [x] Edit E-Learning Request
- [x] Delete E-Learning Request (Draft)

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.training.my_elearning.TAddElearningRequest"/>
<class name="source.dataon.training.my_elearning.TUpdateElearningRequest"/>
<class name="source.dataon.training.my_elearning.TDeleteElearningRequest"/>

```
</details>

---

### Subject : _Selenium 29 June - 03 July_

TCK2005-0567954

> Training > Training Course Detailed

- [x] Add E-Learning Class (Training)
- [x] Edit E-Learning Class (Training)
- [x] Delete E-Learning Class (Training)

> Training > Training Evaluation

- [x] Update Training Attendance
- [x] Update Training Feedback
- [x] Update Training Evaluation

> Training > Training Request (Draft)

- [x] Add Training Request
- [x] Edit Training Request (Draft)
- [x] Delete Training Request (Draft)

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.training.training_course.TAddTrainingCourseElearning"/>
<class name="source.dataon.training.training_course.TUpdateTrainingCourseElearning"/>
<class name="source.dataon.training.training_course.TDeleteTrainingCourseElearning"/>

<class name="source.dataon.training.training_evaluation.TUpdateTrainingAttendance"/>
<class name="source.dataon.training.training_evaluation.TUpdateTrainingFeedback"/>
<class name="source.dataon.training.training_evaluation.TUpdateTrainingEvaluation"/>

<class name="source.dataon.training.training_request.TAddTrainingRequest"/>
<class name="source.dataon.training.training_request.TUpdateTrainingRequest"/>
<class name="source.dataon.training.training_request.TDeleteTrainingRequest"/>

```

</details>

---

### Subject : _Selenium 22 June - 26 June_

TCK2005-0567951

> Training > Training Course Detailed

- [x] Add Feedback (Training)
- [x] Edit Feedback (Training)
- [x] Delete Feedback (Training)
  >
- [x] Add Evaluation (Training)
- [x] Edit Evaluation (Training)
- [x] Delete Evaluation (Training)
  >
- [x] Add Event (Training)
- [x] Edit Event (Training)
- [x] Delete Event (Training)

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.training.training_course.TAddTrainingCourseFeedback"/>
<class name="source.dataon.training.training_course.TUpdateTrainingCourseFeedback"/>
<class name="source.dataon.training.training_course.TDeleteTrainingCourseFeedback"/>

<class name="source.dataon.training.training_course.TAddTrainingCourseEvaluation"/>
<class name="source.dataon.training.training_course.TUpdateTrainingCourseEvaluation"/>
<class name="source.dataon.training.training_course.TDeleteTrainingCourseEvaluation"/>

<class name="source.dataon.training.training_course.TAddTrainingCourseEvent"/>
<class name="source.dataon.training.training_course.TUpdateTrainingCourseEvent"/>
<class name="source.dataon.training.training_course.TDeleteTrainingCourseEvent"/>

```

</details>

---

### Subject : _Selenium 15 June - 19 June_

TCK2005-0567946

> Setting > Training Setting > Training Cost

- [x] Add Training Item Cost
- [x] Edit Training Item Cost
- [x] Delete Training Item Cost

> Setting > Training Setting > Training Evaluation Stage

- [x] Add Training Evaluation Stage
- [x] Edit Training Evaluation Stage
- [x] Delete Training Evaluation Stage

TCK2005-0567949

> Training > Training Course

- [x] Add Training Course List
- [x] Edit Training Course List
- [x] Delete Training Course List
- [x] Set Mandatory Training

> Training > Training Course Detailed

- [x] Add Competency (Training)
- [x] Edit Competency (Training)
- [x] Add Content (Training)
- [x] Edit Content (Training)
- [x] Delete Content (Training)

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.training_setting.training_item_cost.TAddTrainingItemCost"/>
<class name="source.dataon.setting.training_setting.training_item_cost.TUpdateTrainingItemCost"/>
<class name="source.dataon.setting.training_setting.training_item_cost.TDeleteTrainingItemCost"/>

<class name="source.dataon.setting.training_setting.training_evaluation_stage.TAddTrainingEvaluationStage"/>
<class name="source.dataon.setting.training_setting.training_evaluation_stage.TUpdateTrainingEvaluationStage"/>
<class name="source.dataon.setting.training_setting.training_evaluation_stage.TDeleteTrainingEvaluationStage"/>

<class name="source.dataon.training.training_course.TAddTrainingCourseList"/>
<class name="source.dataon.training.training_course.TUpdateTrainingCourseList"/>
<class name="source.dataon.training.training_course.TDeleteTrainingCourseList"/>
<class name="source.dataon.training.training_course.TSetMandatoryTraining"/>

<class name="source.dataon.training.training_course.TAddTrainingCourseCompetency"/>
<class name="source.dataon.training.training_course.TUpdateTrainingCourseCompetency"/>

<class name="source.dataon.training.training_course.TAddTrainingCourseContent"/>
<class name="source.dataon.training.training_course.TUpdateTrainingCourseContent"/>
<class name="source.dataon.training.training_course.TDeleteTrainingCourseContent"/>

```

</details>

---

### Subject : _Selenium 8 June - 12 June_

TCK2005-0567946

> Setting > Training Setting > Training Venue

- [x] Add Training Venue
- [x] Edit Training Venue
- [x] Delete Training Venue

> Setting > Training Setting > Training Evaluation

- [x] Add Training Feedback
- [x] Edit Training Feedback
- [x] Delete Training Feedback
- [x] Add Training Evaluation
- [x] Edit Training Evaluation
- [x] Delete Training Evaluation

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.training_setting.training_venue.TAddTrainingVenue"/>
<class name="source.dataon.setting.training_setting.training_venue.TUpdateTrainingVenue"/>
<class name="source.dataon.setting.training_setting.training_venue.TDeleteTrainingVenue"/>

<class name="source.dataon.setting.training_setting.training_evaluation_library.TAddTrainingFeedback"/>
<class name="source.dataon.setting.training_setting.training_evaluation_library.TUpdateTrainingFeedback"/>
<class name="source.dataon.setting.training_setting.training_evaluation_library.TDeleteTrainingFeedback"/>

<class name="source.dataon.setting.training_setting.training_evaluation_library.TAddTrainingEvaluation"/>
<class name="source.dataon.setting.training_setting.training_evaluation_library.TUpdateTrainingEvaluation"/>
<class name="source.dataon.setting.training_setting.training_evaluation_library.TDeleteTrainingEvaluation"/>

```

</details>

---

### Subject : _Selenium 2 June - 5 June_

TCK2005-0567944

> Setting > Training Setting > Training Category

- [x] Add Training Category
- [x] Edit Training Category
- [x] Delete Training Category

> Setting > Training Setting > Training Provider

- [x] Add Training Provider
- [x] Edit Training Provider
- [x] Delete Training Provider

> Setting > Training Setting > Training Instructor

- [x] Add Training Instructor
- [x] Edit Training Instructor
- [x] Delete Training Instructor

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.training_setting.training_category.TAddTrainingCategory"/>
<class name="source.dataon.setting.training_setting.training_category.TUpdateTrainingCategory"/>
<class name="source.dataon.setting.training_setting.training_category.TDeleteTrainingCategory"/>

<class name="source.dataon.setting.training_setting.training_provider.TAddTrainingProvider"/>
<class name="source.dataon.setting.training_setting.training_provider.TUpdateTrainingProvider"/>
<class name="source.dataon.setting.training_setting.training_provider.TDeleteTrainingProvider"/>

<class name="source.dataon.setting.training_setting.training_instructor.TAddTrainingInstructor"/>
<class name="source.dataon.setting.training_setting.training_instructor.TUpdateTrainingInstructor"/>
<class name="source.dataon.setting.training_setting.training_instructor.TDeleteTrainingInstructor"/>

```

</details>

---

### Subject : _Selenium 14 May - 18 May_

TCK2001-0543231

> Employee Info

- [x] Edit Employee Custom Field
- [x] Edit Employee Check List
- [x] Edit Employee Skills
- [x] Edit Employee Interest
- [x] Edit Employee Document Controlt

> Employee > Employee Letter

- [x] Add Employee Letter
- [x] Edit Employee Letter
- [x] Delete Employee Letter

> Employee > Employee Report

- [ ] View Report Based on Criteria
- [ ] View Employee Survey Report
- [ ] View Data Auhorization Log

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.employee.employee_information.employment_data.TUpdateEmployeeCostumeField"/>
<class name="source.dataon.employee.employee_information.employment_data.TUpdateEmployeeCheckList"/>
<class name="source.dataon.employee.employee_information.additional_info.TUpdateEmployeeSkill"/>
<class name="source.dataon.employee.employee_information.additional_info.TUpdateEmployeeInterest"/>
<class name="source.dataon.employee.employee_information.additional_info.TUpdateEmployeeDocumentControl"/>

<class name="source.dataon.employee.employee_letter.TAddEmployeeLetter"/>
<class name="source.dataon.employee.employee_letter.TUpdateEmployeeLetter"/>
<class name="source.dataon.employee.employee_letter.TDeleteEmployeeLetter"/>

```

</details>

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

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.employee.employee_information.TAddEmployee"/>
<class name="source.dataon.employee.employee_information.TDeleteEmployee"/>

<class name="source.dataon.setting.employee_setting.document_management.TAddDocument"/>
<class name="source.dataon.setting.employee_setting.document_management.TUpdateDocument"/>
<class name="source.dataon.setting.employee_setting.document_management.TDeleteDocument"/>

<class name="source.dataon.setting.employee_setting.survey.survey_setting.TAddSurveySetting"/>
<class name="source.dataon.setting.employee_setting.survey.survey_setting.TUpdateSurveySetting"/>
<class name="source.dataon.setting.employee_setting.survey.survey_setting.TDeleteSurveySetting"/>

<class name="source.dataon.setting.employee_setting.survey.survey_library.TAddSurveyLibrary"/>
<class name="source.dataon.setting.employee_setting.survey.survey_library.TUpdateSurveyLibrary"/>
<class name="source.dataon.setting.employee_setting.survey.survey_library.TDeleteSurveyLibrary"/>

```

</details>

---

### Subject : _Selenium 13 Apr - 17 Apr_

TCK2002-0548712

> Organization > Organization Report

- [x] View Vacant Position Report
- [x] View Job Grade Report
- [x] View Cost Center Position Report **[Save Filter]** **[Email This Report]**
- [x] View Position List Report

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.organization.organization_report.TViewVacantPositionReport"/>
<class name="source.dataon.organization.organization_report.TViewJobGradeReport"/>
<class name="source.dataon.organization.organization_report.TViewCostCenterReport"/>
<class name="source.dataon.organization.organization_report.TPositionListReport"/>

```

</details>

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
- [x] Delete Company Policy

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.organization_setting.organization_structure.job_family_grade.TUpdateJobFamilyGrade"/>
<class name="source.dataon.setting.organization_setting.job_family_level.TUpdateJobFamilyLevel"/>

<class name="source.dataon.setting.organization_setting.job_family.TAddJobFamily"/>
<class name="source.dataon.setting.organization_setting.job_family.TUpdateJobFamily"/>

<class name="source.dataon.organization.company_policy.TAddCompanyPolicy"/>
<class name="source.dataon.organization.company_policy.TUpdateCompanyPolicy"/>
<class name="source.dataon.organization.company_policy.TDeleteCompanyPolicy"/>

```

</details>

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

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.organization_setting.cost_center.TAddCostCenter"/>
<class name="source.dataon.setting.organization_setting.cost_center.TUpdateCostCenter"/>
<class name="source.dataon.setting.organization_setting.cost_center.TDeleteCostCenter"/>

<class name="source.dataon.setting.organization_setting.organization_structure.job_status.TAddJobStatus"/>
<class name="source.dataon.setting.organization_setting.organization_structure.job_status.TUpdateJobStatus"/>
<class name="source.dataon.setting.organization_setting.organization_structure.job_status.TDeleteJobStatus"/>

```

</details>

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

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.organization_setting.job_grade.TAddJobGrade"/>
<class name="source.dataon.setting.organization_setting.job_grade.TUpdateJobGrade"/>
<class name="source.dataon.setting.organization_setting.job_grade.TDeleteJobGrade"/>

<class name="source.dataon.setting.organization_setting.job_grade_category.TAddJobGradeCategory"/>
<class name="source.dataon.setting.organization_setting.job_grade_category.TUpdateJobGradeCategory"/>
<class name="source.dataon.setting.organization_setting.job_grade_category.TDeleteJobGradeCategory"/>

```

</details>

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

##### Script

<details>
<summary> Script Class </summary>

```JAVA

<class name="source.dataon.setting.organization_setting.company.TAddCompany"/>
<class name="source.dataon.setting.organization_setting.company.TUpdateCompany"/>
<class name="source.dataon.setting.organization_setting.company.TDeleteCompany"/>

<class name="source.dataon.setting.organization_setting.organization_structure.TUpdateDepartement"/>
<class name="source.dataon.setting.organization_setting.organization_structure.TUpdatePosition"/>
<class name="source.dataon.setting.organization_setting.job_title.TUpdateJobTitle"/>

```

</details>

---

### Learn Selenium : _21 Feb - 6 Mar_
