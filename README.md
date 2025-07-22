# PIFSC Data Archiving Guide 101

## Table of Contents

1.  **[The Basics: Key Terms and Systems](#the-basics:-key-terms-and-systems)**
2.  **The Archive Workflow: Step-by-Step**
      * [Step 1: Planning](#step-1:-Planning)
      * [Step 2: Prep and QC Your Data](#step-2:-prep-and-qc-your-data)
      * [Step 3: Document Your Data in InPort](#step-3:-document-your-data-in-inport)
      * [Step 4: Build the S2N Submission Package](#step-4:-build-the-s2n-submission-package)
      * [Step 5: Handle Special Cases like Imagery and Code](#step-5:-handle-special-cases-like-imagery-and-code)
      * [Step 6: Submit and Make Updates Later](#step-6:-submit-and-make-updates-later)

-----

## The Basics: Key Terms and Systems


  - **[PARR](https://www.ngdc.noaa.gov/parr.html)**: This stands for **Public Access to Research Results**. It’s the federal mandate that says we have to make our research data available to the public.
  - **[NCEI](https://www.ncei.noaa.gov/)**: The **National Centers for Environmental Information**. Serves as the designated archive for NOAA's environmental data, responsible for its long-term preservation and accessibility.
  - **[InPort](https://www.fisheries.noaa.gov/inport/)**: This is our metadata catalog. Every dataset needs an InPort record so people can find it and understand it. It’s the who, what, where, when, and how for your data.
  - **[S2N](https://www.ncei.noaa.gov/archive/send2ncei/)**: This means **Send2NCEI**. It's the website you'll use to bundle up your data, metadata, and other documents into a package to officially send to the NCEI archive.
  - **[NODD](https://www.noaa.gov/information-technology/open-data-dissemination)**: The **NOAA Open Data Dissemination** program. This is our go-to for putting large datasets (like raw imagery) on  Google Cloud so people can access them.

-----

## The Archive Workflow: 


### Step 1: Planning

Good archiving starts with a good plan for data collection and organizing! Before you begin a project its best to meet with someone from the DST to map out the project's data collection, timeline, and what's needed for archiving. Getting this done before data collection makes archiving much easier down the road😊

**Related Guides:**

  * "PARR Guidance for Datasets and Publications"
  * "Archive Process Checklist"

### Step 2: Prep and QC Your Data

Your data needs to be clean, correctly formatted, reliable, and accurate. This step is all about getting your data files ready and running them through **Quality Control (QC)** process. 

**Helpful Tools:**
  * folderstats
  * optical val

**Related Guides:**

  * "How to: QC your data"
  * "How to: Prepare Data Files IN database via SQL Developer"
  * "How to: Prepare Data Files NOT in Database"

### Step 3: Document Your Data in InPort

In order to make data accessible and digestible  you have to describe it well. This is done by creating a metadata record in **InPort**. 

**Related Guides:**

  * "How to: InPort (document your data)"
  * "Collaborative InPort Template"
  * "How to: Data Citations"

### Step 4: Build the S2N Submission Package

With your data prepped and your InPort record done, it's time to build the package you'll send to NCEI. You'll use the **S2N** website to create a "stub" that links your data, your data dictionary, and the key metadata together for submission.

**Related Guides:**

  * "How to: S2N (submit your data to NOAA archive)"
  * "SOP: How to: Archive Package Review 2023"

### Step 5: Handle Special Cases like Imagery and Code

Not all data is a simple spreadsheet. We have specific ways to handle things like imagery and the R scripts. Big files often go to Google cloud via **NODD**, and code belongs in GitHub.

**Related Guides:**

  * "SOP: Imagery Archive Prep 2023"
  * "SOP: How to get set up for NODD 2023"
  * "WorkingDoc: SOP Archiving R scripts on GitHub"
  * "Guidance on archiving video 2024"

### Step 6: Submit and Make Updates Later

....

**Related Guides:**

  * "How to: Update Archived Data or Metadata 2023"
  * "SOP: Request a Reserve DOI"
