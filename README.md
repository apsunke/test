# Untitled

SNOWFLAKE VIRTUAL HANDS-ON LAB

Automating Data Pipelines to Drive Marketing Analytics with Snowflake & Fivetran

![A picture containing text

Description automatically generated](.gitbook/assets/0.png)

## 

Format & Agenda

* **5 Minute Introduction : Snowflake & Fivetran**
* **55 minutes of instructor-led content**
  * A Snowflake sales engineer will walk you through Snowflake UI orientation and Partner Connect \(following the lab guide\).
  * A Fivetran sales engineer will walk you through the Fivetran modules.
  * A Snowflake sales engineer will walk you through some of Snowflake’s unique features
* **30-minute Q&A**
* **1-2 sales engineers will answer questions that arise during the lab**

Hands on Lab Participant Materials

To participate in the virtual hands-on lab, attendees need the following:

1. **Prior to attending the lab**
   1. **Github account -** Participants will need to create, or already have, an account on Github. Other git-based source control hosting sites will work fine \(Gitlab, Bitbucket\), but the instructions will assume Github. An account on Github is free. [https://github.com/join](https://github.com/join). _See appendix 1 for step-by-step instructions._
   2. **Snowflake Free Trial** - Registrants of the virtual hands-on lab need to sign up for a [free trial](https://signup.snowflake.com/). Please sign up using an email address that hasn’t been used previously. _See appendix 2 for step-by-step instructions_**.**
   3. **OPTIONAL:** Log in to your Google account, if you have one.
   4. **OPTIONAL: Google Ads account credentials.**

Sample Google Ads data will be provided if you do not have a Google Ads account.

1. **During the lab**

* 1. [**Sample Google Ads data \(Google Sheets\)**](https://github.com/fivetran/snowflake_fivetran_vhol/blob/main/LAB_ASSETS/GSHEETS_LINKS.md) - a public Google Sheet with three workbooks. Each workbook will become a table in our sample Google Ads data schema. The above link takes you to a page full of Google Sheets links -- all of these sheets are copies of the same data, you can use any link on that page. 
  2. [**dbt Project Github Repository URL**](https://github.com/fivetran/snowflake_fivetran_vhol) **\(**[**https://github.com/fivetran/snowflake\_fivetran\_vhol**](https://github.com/fivetran/snowflake_fivetran_vhol)**\)** 
  3. [**SQL Script file**](https://github.com/fivetran/snowflake_fivetran_vhol/raw/main/LAB_ASSETS/vhol_script.sql.zip) **-** Participants will load [this file](https://github.com/fivetran/snowflake_fivetran_vhol/raw/main/LAB_ASSETS/vhol_script.sql.zip) into a Snowflake worksheet when prompted during the lab. Save this file where you can easily find it during the lab.

## 

## 

Lab Script

## INTRODUCTION

With the growth of your data and business, so does the complexity involved in traditional approaches and architecture. Snowflake and Fivetran have partnered to bring you the Data Cloud and the most automated data integration solution which helps customers simplify data pipelines for all your businesses so you can focus on your data and analytics instead of infrastructure management and maintenance. In this virtual hands-on lab, you will follow a step-by-step guide to perform marketing analytics for Google Ads data by using Fivetran, Snowflake, and dbt. Let’s get started.

## SNOWFLAKE - PART ONE

![Graphical user interface, application, website

Description automatically generated](.gitbook/assets/1.png)

1. Login to your Snowflake trial account.

![Graphical user interface, text, application, email

Description automatically generated](.gitbook/assets/2.png)

1.  UI Tour \(SE will walk through this live\). For post-workshop participants, click [here](https://docs.snowflake.com/en/user-guide/snowflake-manager.html#quick-tour-of-the-web-interface) for a quick tour of the UI.

![Graphical user interface, text, application

Description automatically generated](.gitbook/assets/3.png)

1. Let’s change our role and enable notifications. We need to work in the ACCOUNTADMIN role for this lab and notifications are how Snowflake will alert you when resource monitor thresholds have been crossed. Click on your User Name in the upper right-hand corner.

![Graphical user interface, application

Description automatically generated](.gitbook/assets/4.png)

1. You’ll get a popup with 4 items; click on Switch Role.

![Graphical user interface, application

Description automatically generated](.gitbook/assets/5.png)

1. Select ACCOUNTADMIN.

![Graphical user interface, text

Description automatically generated with medium confidence](.gitbook/assets/6.png)

1. The UI will refresh and you should see ACCOUNTADMIN under your username. If you don’t, go back to step 5.

