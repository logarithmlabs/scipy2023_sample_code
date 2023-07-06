# Motivation

The semiconductor industry has followed Moore's law for over 50 years, with increasing demand for faster chips in AI, mobile devices, and automation. It has become challenging for upstream chemical suppliers to identify and control critical material parameters in semiconductor manufacturing. 

DuPont's semiconductor quality focus was to maintain 6-sigma control on all process parameters for 20 years, reducing out-of-control(OOC) performance at customers. However, some materials that pass 6-sigma checks are still OOC when used. To reduce customer issues, we are adopting a multivariate analysis approach in addition to 6-sigma control.

We aim to have complete visibility of material inputs- manufacturing parameters, test results, certificates of analysis, factory conditions, shipping/storage conditions, run analytics to identify critical variables, and proactively control the right parameters to optimize cost and prevent quality issues during fabrication.

The photolithography chemical manufacturing process involves precise regulation and monitoring, generating a lot of data, but these datasets are not stored centrally. Different teams use various tools (Excel, JMP, dashboards) to analyze them. Test results, equipment conditions, and logistics are stored and analyzed separately, introducing friction.

This highlights the need for organized data for analytics.

# Goals

We realized that the success of statistics/ML depends on accurate and readily available datasets for analysis. We focused our initial efforts on two primary targets.

* Availability: Data Extraction/Automation (relieve domain-experts manual data organization) 
* Accuracy: Data quality

# Methods

## Three phase Project

1. Assessment phase: We identified and documented data sources, systems and access patterns.

2. MVP phase: We created data pipelines, developed code patterns to access various kinds of data, and identified and corrected data quality issues. We built product models using PCA, PLS, and OPLS modeling to understand the product’s parameters' performance and how they are related to each other. We kept infrastructure complexity low during this phase.

3. Production phase: We engaged enterprise IT teams early to align with confidentiality and security requirements for data on the cloud, while meeting the quality team’s goals. We reused best practices, techniques and tools developed during the MVP to scale to multiple products, use cases and internal teams.

Data engineering, statistics/data science and product experts collaborated closely to ensure scalability to multiple processes and products. We used tools from the scientific python stack like pandas, jupyter, panel, numpy, pandas-profiling and open source python tools like openpyxl, sqlite3, pyodbc.


# Conclusion

A key to success with data projects in a large enterprise is demonstrating value to the team and progress at multiple stages. 

We followed consistent practices for the data pipeline, data sources, data discoverability, data quality, and code.

The scientific python data stack provides the tools needed to demonstrate this without large upfront infrastructure commitments before demonstrating value to the organization, while allowing us to iterate quickly. 

We summarize the tools and techniques used at every stage and hope practitioners in similar settings can apply our experiences and learnings to drive better data utilization and awareness in their organizations.
