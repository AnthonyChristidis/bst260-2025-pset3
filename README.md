# Problem Set 3: Data Wrangling, Visualization, and Exploratory Data Analysis with tidyverse

## Overview

This assignment focuses on advanced data manipulation, visualization, and exploratory data analysis using the tidyverse ecosystem. You'll explore potential differences in systolic blood pressure across racial groups using the NHANES dataset, investigate confounders like age and smoking, and create publication-quality tables and visualizations.

## Getting Started

1. **Accept the assignment** via the GitHub Classroom link
2. **Clone this repository** to your local machine
3. **Open the repository folder** in RStudio as a project
4. **Complete all problems** in the `pset-03-data-wrangling.qmd` file

## Assignment Files

- `pset-03-data-wrangling.qmd` - Main assignment file with all 18 problems
- `README.md` - This instruction file

## Technical Requirements

### Required Packages

- **dplyr** - Data manipulation and transformation
- **tidyr** - Data reshaping and tidying
- **forcats** - Working with factor variables
- **ggplot2** - Data visualization
- **knitr** - Table formatting with `kable`
- **NHANES** - Health survey dataset

### Key Constraint: Single Pipe Operations

- **All solutions must use a single pipe (`|>`) chain** - no intermediate variables
- Code can span multiple lines but must be one continuous operation
- Focus on chaining tidyverse functions together efficiently

### Key Concepts Covered

- **Data filtering and manipulation** - Using `filter()`, `select()`, `mutate()`
- **Grouping and summarization** - `group_by()` and `summarize()` operations
- **Data visualization** - Creating plots with `ggplot2`
- **Table formatting** - Professional tables with `kable()`
- **Descriptive statistics** - Means, standard deviations, confidence intervals
- **Exploratory data analysis** - Investigating confounders and group differences
- **Factor manipulation** - Combining and reordering categories with `forcats`

## What You'll Create

By the end of this assignment, your repository should have this structure:

**Root Directory:**

- `pset-03-data-wrangling.qmd` - Main assignment file with all 18 problems
- `pset-03-data-wrangling.html` - Rendered HTML output  
- `README.md` - This instruction file

## Assignment Structure

**18 Problems covering:**

- **Problems 1-2**: Basic NHANES data filtering and descriptive statistics
- **Problems 3-5**: Grouped analysis and confidence intervals
- **Problems 6-8**: Age as a confounder - tables and visualizations  
- **Problems 9-10**: Data restructuring and sample size considerations
- **Problems 11-13**: Stratified analysis and group comparisons
- **Problems 14-15**: Additional confounders (BMI and smoking)
- **Problems 16-18**: Advanced visualization and comprehensive exploratory analysis

## Key Instructions

1. **Use single pipe operations** for all problems - no intermediate variables
2. **Format tables with kable()** - never display raw dataframes
3. **Use two significant digits** for all numeric displays
4. **Create publication-quality graphs** with proper labels and titles
5. **Show both code and output** in your rendered document

## Technical Tips

- **Pipe chaining**: Connect multiple operations with `|>` 
- **Table formatting**: Always use `kable()` for displaying results
- **Confidence intervals**: Use formula $\bar{X} \pm 1.96 \, s / \sqrt{n}$
- **Factor manipulation**: Use `fct_collapse()` to combine factor levels
- **Missing data**: Handle `NA` values appropriately in calculations
- **Visualization**: Include proper axis labels, titles, and captions

## Dataset Information

**NHANES (National Health and Nutrition Examination Survey)**

- 10,000 observations with 76 variables
- Focus on 2011-2012 survey year (5,000 observations)
- Key variables: `BPSysAve`, `Race3`, `Gender`, `AgeDecade`, `BMI`, `Smoke100`
- Explore health disparities across demographic groups

## Submission

Your submission is your final committed and pushed repository. Make sure to:

1. **Complete all 18 problems** in the assignment file
2. **Render your document to HTML** successfully
3. **Include both .qmd and .html files** in your submission
4. **Use proper formatting** with kable for all tables
5. **Commit your changes** with meaningful messages
6. **Push your final work** to GitHub
7. **Verify** that all code and output are visible in your GitHub repository

## Due Date

**September 26, 2025, 11:59 PM**

## Getting Help

- Post questions on our class Slack in the #pset-03 channel
- Attend office hours for coding and data visualization help
- Review course materials on tidyverse and ggplot2
- Check function documentation using `?function_name`

