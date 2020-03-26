# Health values

:hospital::mask: Inhalation health benchmarks and references

<div class="well">
    
## To do

1. [ ] Add these fields for new pollutants:
    - `Persistent Bioaccumulative Toxicants`	
    - `Respiratory Sensitizers`
    - `Developmental Toxicants`
1. [ ] Check early life adjustment for new pollutants
1. [ ] Auto-add adjustments to risks in RASS?
1. [ ] Check health endpoints for new pollutants
1. [ ] Q's for MDH
    - Cancer risk for Formaldehyde and Naphthalene
1. [ ] Address Monika's Q's
1. [ ] Drop `is pollutant a HAP` column?
1. [ ] Update change log

</div>

# Hierarchy of sources

Benchmarks are selected using the following hierarchy:

1. [Minnesota Department of Health](https://www.health.state.mn.us/communities/environment/risk/guidance/air/table.html)
    - Risk Assessment Advice
    - Health Based Values
    - Inhalation toxicity values in the ISV spreadsheet
    - Health Risk Values - [SONAR](https://www.health.state.mn.us/communities/environment/risk/docs/rules/hrvsonar.pdf) _(PDF)_
    - MDH site specific values
2. [EPA IRIS](https://www.epa.gov/iris)
3. [Cal EPA OEHHA RELs](https://oehha.ca.gov/air/general-info/oehha-acute-8-hour-and-chronic-reference-exposure-level-rel-summary) & [PDF Table](https://ww3.arb.ca.gov/toxics/healthval/contable.pdf)
4. [CDC ATSDR](https://www.atsdr.cdc.gov/mrls/mrllist.asp)
5. [EPA PPRTVs](https://www.epa.gov/pprtv/provisional-peer-reviewed-toxicity-values-pprtvs-assessments)


## Downstream tools

1. [Air monitoring data explorer](https://www.pca.state.mn.us/air/air-toxics-data-explorer)
1. [Air toxics values webpage](https://public.tableau.com/profile/mpca.data.services#!/vizhome/Airtoxicityvalues/Airtoxicityvalues)
1. [MNRISKS modeling tools](https://www.pca.state.mn.us/air/air-modeling-and-human-health)
1. AERA background monitoring risks
1. [AERA RASS](https://www.pca.state.mn.us/air/aera-forms-and-tools)
1. [Web RASS](https://mpca.shinyapps.io/fairscreen/) _on hold_

> __Check for other risk screening tools__
>    - Env Review
>    - Permitting
>    - Remediation

<br>


# Change Log :notebook:

Notable changes:

### 2019-03-15
    79-01-6	Trichloroethylene	2	MDH RAA	6	RAA	Acute	Reproductive
    Multiple	carcinogenic PAHs-relative potency factors stayed the same	6.00E-04	EPA IRIS unit risk	0.0011	Cal EPA unit risk	Chronic	Cancer
    156-60-5	Dichloroethylene, 1,2-trans-		MDH advice	60	PPRTV	Chronic	Noncancer
    100-00-5   	Chloronitrobenzene, p-   	2	PPRTV	6	PPRTV	Chronic 	Noncancer
    142-82-5	Heptane, N	400	PPRTV			Chronic 	Noncancer
    142-82-5	Heptane, N	4000	PPRTV			Subchronic	Noncancer
    76-13-1	Trichloro-1,2,2-trifluoroethane, 1,1,2-	5000	PPRTV			Chronic 	Noncancer
    76-13-1	Trichloro-1,2,2-trifluoroethane, 1,1,2-	50000	PPRTV			Subchronic	Noncancer
    420-46-2	Trifluoroethane, 1,1,1-	20000	PPRTV			Chronic 	Noncancer
    420-46-2	Trifluoroethane, 1,1,1-	200000	PPRTV			Subchronic	Noncancer
    463-58-1	Carbonyl sulfide	660	Cal EPA			Acute	Noncancer
    101-68-8	Methylene diphenyl diisocyanate (MDI)	12	CAL EPA			Acute	Noncancer
    584-84-9	Toluene diisocyanate, 2,4-	2	CAL EPA			Acute	Noncancer
    91-08-7	Toluene-2,6-diisocyanate	2	CAL EPA			Acute	Noncancer
    00-07-7	Petroleum Hydrocarbons, Aliphatic (C7 - C11)		HBV never completed	5000	HBV	Chronic 	Cancer
    60-34-4	Methyl Hydrazine		PPRTV not published	0.1	PPRTV	Chronic 	Cancer


### 2018-19-07
- Benzo(a)pyrene(BaP) added inhalation non-cancer RfC of `0.002` from IRIS

### 2018-04-04

#### Changes
- Trichloroethylene(79-01-6) acute value updated to MDH RAA from 2,000 to 6 ug/m3.

### 2018-02-01

#### Changes
- Arsine(7784-42-1) cancer IHB removed. Was previously assumed equivalent to Arsenic.


### 2017-04-01

#### Changes
- MPSFs for Lead and Lead compounds updated to align with IRAP modeling results. This corrects for the previous modeling using the default _Henry's Law constant_ assigned to inorganic metals.
- All inhalation health benchmarks rounded to 2 significant digits
- All of MDH's HRV and HBV chronic inhalation health benchmarks rounded to 1 significant digit, except for benzene
- Tetrachloroethylene (Perchloroethylene) non-cancer IHB updated from 100 to 15 ug/m3 per MDH guidance dated July 2014
- Napthalene cancer IHB set to 9 ug/m3 per MDH guidance dated Feb. 2017
- Ethylene Oxide cancer IHB set to EPA's IRIS value updated Feb. 2017
- Trimethylbenzenes non-cancer IHB set to EPA's IRIS value updated Sept. 2016
- Ethanol specific risk values identified in references, rather than on separate rows
- Chromic acid mists and dissolved Cr(VI) aerosols CAS# changed to _18540-29-9-aer_

#### Bug fixes
- Benzo(k)fluoranthene CAS# changed to _207-08-9_  
- Furfural CAS# changed to _98-01-1_  
- Formic Acid (ethanol facility) CAS# changed to _64-18-6_
- Ethylene dibromide (Dibromoethane) changed to _Ethylene dibromide (1,2-Dibromoethane)_
- Methylene Bromide CAS# 74-95-3 changed to _Dibromomethane (Methylene Bromide)_
