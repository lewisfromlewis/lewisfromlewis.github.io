---
title: "The RDH ICU DVT Story"
author: "Lewis Campbell"
date: "23 August 2018"
output:
    html_document:
        theme: paper
        keep_md: true
        toc: true
        toc_float: true
        toc_depth: 4
---



# DVT audit

After an adverse event we reviewed our practice in thromboprophylaxis (prevention of DVTs). Data collected in this audit covers the same subject as part of the binational registry held by ANZICS-CORE. Previous audits had focused on the **process** of thromboprophylaxis: whether a drug or device had been given according to our protocol. In this report we'll call a failure to act according to the protocol a *"disruption"* because it's a cooler word than *"failure"*. The previous audits were also ad-hoc, time consuming and depended on the judgment, enormous expertise and experience of the auditor. Those audit designs were therefore not reproducible and led naturally to producing too many single-event disruptions to produce a clear and predictable recommendation. The audits were largely conducted according to a timed schedule rather than targeted to disruptions found in previous results.

## Aims

We wanted an audit that would:

1. respond to concerns over longer run event rates
    - without being simply reactive to emotive single events
    
2. allow us to track the progress of initiatives

3. start simple, with a process audit
    - but allow surrogate or actual measures of event rates to be built into the auditing scheme later on

4. act as a model for audits of other topics

In short, we wanted it literate, expandable and reproducible.

## Reporting plan

We decided that a common **definition** for these disruptions was important, so the definitions are coded.^[
Any lack of thromboprophylaxis where it's indicated; any patient-relevant deviation from protocol such as "wrong" dose; any time something is done without a medical order
]
It's also very important that we can **update** these definitions across the whole set of auit runs, as long as we have the data in all the runs.  So if we decide that receiving IPC without a medical order is simply good nursing initiative, then we could redefine that and report separately.

The **report from each run** is of interest because we want an ability to review any disruptions.  We don't want that to consume the time of the audit. In fact, it's a bit of a distraction from the long run work of improving the whole system.  So we will simply copy the chart of any patient where the audit detects a disruption and send it to the responsible specialist for comment and action.

The report from the **long run** is of more interest, because the trend will tell us about what our true stable behaviour is, and whether it responds to any initiatives.  As of the end of August 2018 that is a work in progress.

## Report of run


This is an automated report prepared using [rStudio](https://www.rstudio.com) to generate deidentified reports from an input file which is structured according to our [data management practice](https://lewisfromlewis.wordpress.com/2017/10/16/a-workflow-for-analysing-data-from-my-icu/) than we usually use and prettified using [markdown](https://bookdown.org/yihui/bookdown) integrated with rStudio. Version control and publishing is done by [git](https://github.com/lewisfromlewis/DVT).

This was run number 1 of the audit, performed on 14/08/2018. In this run there were 20 patients and data was gathered on their thromboprophylaxis in the first 24 hours of the current admission, using the [unit policy](http://internal.health.nt.gov.au/PGC/dm/_layouts/WordViewer.aspx?id=/pgc/dm/Documents/TEHS/Royal%Darwin%Hospital/Anaesthetics/Anticoagulat%20and%20Antiplatelet%20Administration%20-%20Perioperative%20NT%20Hospitals%20Guideline.docx&DefaultItemOpen=1) as the standard.


Firstly,there were  the patients identified by this audit as not having received DVT prophylaxis appropriately. These might be because they did not receive either chemical or mechanical prophylaxis when it was indicated, or they received prophylaxis that was not indicated.

Table: Problems identified by the auditor on this run

Contra Hep   Contra Type   Chemical order   Dose per protocol   Doses as Rx   OAC   Contra Mech   Mech order   Mech on   Chart Copied 
-----------  ------------  ---------------  ------------------  ------------  ----  ------------  -----------  --------  -------------
Y            ICH           N                N                   Y             NA    N             N            N         Y            
Y            CLP           Y                Y                   Y             NA    N             N            N         Y            
N            NA            N                N                   Y             NA    N             Y            N         N            
Y            PSH           N                N                   Y             NA    N             N            N         Y            

Now we'll spend a couple of pages checking on the patterns of how errors seem to happen and how that's changed over the audits.

Table: Heparin not given, or not given properly, where there was no contraindication

Contra Hep   Contra Type   Chemical order   Dose per protocol   Doses as Rx   OAC    Contra Mech   Mech order   Mech on   Chart Copied 
-----------  ------------  ---------------  ------------------  ------------  -----  ------------  -----------  --------  -------------
N            NA            N                N                   Y             NOAC   N             N            N         Y            
N            NA            N                N                   Y             NA     N             Y            N         N            



Table: Mechanical prophylaxis given without an order

Contra Hep   Contra Type   Chemical order   Dose per protocol   Doses as Rx   OAC   Contra Mech   Mech order   Mech on   Chart Copied 
-----------  ------------  ---------------  ------------------  ------------  ----  ------------  -----------  --------  -------------
N            NA            Y                Y                   W             NA    N             N            Y         Y            

## What next?
The results of this audit will now be appended to the Story So Far. The collected patient records are now stored as All_patients1.csv, and the next CRF to complete is the blank file DVT_Audit_run2.csv. The next auditor needs to fill it out according to the [Audit Guide](Sorry. This doesn't have a link yet), making sure to put the correct Run number, then save it in the same place they found it.



Thanks for reading!
