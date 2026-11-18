# Bloomberg Industry Group Investigations - Staff-Linked Homicides in Jails and Prisons

## Terms of Use

By downloading the Dataset, you agree that you will attribute the Dataset and any use of the Dataset to Bloomberg Industry Group and/or Bloomberg Law. You may use the Dataset for personal or internal business purposes, and may make limited use of the Dataset in connection with the provision of other services to clients; provided that you may not monetize the Dataset or otherwise make commercial use of the Dataset where the Dataset constitutes all, or substantially all, of the commercial offering. The Dataset is provided "as-is" and without any express or implied warranties.

## Introduction

This repository contains a database of 71 individuals who were beaten, suffocated, neglected, or restrained by jail staff in the past ten years and whose deaths were ruled homicides by a government pathologist. The database accompanies a Bloomberg Law investigation into the consequences jailers faced after those deaths. The story, "When Jailers Kill People in Custody, Few Face Criminal Charges," was published on Nov. 19, 2026.

## How the Database was Constructed

Most homicides in this database are drawn from more than 275,000 civil rights complaints filed in federal district court from Jan. 1, 2017 to Dec. 31, 2025. The reporting team used large language models to generate summaries of the complaints and then examined them.

Additional homicides were uncovered in law enforcement custodial death reports and state data. We limited our analysis to deaths documented between 2015 and early 2025.

To investigate and confirm homicides committed by detention center staff, Bloomberg Law submitted more than 90 public records requests for autopsy reports, death investigation summaries, district attorney memos, and jail surveillance footage.

All homicides included in our analysis were independently confirmed by an autopsy report, death certificate, or other government source.

## Data Description

-   `Database of Staff-Linked Detainee Homicides.csv` - A comma-separated values file of jail and prison detainee deaths that were ruled a homicide.

## Data Dictionary

| Data Field | Description | Data Type |
|------------------------|------------------------|------------------------|
| `deceased` | The name of the deceased detainee whose death was ruled a homicide | string |
| `jail_prison_name` | The name of the detention facility where the detainee was incarcerated | string |
| `city` | The city where the detention facility is located | string |
| `county` | The county where the detention facility is located | string |
| `state` | The state where the detention facility is located | string |
| `death_year` | The year the death occurred | integer |
| `charges_filed` | Details on whether the death led to criminal charges filed against jail or prison staff | string |
| `outcome` | Outcome of criminal cases when charges were filed (blank if no charges filed) | string |
