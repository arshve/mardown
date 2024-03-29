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
Reset Menu  : ?resetapp=1&resetctag=1&resetmenu <br>
Comp Id     : ?sfid=sys.sec.sfinfo&sfchid=sys.sec.func._xdump&param=REQUEST.scookie <br>
Cek Server CF/Lucee : http://192.168.102.149/sf6/lucee/admin/web.cfm <br>
Cek DB Akun : ?sfid=sys.sec.sfinfo&sfchid=sys.sec.func._xdump&param=REQUEST.dbdriver <br>

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
pass : IndoDev24@$


</details>

- [Sf1](http://192.168.0.112)
- [Sf2](http://192.168.0.170)
- [Sf3](http://192.168.0.185)
- [Sf4](http://192.168.101.155)
--- 
<details>
<summary> <span style="color:orange">Selenium November</span> </summary>

TCK2111-0685351

>  Setting > Performance Setting > Succession Parameter
      
- [x] Add Succession Planning
- [x] Edit Succession Planning > Search Successor
- [x] Edit Succession Planning > View Lengh of Service
- [x] Edit Succession Planning > View Performance
- [x] Edit Succession Planning > View Competency
- [x] Edit Succession Planning > View Box Analysis
- [x] Edit Succession Planning > Drilldown
- [x] Edit Succession Planning > Preferred
- [x] Edit Succession Planning > Remove

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.performance.TSuccessionPlanning"/>

```

</details>

TCK2111-0685352

>  Performance Management > Performance Conclusion Adjustment

- [x] Upload Performance Conclusion Adjustment, Replace existing data"Yes"
- [x] Upload Performance Conclusion Adjustment, Replace existing data"No"
- [x] Add Performance Conclusion Adjustment All Grade, All Org Unit, All Position, All Employee kemudian draft
- [x] Add Performance Conclusion Adjustment beberapa Grade, beberapa Org Unit, beberapa Position, beberapa Employee kemudian draft
- [x] Add Performance Conclusion Adjustment All Grade, All Org Unit, All Position, All Employee kemudian submit
- [x] Add Performance Conclusion Adjustment beberapa Grade, beberapa Org Unit, beberapa Position, beberapa Employee kemudian submit
- [x] Edit Performance Conclusion Adjustment > Calculate
- [x] Edit Performance Conclusion Adjustment > Calculate and Re-adjust
- [x] Edit Performance Conclusion Adjustment > View History
- [x] Delete Performance Conclusion Adjustment

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.performance.TPerformanceConclusionAdjustment"/>
  
```

</details>

TCK2111-0685350

>  Performance Management > Performance Monitoring

- [x] Melakukan Performance Monitoring , Verify Monitoring Period, Upload attachment pada tab Org Unit Objective
- [x] Melakukan Performance Monitoring , Verify Monitoring Period, Upload attachment pada tab Personal Objective

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.performance.performance_monitoring.TAddDelPerformanceMonitoringForm"/>

```
</details>

TCK2111-0685349

>  Performance Management > Performance Monitoring

- [x] View Request Status Performance Monitoring
- [x] lakukan filter dengan klik ikon filter di kanan atas
- [x] Download template Performance Monitoring
- [x] Upload Performance Monitoring
- [x] Delete Performance Monitoring dengan menggunakan ikon delete di kanan atas


##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.performance.performance_monitoring.TPerformanceMonitoringViewStatus"/>
  <class name="source.dataon.performance.performance_monitoring.TPerformanceMonitoringUpload"/>
  
```
</details>
</details>

---

<details>
<summary> <span style="color:orange">Selenium October</span></summary>

TCK2110-0678060

>  Performance > Performance Form
      
- [x] Add Simple Performance > draft
- [x] Add Simple Performance > send
- [x] View Request Status
- [x] Preview Final Score Report
- [x] Preview Employee Performance Rank
- [x] Preview Performance Status Report

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.performance.performance_form.TSimplePerformanceForm"/>
  <class name="source.dataon.performance.simplereport.TPerformanceStatusReport"/>
  <class name="source.dataon.performance.simplereport.TFinalScoreReport"/>
  <class name="source.dataon.performance.simplereport.TEmployeePerformanceRank"/>

```

</details>

TCK2110-0678419

>  Performance Management > Performance Planning

- [x] Mengubah Performance Planning - mengisi weight dan target kemudian draft
- [x] Mengubah Performance Planning - mengisi tab Training Plan- lakukan filter
- [x] Mengubah Performance Planning - mengisi tab Training Plan- Add Competency Gap lalu Add Row dan add competency gap kembali
- [x] Mengubah Performance Planning - mengisi tab Training Plan- Edit Competency Gap
- [x] Mengubah Performance Planning - mengisi tab Training Plan- Delete Competency Gap
- [x] Mengubah Performance Planning - mengisi tab Development Plan- lakukan filter
- [x] Mengubah Performance Planning - mengisi tab Development Plan- Add Row kemudian submit
- [x] Mengubah Performance Planning - mengisi tab Development Plan- Edit Description kemudian Submit
- [x] Mengubah Performance Planning - mengisi tab Development Plan- Edit Description kemudian Delete

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.performance.performance_planning.TPerformancePlanningForm"/>
  https://docs.google.com/spreadsheets/d/12s5tFyU1AB33HlAcWgv4vVW9ygzgv96c8gStbjMWg6A/edit?usp=sharing
  
```

</details>

TCK2110-0678426

>  Performance Management > Performance Planning

- [x] Mengubah Performance Planning - mengisi tab Career Plan- lakukan filter
- [x] Mengubah Performance Planning - mengisi tab Career Plan- Add Job Title From Career Path Map kemudian submit
- [x] Mengubah Performance Planning - mengisi tab Career Plan- Edit Job Title kemudian Submit
- [x] Mengubah Performance Planning - mengisi tab Career Plan- Edit Job Title kemudian Delete
- [x] View Competency Match
- [x] View Box Analysis
- [x] View Succession Plan
- [x] Mengubah Performance Planning kemudian Sent to Approver

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.performance.performance_planning.TPerformancePlanningForm"/>

```
</details>

TCK2109-0670827

>  Performance Management > Performance Planning

- [x] View Request Status Performance Planning
- [x] lakukan filter dengan klik ikon filter di kanan atas
- [x] Delete Performance Planning dengan menggunakan ikon delete di kanan atas
- [x] Melakukan Replace Performance Planning
- [x] Upload Performance Planning dengan type "Personal", Empty
- [x] Upload Performance Planning dengan type "Personal", Fill Template
- [x] Upload Performance Planning dengan type "Org Unit", Empty
- [x] Upload Performance Planning dengan type "Org Unit", Fill Template
- [x] Upload Performance Planning dengan Delete Previous Objective "Yes"


##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.performance.performance_planning.TPerformancePlanningFormOP"/>
  
```
</details>
</details>

---
<details>
<summary><span style="color:orange">Selenium September</span></summary>

TCK2109-0670360

>  Performance > Report > Advanced Performance Report > Box Analysis Report
      
- [x] Preview Box Analysis Report Org Unit All
- [x] Preview Box Analysis Report Org Unit Selected
- [x] Preview Box Analysis Report Group By Region
- [x] Preview Box Analysis Report Group By Organization Unit
- [x] Excel Box Analysis Report Org Unit All
- [x] Excel Box Analysis Report Org Unit Selected
- [x] Excel Box Analysis Report Group By Region
- [x] Excel Box Analysis Report Group By Organization Unit
- [x] Pdf Box Analysis Report Org Unit All
- [x] Pdf Box Analysis Report Org Unit Selected
- [x] Pdf Box Analysis Report Group By Region
- [x] Pdf Box Analysis Report Group By Organization Unit

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.performance.report.TBoxAnalysisReport"/>

```

</details>

TCK2109-0670822

>  Setting > Performance Setting > Performance Form Setting

- [x] Add Performance Form Setting by Admin
- [x] Add Performance Form Setting by User "Credit"
- [x] Add Performance Form Setting by User "Percentage"
- [x] Edit Performance Form Setting
- [x] Delete Performance Form Setting

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.setting.performance_setting.performance_form.TPerformanceFormSetting"/>
  
```

</details>

TCK2109-0670824

>  Setting > Performance Setting > Performance Form Setting

- [x] Set Question Performance Form Setting "All Positions"
- [x] Set Question Performance Form Setting "Certain Positions"
- [x] Set Question Performance Form Setting "Question Composition"
- [x] Preview Performance Form Setting Question For "All Positions"
- [x] Preview Performance Form Setting Question For "Certain Position"

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.setting.performance_setting.performance_form.TPerformanceSetQuestion"/>

```
</details>

TCK2109-0670827

>  Performance Management > Performance Form > Simple Performance Search <br>
>  Performance Management > Performance Form

- [x] Search Performance Form
- [x] Melakukan pengisian Performance Form Periodic (draft, send, delete)
- [x] Melakukan pengisian Performance Form Non Periodic (draft, send, delete)


##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.performance.TPerformanceForm"/>
  
```
</details>
</details>

---

<details>
<summary><span style="color:orange">Selenium Augst</summary>
TCK2107-0657443

>  Setting > Performance Setting > Box Analysis
      
- [x] Process Box Analysis Add
- [x] Reprocess
- [x] Process Box Analysis Delete

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.setting.performance_setting.box_analysis.TBoxAnalysisProcess"/>

```

</details>

TCK2108-0663934
- [x] Delete Box Analysis
- [x] Edit Box Analysis and set Matrix

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.setting.performance_setting.box_analysis.TSetMatrixBoxAnalysis"/>

```

</details>

TCK2108-0663933

- [x] Add Box Analysis data source x Axis dan y axis Total Performance
- [x] Add Box Analysis data source x Axis dan y axis OtherPerfomanceComp "Appraisal"
- [x] Add Box Analysis data source x Axis dan y axis OtherPerfomanceComp "Org Unit KPI"
- [x] Add Box Analysis data source x Axis dan y axis OtherPerfomanceComp "Personal KPI"
- [x] Add Box Analysis data source x Axis dan y axis OtherPerfomanceComp "Competency"
- [x] Add Box Analysis data source x Axis dan y axis OtherPerfomanceComp "Task"
- [x] Add Box Analysis data source x Axis dan y axis OtherPerfomanceComp "Feedback"

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.setting.performance_setting.box_analysis.TAddBoxAnalysis"/>

```
</details>

TCK2108-0663932

>  Setting > Performance Setting > Succession Parameter

- [x] Add Succession Parameter Within Same Job Family "Yes"
- [x] Add Succession Parameter Job Family Level "Same Level"
- [x] Add Succession Parameter Minimum Readiness, Maximum Possibility of Leaving, Maximum Impact of Leaving "Low"
- [x] Add Succession Parameter Minimum Readiness, Maximum Possibility of Leaving, Maximum Impact of Leaving "Medium"
- [x] Add Succession Parameter Minimum Readiness, Maximum Possibility of Leaving, Maximum Impact of Leaving "High"
- [x] Edit Succession Parameter
- [x] Delete Succession Parameter


##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.setting.performance_setting.succession_param.TSuccessionParameter"/>

```
</details>
<br>
</details>

---
<details>
<summary><span style="color:orange">Selenium July</span></summary>
TCK2107-0657443

>  Setting > Performance Setting > Competency Library
      
- [ ] Competency Matrix by Job Family set Configure with Excel "Yes"
- [ ] Competency Matrix by Job Title set Configure with Excel "Yes"
- [ ] Competence Point

TCK2107-0657442

>  Setting > Performance Setting > Performance Period Setting

- [x] Edit Performance Period dengan ubah bagian General (selain bagian Period Component)
- [x] Edit Performance Period dengan ubah bagian Apprisal-Remove Configuration
- [x] Edit Performance Period dengan ubah bagian Org Unit KPI-Remove Configuration
- [x] Edit Performance Period dengan ubah bagian Personal KPI-Remove Configuration
- [x] Edit Performance Period dengan ubah bagian Apprisal-Remove All Configuration
- [x] Edit Performance Period dengan ubah bagian Org Unit KPI-Remove All Configuration
- [x] Edit Performance Period dengan ubah bagian Personal KPI-Remove All Configuration

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.setting.performance_setting.performance_period_editonly.TEditPerformanceOrgUnitKPI"/>
  <class name="source.dataon.setting.performance_setting.performance_period_editonly.TEditPerformancePeriodAppraisal"/>
  <class name="source.dataon.setting.performance_setting.performance_period_editonly.TEditPerformancePersonalKPI"/>
  <class name="source.dataon.setting.performance_setting.performance_period_editonly.TEditPerformancePeriodCompetency"/>

```
</details>
<br>
TCK2107-0657441

>  Setting > Performance Setting > Performance Period Setting

- [x] Edit Performance Period dengan ubah bagian General (selain bagian Period Component)
- [x] Edit Performance Period dengan ubah bagian Apprisal-submit
- [x] Edit Performance Period dengan ubah bagian Org Unit KPI-submit
- [x] Edit Performance Period dengan ubah bagian Personal KPI-submit
- [x] Edit Performance Period dengan ubah bagian Competency-submit
- [x] Edit Performance Period dengan ubah bagian Task
- [x] Edit Performance Period dengan ubah bagian Feedback
- [x] Delete Performance Period
- [x] Preview Form (Ikon pada kolom Preview)
##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.setting.performance_setting.performance_period_editonly.TEditPerformanceCompGeneral"/>
  <class name="source.dataon.setting.performance_setting.performance_period_editonly.TPerformancePeriodPreview"/>

```

</details>
<br>
TCK2107-0657439

>  Setting > Performance Setting > Performance Period Setting

- [x] Add Performance Period dengan Period Component "Appraisal", centang Set Configuration With Excel "Default"
- [x] Add Performance Period dengan Period Component "Appraisal", centang Set Configuration With Excel "Weight, Target, Achievement Type"
- [x] Add Performance Period dengan Period Component "Org Unit", centang Set Configuration With Excel "Default"
- [x] Add Performance Period dengan Period Component "Org Unit", centang Set Configuration With Excel "Org Unit"
- [x] Add Performance Period dengan Period Component "Org Unit", centang Set Configuration With Excel "Weight, Target, Achievement Type"
- [x] Add Performance Period dengan Period Component "Personal KPI", centang Set Configuration With Excel "Library"
- [x] Add Performance Period dengan Period Component "Personal KP", centang Set Configuration With Excel "Position"
- [x] Add Performance Period dengan Period Component "Personal KP", centang Set Configuration With Excel "Weight, Target, Achievement Type"

##### Script

<details>
<summary> Script Class </summary>

```JAVA

  <class name="source.dataon.setting.performance_setting.performance_period_editonly.TEditPerformanceUploadConf"/>

```

</details>
</details>

---

<details>
<summary><span style="color:orange">Selenium June</span></summary>
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
</details>
<br>
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
<br>
</details>

---

<details>
<summary> <span style="color:orange">Selenium May</span></summary>

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
<br>
</details>

---

<details>
<summary><span style="color:orange">Selenium Maret</span></summary>

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
<br>
</details>

---

<details>
<summary><span style="color:orange">Selenium Maret</span></summary>

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
<br>

---
### <span style="color:orange">Selenium 01 Mar -31 Mar 2021</span>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium Desember</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange"> Selenium 10 Nov - 11 Nov 2020_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 28 Sep - 02 oct 2020_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange"> Selenium 14 Sep - 18 Sep 2020_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 08 Sep - 11 Sep 2020_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 31 Aug - 03 Sep 2020_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 20 Jul - 24 Jul 2020_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 13 Jul - 17 Jul 2020_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 6 Jul - 10 Jul 2020_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 29 June - 03 July_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 22 June - 26 June_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 15 June - 19 June_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 8 June - 12 June_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 2 June - 5 June_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 14 May - 18 May_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 05 May - 15 May_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 13 Apr - 17 Apr_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 6 Apr - 9 Apr_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 30 Mar - 3 Apr_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 23 Mar - 27 Mar_</span></summary>

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
</details>

---

<details>
<summary><span style="color:orange">Selenium 9 Mar - 20 Mar_</span></summary>

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
</details>

---

### Learn Selenium : _21 Feb - 6 Mar_
