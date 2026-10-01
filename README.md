# HUDK4054Indivisual-Assignment2
Write Readme Style Metadata 
<a id="top"></a>

<h1 align="center">🌙 🧠 ✨<br>Anxiety · Habits · Learning</h1>

<h3 align="center">Anxiety and Students' Learning Behaviors:<br>Considering Social Media Use and Sleep</h3>


<p align="center">🧠 Anxiety &nbsp; · &nbsp; 🌙 Sleep &nbsp; · &nbsp; 📱 Social media &nbsp; · &nbsp; 📚 Learning routines</p>

<p align="center">
  <a href="#project-status"><img src="https://img.shields.io/badge/Status-Research%20Proposal-A855F7?style=for-the-badge" alt="Status: research proposal"></a>
  <a href="#learning-analytics-connection"><img src="https://img.shields.io/badge/Field-Learning%20Analytics-0284C7?style=for-the-badge" alt="Field: learning analytics"></a>
  <a href="#dataset"><img src="https://img.shields.io/badge/Source%20Sample-3000%20Students-F59E0B?style=for-the-badge" alt="Source sample: 3000 students"></a>
  <br>
  <a href="#metadata-standard"><img src="https://img.shields.io/badge/Metadata-DDI%20Inspired-EC4899?style=for-the-badge" alt="Metadata: DDI inspired"></a>
  <a href="https://data.mendeley.com/datasets/rc5htd5dfr/1"><img src="https://img.shields.io/badge/Data%20License-CC%20BY%204.0-16A34A?style=for-the-badge" alt="Source data license: CC BY 4.0"></a>
  <a href="https://doi.org/10.17632/rc5htd5dfr.1"><img src="https://img.shields.io/badge/DOI-10.17632%2Frc5htd5dfr.1-6366F1?style=for-the-badge" alt="Source dataset DOI: 10.17632/rc5htd5dfr.1"></a>
  <a href="https://orcid.org/0009-0004-9329-1296"><img src="https://img.shields.io/badge/ORCID-Miho%20Suzuki-A6CE39?style=for-the-badge" alt="Miho Suzuki's ORCID"></a>
</p>


---

<a id="overview"></a>

## 🌈 Overview

As a student, I am interested in how anxiety relates to our learning routines. Students may experience anxiety while also having different sleep habits and patterns of social media use. Let's find out whether anxiety is related to attending classes and spending time studying when these daily habits are considered together.

This project uses an existing dataset to examine anxiety in relation to two learning behaviors: class attendance and daily study time. Social media use and sleep duration will be included in the analysis to examine whether anxiety remains associated with these behaviors after accounting for those habits.

> [!NOTE]
> **🧠 The question driving this project**
> Is anxiety associated with university students' class attendance and study time after accounting for social media use and sleep duration?

| 🧠 What I am curious about | 📚 What I will examine | 🌙 📱 What I will account for |
|---|---|---|
| Students' self-rated anxiety | Class attendance and daily study time | Sleep duration and social media use |

<a id="project-status"></a>

<a id="research-questions"></a>

## 🔎 Research Questions

1. Is anxiety associated with  <ins>class attendance</ins> when social media use and sleep duration are considered together?
2. Is anxiety associated with <ins>daily study time</ins> when social media use and sleep duration are considered together?
3. How does the estimated association between anxiety and each behavior differ before and after accounting for social media use and sleep?

These questions concern associations. Including social media and sleep in a regression accounts for measured differences in those variables, but does not establish that anxiety causes a change in learning behavior.

<a id="variables-at-a-glance"></a>

## 🎯 Variables at a Glance

| Role in this project | Variable | Interpretation |
|---|---|---|
| Main outcome | `Class_Attendance` | Attendance percentage during a semester |
| Secondary outcome | `Study_Hours` | Daily time spent studying |
| Main predictor of interest | `Anxiety_Level` | Self-rated anxiety on the documented rating scale |
| Additional predictor | `Social_Media_Use` | Daily time spent on social media |
| Additional predictor | `Sleep_Hours` | Daily sleep duration |

> [!TIP]
> **Reading the project:** Anxiety is the main predictor. Attendance is the main outcome, and study time is the secondary outcome. Sleep and social media use are included in both models.

<a id="learning-analytics-connection"></a>

<a id="dataset"></a>

## 🗂️ Dataset

