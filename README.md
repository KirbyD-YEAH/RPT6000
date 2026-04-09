# COBOL RPT6000
___

## Overview
___
The **RPT5000** program is an enhanced COBOL reporting tool designed to process customer sales data and generate a structured, year-to-date 
sales report organized by branch and sales representative.

Building upon the foundations of its predecessor (RPT3000), this version introduces control break processing, detailed sales comparisons, 
and formatted report output with pagination. It provides a clear summary of sales performance, including calculated changes in both dollar 
amount and percentage.

## Table of Contents
___
* [Key Functionalities](#key-functionalities)
* [Tech Stack](#tech-stack)
* [Installation](#installation)
* [Running Output](#running-output)
* [Learning Outcomes](#learning-outcomes)
* [Help](#help)
* [Authors](#authors)

### Key Functionalities
___
 * **EVALUATE** Statement
Used to simplify complex decision-making by replacing multiple IF statements, especially for handling control breaks and end-of-file processing.
 * 88-Level Condition Names
Improved readability by using condition names like CUSTMAST-EOF and NOT-FIRST-RECORD instead of raw values.
 * Control Break Processing
Implemented logic to detect changes in branch and sales representative, triggering subtotal calculations and formatted output sections.
 * Sequential File Processing
Read and processed fixed-format customer records from an input file, demonstrating structured batch processing.
 * Accumulation and Reset of Totals
Used ADD and MOVE ZERO to maintain and reset running totals for sales representatives, branches, and grand totals.
 * Arithmetic Calculations with Error Handling
Applied **COMPUTE** statements with **ROUNDED** and **ON SIZE ERROR** to safely calculate sales changes and percentages.
 * Pagination and Report Formatting
Controlled page layout using line counters, headings, and spacing to produce a clean, professional report.
 * Modular Program Structure (Paragraphs & PERFORM)
Organized logic into reusable paragraphs, improving readability, maintainability, and program flow.

## Tech Stack
___
* ![COBOL](https://img.shields.io/badge/COBOL-Enterprise-blue)
* ![Visual Studio Code](https://img.shields.io/badge/VS_Code-007ACC.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
* ![GitHub](https://img.shields.io/badge/GitHub-000000.svg?style=for-the-badge&logo=GitHub)

## Installation
___
1. Clone the repository to your local machine. (or just steal my code)
2. Put the code into VS Code in your mainframe of choice

## Running Output
___
![Code Running](assets/RPT5000AgainHolyCow.png)

## Learning Outcomes
___
 * Gained experience with COBOL file handling (sequential file processing)
 * Implemented control break logic for grouped reporting
 * Practiced data formatting and report generation in a legacy language
 * Applied arithmetic operations for business calculations (percent change, totals)
 * Improved understanding of modular programming using structured paragraphs
 * Developed skills in debugging and testing batch-style programs
 * Two-Level Summary Report: Expanded control break logic to handle multiple grouping levels (sales representative within branch), producing nested subtotals and a more detailed hierarchical report structure.
 * Switch Conditional Names (88-Level): Leveraged 88-level condition names as logical switches to improve readability and control program flow (e.g., EOF flags, first-record indicators).
 * EVALUATE Case Structure: Applied the EVALUATE statement as a case structure to streamline multi-branch decision logic, replacing complex nested IF statements.
 * SET TRUE/FALSE Statements: Used SET statements with condition names to explicitly control boolean-like flags, improving clarity and maintainability of program state management.
  
## Help
___
* Make sure compiler is running correctly.
* Potentially re-clone repository
* restart IDE

## Authors
___
**Kirby Dunker**

<img src="https://github.com/KirbyD-YEAH.png" alt="Profile Picture" width="100" />

* **Kirby's GitHub Profile**: [KirbyD-YEAH](https://github.com/KirbyD-YEAH)
* **Kirby's Email**: [brdunk02@wsc.edu](mailto:brdunk@wsc.edu)

**Clay Rasmussen**

<img src="https://github.com/Clay-Rasmussen.png" alt="Profile Picture" width="100" />

* **Clay's GitHub Profile**: [Clay-Rasmussen](https://github.com/Clay-Rasmussen)
* **Clay's Email**: [clrasm02@wsc.edu](mailto:clrasm02@wsc.edu)

[Back to the top](#overview)
