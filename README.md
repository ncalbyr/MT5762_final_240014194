MT5762: Introductory Data Analysis- Final Project




 Instructions
 
 Carefully read and follow the instructions below:
 
 • Submit your solution via MMS before 5pm on November 1, 2024. Penalties for late
 submissions will follow the school policy (an initial penalty of 15% of the maximum
 available mark, then a further 5% per 8-hour period, or a part thereof). Because of the
 significant initial penalty of 15%, you should not submit at the last minute.
 
 • The report should not exceed 5 pages in length, excluding appendices. The body
 should contain all relevant figures, references, and tables. Violating the page limit (or,
 similarly, extreme font or margin choices) will result in marks being deducted.
 
 • The report should contain the following sections: introduction, methods, results, and
 discussion. Also include an abstract of no more than 300 words (marks will be deducted if
 it is longer) written in plain language (i.e., something understandable to those interested
 in the topic but without statistical training). Read the document “Guidance on writing
 reports.docx”, which is on Moodle, before writing your report.
 
 • Include your R code as an appendix to your report (this is not subject to the page
 limit). Make sure that your R code is tidy and well-commented and that your results
 are reproducible.
 
 • Consider your target audience to be the managing board of Transport for London, the
 operator of the London bike sharing system, which has only a passing familiarity with
 statistics. However, also consider that statisticians may also read your report to confirm
 the validity of your claims, i.e., details are required, but should not interfere with the
 readability for a general audience.
 
 • Include references throughout the text as required and include a bibliography. Your
 references should generally be from peer-reviewed sources (which you can find using
 Google Scholar or similar). Random websites are not compelling references.
 
 • Analysis can be done in any software (e.g., R). Do not include raw computer output in
 the body of the report- make sure that any results you include are tidy (e.g., in a table)
 and are relevant. For writing your report, you can use any document preparation system
 
 (1)

(e.g., RMarkdown, Quarto, LaTeX, Google Docs, or MS Word), but the end product
 must be in .pdf form.
 
 Marking:

 
 A total of 50 marks are available, which will be allocated as follows:
 
 • 35 marks will be allocated for the correctness and completeness of the statistical anal
yses and the interpretations of the results (see breakdown in the next section).

 • 5 marks will be allocated for the abstract.
 
 • 10 marks will be allocated for the quality of the report. This includes the clarity of
 the exposition (including appropriate use figures and tables) and its utility for the target
 audience, proper referencing, and clarity of your code.
 
 (2)
 
Introduction: the data set

 Suppose that you are working as a data analyst for Transport for London (TfL), the operator
 of the London bike sharing system. Bike sharing systems are a new generation of bike rentals
 where the users can rent bikes from a particular station and return them at another one. The
 managing director of TfL is interested in the following questions:
 
 How do the variables given below affect the number of rented bikes, and how well can the
 number of bikes that will be rented tomorrow be predicted based on today’s weather forecast?
 
 The question is broken into more specific sub-questions below.
 
 You are given a data set1 containing 100 daily observations of the variables:

 
 • temperature (the maximum temperature in 𝑜C),
 
 • humidity (the average humidity in %),
 
 • windspeed (the average windspeed in km/h),
 
 • season,
 
 • weekend (0 if the day is a working day and 1 if it is a weekend),

 • holiday (0 if the day is not a holiday and 1 if it is a holiday), and
 
 • count (the number of rented bikes).

 The data set "Bike_sharing_2022.csv", is available on Moodle.
 
 Part 1 [5 marks]

 
 Conduct an appropriate exploratory analysis of the data that is informed by the questions
 posed in Parts 2 to 4 below.

 
 Part 2 [10 marks]


 
 Days with fewer than 35,000 rented bikes are not profitable for TfL. Therefore, the managing
 director of TfL asks you to estimate:

 
 a) the expected proportion of days with fewer than 35,000 rented bikes;
 
 b) a 90% confidence interval for that proportion;
 
 c) the expected proportion of days with fewer than 35,000 rented bikes for each season;
 
 d) whether there is a difference between the proportions in winter and spring.
 
 Make sure to include interpretations of your analyses above that are useful for the target
 audience.
 
 (1) The data set is powered by TfL Open Data.
 (3)
 
Part 3 [10 marks]



 Test whether the expected number of rented bikes varies across seasons. Interpret and explain
 your results. 
 
 Furthermore, test whether there is a difference between the expected number of
 bikes rented on working days and weekends. 
 
 Interpret and explain your results. 
 
 In addition, compute the power of the above test, assuming that the true difference is the one observed.
 
 For the observed sample size, what effect size (i.e., difference between the expected values)
 would be required to obtain a power of 80%? 
 
 For the given effect size, what sample size would be required to obtain a power of 80%? 
 
 Explain the implications of your results for the target audience.

 
 Part 4 [10 marks]


 
 Determine how the variables temperature, humidity, windspeed, season, weekend, and
 holiday affect the number of rented bikes. Interpret the estimated parameters of your model.
 Estimate the expected number that the TfL can expect to be rented on any given day, together
 with 95% bounds, for:

 
 a) a working day in spring with temperature 16𝑜C, 8% humidity, and 12 km/h windspeed;
 
 b) a holiday on a summer weekend with temperature 26𝑜C, 30% humidity, and 7 km/h
 windspeed;
 
 c) aworking day in autumn with temperature 10𝑜C, 85% humidity, and 30 km/h windspeed;
 
 d) a day on a winter weekend that is not a holiday with temperature-1𝑜C, 70% humidity,
 and 16 km/h windspeed.
 