| Item | Information |
|---|---|
| Dataset title | University Student Stress Dataset |
| Repository | Mendeley Data |
| Version | 1 |
| Publication year | 2025 |
| Source DOI | [10.17632/rc5htd5dfr.1](https://doi.org/10.17632/rc5htd5dfr.1) |
| Population described by the creators | Undergraduate students in Bangladesh |
| Source sample size | 3,000 responses |
| Age coverage | 19–24 years |
| Variables | 18 columns |
| Unit of observation | One student's response per row |
| Source data license | CC BY 4.0 |

The creators report an anonymous Google Forms survey distributed by email to 3,710 students, with 3,000 complete responses retained. This project is a secondary analysis; I did not collect these responses. See the [original dataset record](https://data.mendeley.com/datasets/rc5htd5dfr/1) for provenance.

### Source Files

The dataset package has five folders: `Raw_Responses`, `Cleaned_Data`, `Documentation`, `Code`, and `Figures`. The main file for this project is:

`Cleaned_Data/university_student_stress_dataset.csv`

The source documentation includes a variable description table. It should be read alongside the cleaned data because some documented values differ from the CSV.


<a id="data-dictionary"></a>

## 📖 Data Dictionary

This dictionary covers all 18 columns. Units and documented scales come from the source variable description table. **Observed values** below come from the Mendeley cleaned CSV preview; they are not automatically the full set of allowable survey responses.

<details open>
<summary><strong>📖 Full data dictionary — all 18 variables (click to fold or expand)</strong></summary>

| Variable | Readable name and meaning | Type in cleaned CSV | Units / documented values | Observed values in CSV preview |
|---|---|---|---|---|
| `Age` | Student age | Integer | Years | 19–24 |
| `Gender` | Gender category | Categorical | Male, Female, Other documented | Male, Female |
| `Study_Hours` | Daily study duration | Integer | Hours per day | 0–9 |
| `Class_Attendance` | Attendance during a semester | Integer | Percentage | 40–99 |
| `Tuition` | Extra coaching participation | Categorical | Yes / No; not a tuition-fee amount | Yes, No |
| `Exam_Frequency` | Exam frequency rating | Integer rating | 1–10 rating | 1–9 |
| `Assignment_Load` | Assignment workload rating | Integer rating | 1–10 rating | 1–9 |
| `Sleep_Hours` | Daily sleep duration | Integer | Hours per day | 4–9 |
| `Social_Media_Use` | Daily social media use | Integer | Hours per day | 0–7 |
| `Screen_Time` | Total daily screen use | Integer | Hours per day | 1–11 |
| `Physical_Exercise` | Exercise indicator in cleaned data | Categorical | Codebook says days per week; CSV uses Yes / No | Yes, No |
| `Family_Income_Level` | Family income category | Ordered categorical | Low, Medium, High; monetary cutoffs unspecified | Low, Medium, High |
| `Peer_Pressure` | Self-rated peer pressure | Integer rating | 1–10 rating | 1–9 |
| `Family_Support` | Self-rated family support | Integer rating | 1–10 rating | 1–9 |
| `Anxiety_Level` | Self-rated anxiety | Integer rating | 1–10 rating; not a clinical diagnosis | 1–9 |
| `University_Type` | University category | Categorical | Public, Private, National University | Public University, Private University, National University |
| `Stress_Score` | Derived composite stress measure | Integer score | Score units; construction requires verification | Minimum −9; maximum 33 |
| `Stress_Level` | Category derived from stress score | Ordered categorical | Low, Medium, High | Low, Medium, High |

</details>

### Coding and Documentation Notes


<details>
<summary><strong>🔍 Measurement details and coding notes</strong></summary>

- **Model structure:** attendance and study time will be analyzed in separate models, each including anxiety, social media use, and sleep duration.
- **Stress variables:** `Stress_Score` and `Stress_Level` are documented for completeness but are not included in the proposed models because they are derived from other indicators.
- **Exercise mismatch:** do not convert Yes/No into days per week. Resolve the discrepancy before using exercise in a model.
- **Rating scales:** the codebook describes several 1–10 scales, while the CSV preview shows 1–9. A value of 10 is documented even though it was not observed in the preview.
- **Missing values:** no missing-value code is specified in the documentation reviewed. Check the downloaded file for blanks and sentinel codes before analysis. Do not treat zero as missing automatically.
- **Negative stress scores:** negative values appear in the CSV. Do not delete them merely because they are negative; verify the scoring rule first.
- **Derived variables:** the creators describe `Stress_Score` as combining academic, psychological, and lifestyle information, with `Stress_Level` derived from it. The exact formula and category thresholds must be checked in the source code.

</details>

<a id="analysis-plan"></a>

## 🧪 Analysis Plan

### 🧹 1. Inspect and Prepare the Data
download version 1 and retain an unchanged copy. I will check the row count, column names, data types, missing values, duplicate rows, and ranges. Any changes will be recorded separately.

### 📊 2. Describe the Variables
summarize anxiety, class attendance, study time, social media use, and sleep duration. 

### 🔗 3. Examine Associations
examine anxiety's relationship with attendance and study time separately. Also examine relationships among anxiety, social media use, and sleep to understand how the predictors relate to one another. 

### 🧮 4. Compare Regression Models

For each outcome,  compare a model containing anxiety alone with a model that also includes social media use and sleep duration. The two adjusted models are:

```text
Class_Attendance = β₀ + β₁(Anxiety_Level)
                      + β₂(Social_Media_Use)
                      + β₃(Sleep_Hours) + ε

Study_Hours = α₀ + α₁(Anxiety_Level)
                 + α₂(Social_Media_Use)
                 + α₃(Sleep_Hours) + ε
```

The main quantities of interest are the anxiety coefficients, β₁ and α₁. They describe the estimated difference in attendance percentage points or daily study hours associated with a one-point difference in anxiety rating, holding social media use and sleep duration constant in the model.

Compare the anxiety estimates before and after adding social media use and sleep. Treating anxiety as a numeric rating assumes a linear relationship across its scale; examine whether that assumption is reasonable. Attendance is bounded and study hours are nonnegative, so I will also check whether the models fit these outcomes appropriately.
Any adjusted association will remain exploratory. Accounting for two daily habits does not remove all possible alternative explanations, such as academic workload or differences between institutions.

### 💻 Planned Software

I plan to use Python with pandas for preparation, matplotlib or seaborn for plots, and statsmodels for regression.

<a id="limitations"></a>


<a id="data-access-and-sharing"></a>

## 🔓 Data Access and Sharing

Access the source through [Mendeley Data, version 1](https://data.mendeley.com/datasets/rc5htd5dfr/1), open `Cleaned_Data`, and download `university_student_stress_dataset.csv`. The source record offers public access.

The dataset is licensed under [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/). Reuse requires appropriate attribution, a license link, and an indication of changes. This badge refers to the **source dataset**, not a separate license for all future project code.

<a id="data-and-file-overview"></a>

## 📁 Data and File Overview

The current deliverable is `README.md`, which contains the project description, metadata, data dictionary, and analysis plan. The original dataset remains at Mendeley Data.

The following structure is **planned for future analysis**:

| File or folder | Purpose | Status |
|---|---|---|
| `README.md` | Research overview and dataset metadata | Included |
| `data/raw/university_student_stress_dataset.csv` | Unchanged downloaded source file | To be added |
| `data/processed/` | Working data with recorded transformations | Planned |
| `analysis/` | Analysis scripts or notebooks | Planned |
| `results/` | Tables and figures generated by this project | Planned |
| `requirements.txt` | Software versions needed to reproduce analysis | Planned |

The figures in the original dataset package belong to the dataset creators; they are not results from this proposed project.

<a id="ethical-considerations"></a>


<a id="metadata-standard"></a>

## 🏷️ Metadata Standard

I chose **DDI-Codebook** as the framework for documenting this dataset because it organizes study information, provenance, access, files, and variable definitions. These elements are useful for secondary analysis of student survey data.

This README follows a **DDI-inspired, human-readable structure**. It is written in Markdown and is not a schema-validated DDI XML document.

| DDI documentation area | README section |
|---|---|
| Study identification and purpose | Overview, Research Questions, Researcher Information |
| Source and methodology | Dataset, Analysis Plan |
| Data files | Source Files, Data and File Overview |
| Variable descriptions and derivation | Data Dictionary |
| Access and reuse | Data Access and Sharing, Citation |

Reference: [DDI-Codebook documentation](https://ddialliance.org/ddi-codebook).

<a id="researcher-information"></a>

## 👩🏻‍💻 Researcher Information

**Researcher:** Miho Suzuki  
**Program:** M.S. in Learning Analytics, Teachers College, Columbia University  
**Role:** Student researcher conducting a proposed secondary analysis  
**ORCID:** [0009-0004-9329-1296](https://orcid.org/0009-0004-9329-1296)  
**Project DOI:** Not assigned. The DOI in this README identifies the source dataset.

The ORCID above identifies me as the student researcher. The source dataset DOI identifies the data created by the original contributors.

<a id="template-and-software"></a>

## 💭 Reflection Draft
The most challenging part was connecting my interest in student anxiety and daily habits to an educational research question. I initially focused on stress, but I wanted the project to examine students' learning behaviors more directly. I chose attendance and study time as outcomes and made anxiety the main predictor, while considering social media use and sleep together. Creating the data dictionary helped clarify these roles and showed why the derived stress score requires caution. I also learned to distinguish associations from causal effects and learning behavior from learning achievement. I also had a lot of fun creating this README and making it colorful and playful. I gained ideas and inspiration from other repositories and YouTube tutorials. Practicing what I learned helped me make deeper connections between the ideas and remember them more clearly. This gave me knowledge I can use again in future projects.
<a id="citation"></a>
## 🎨 Template and Software

This file uses GitHub-flavored Markdown with simple HTML for the centered heading, colorful badge rows, and navigation. Emoji section markers, GitHub alerts, and expandable documentation make the research easier to browse. Its visual layout is inspired by the Clairvoyant and Markdownify examples referenced in the assigned video. The text and sections are adapted for a research project.

The badges use [Shields.io](https://shields.io/). [Make a README](https://www.makeareadme.com/) provides an organizational reference, and [OSF's data dictionary guide](https://help.osf.io/article/217-how-to-make-a-data-dictionary) informs the variable documentation.

<a id="reflection-draft"></a>
## 🔖 Citation
the original dataset creators:

Paul, Subrata Kumer; Paul, Rakhi Rani; Musa Miah, Abu Saleh; Hamid, Md. Ekramul; Rashidul Hasan, Mirza A.F.M. (2025). *University Student Stress Dataset* (Version 1) [Data set]. Mendeley Data. https://doi.org/10.17632/rc5htd5dfr.1

---

<p align="center">🌙 🧠 📚 ✨<br><strong>Behind every row is a student experience.</strong><br>
<p align="center"><a href="#top">⬆️ Back to the top</a></p>