## Common Pitfalls to Avoid

- **Creating intermediate variables** (use single pipe chains)
- **Displaying raw dataframes** (always use `kable()`)
- **Forgetting to handle missing values** in calculations
- **Poor plot labeling** (missing titles, axis labels, captions)
- **Incorrect confidence interval calculations**
- **Not filtering out missing data** before analysis

## Grading

| **Criteria** | **Excellent (A)** | **Good (B)** | **Satisfactory (C)** | **Needs Improvement (D-F)** |
|:-------------|:------------------|:-------------|:---------------------|:---------------------------|
| **tidyverse Proficiency & Pipe Usage (30 points)** | 27-30: Perfect use of single pipe chains, efficient tidyverse operations, no intermediate variables. Demonstrates mastery of dplyr/tidyr workflow. | 24-26: Good pipe usage with minor inefficiencies. Most operations properly chained together. | 18-23: Some proper pipe usage but creates unnecessary intermediate variables or inefficient operations. | 0-17: Poor pipe usage, creates many intermediate variables, doesn't follow single-pipe constraint. |
| **Data Manipulation & Descriptive Analysis (25 points)** | 23-25: Excellent data filtering, grouping, and summary calculations. Perfect confidence interval calculations and proper handling of confounders. | 20-22: Good data manipulation with minor errors in calculations or group operations. | 15-19: Basic data manipulation but misses some key operations or has calculation errors. | 0-14: Poor data manipulation, major errors in filtering, grouping, or calculations. |
| **Visualization with ggplot2 (20 points)** | 18-20: Beautiful, publication-quality plots with proper labels, titles, captions. Excellent use of faceting, colors, and geometric elements. | 16-17: Good visualizations with minor labeling or aesthetic issues. Plots are clear and informative. | 12-15: Basic plots created but missing some labels, poor aesthetics, or unclear presentation. | 0-11: Poor or missing visualizations, major labeling problems, or plots don't convey intended information. |
| **Table Formatting & Presentation (15 points)** | 14-15: All tables perfectly formatted with kable, appropriate significant digits, clear column names. Professional presentation throughout. | 12-13: Good table formatting with minor issues in presentation or significant digits. | 9-11: Basic table formatting but some raw dataframes shown or poor formatting choices. | 0-8: Poor table presentation, displays raw dataframes, missing kable usage, or unclear formatting. |
| **Code Organization & Documentation (5 points)** | 5: Exceptionally clean, well-commented code. Clear logic flow, excellent variable naming, easy to follow. | 4: Good code organization with minor documentation gaps. Code is readable and well-structured. | 3: Basic code organization but some unclear sections or missing comments where needed. | 0-2: Poor code organization, unclear logic, missing documentation, or difficult to follow. |
| **Technical Requirements & Submission (5 points)** | 5: Document renders perfectly, all required packages used correctly, proper HTML output, excellent GitHub submission. | 4: Meets technical requirements with minor issues. Document renders successfully. | 3: Some technical issues but document renders and meets basic requirements. | 0-2: Major technical problems, rendering failures, or incomplete submission. |

## Key Assessment Points

**Specific Things Graders Will Look For:**

1. **Single pipe operations**: All problems solved without intermediate variables
2. **Proper kable usage**: No raw dataframes displayed, all tables formatted
3. **Correct descriptive calculations**: Means, standard deviations, confidence intervals
4. **Quality visualizations**: Proper ggplot2 usage with complete labeling
5. **Data handling**: Appropriate treatment of missing values and factor manipulation
6. **Exploratory insights**: Understanding patterns in age, BMI, and smoking distributions

**Common Deductions:**

- Creating intermediate variables instead of using pipes (-3 points per instance)
- Displaying raw dataframes instead of kable tables (-2 points per table)
- Missing or incorrect confidence interval calculations (-5 points per problem)
- Poor plot labeling or missing titles/captions (-3 points per plot)
- Incorrect handling of missing data (-3 points per problem)
- Document rendering failures (-10 points)

This rubric emphasizes the **data wrangling skills** and **exploratory data analysis** essential for modern data science workflows.

## Resources

- **NHANES package documentation**: `help(package = "NHANES")`
- **Dataset structure**: `str(NHANES)` after loading the package
- **tidyverse cheat sheets**: RStudio cheat sheets for dplyr, ggplot2
- **ggplot2 reference**: Course materials on data visualization
- **Exploratory data analysis**: Review materials on confounders and descriptive statistics
