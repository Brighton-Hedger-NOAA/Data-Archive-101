# PIFSC Data Archiving Guide 101

## Table of Contents

1.  **[The Basics: Key Terms and Systems](#the-basics-key-terms-and-systems)**
2.  **The Archive Workflow: Step-by-Step**
      * [Step 1: Planning](#step-1-Planning)
      * [Step 2: Prep and QC Your Data](#step-2-prep-and-qc-your-data)
      * [Step 3: Document Your Data in InPort](#step-3-document-your-data-in-inport)
      * [Step 4: Build the S2N Submission Package](#step-4-build-the-s2n-submission-package)
3.  **[Special Cases like Imagery and Code](#special-cases-like-imagery-and-code)**
4.  **[Misc Archive Info](#misc-archive-info)**
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

**A Deeper Guide:**
 * link parr github page

**Related Documents:**

  * [PIFSC Publication Guidance](https://docs.google.com/document/d/1Fk5DPcdzFjuga-nuU943HOboVh35EvijLpKoGaaQkvk/edit?usp=sharing)

### Step 2: Prep and QC Your Data

Your data needs to be clean, correctly formatted, reliable, and accurate. This step is all about getting your data files ready and running them through **Quality Control (QC)** process. 

**Helpful Tools:**
  * [Folder Stats Tool](https://github.com/MichaelAkridge-NOAA/archive-toolbox/blob/main/toolbox/desktop/folder-stats-tool/folderstats.exe)
  * [Archive Manifest File Tool](https://github.com/MichaelAkridge-NOAA/archive-toolbox/blob/main/toolbox/desktop/archive-manifest-file-tool/mnftool_gui.exe)
  * [Clear Thumbs Database Tool](https://github.com/MichaelAkridge-NOAA/archive-toolbox/tree/main/toolbox/desktop/clear-thumbs-db-files)
  * [File Copy Tool](https://github.com/MichaelAkridge-NOAA/archive-toolbox/blob/main/toolbox/desktop/file-copy-tool/filecopy_tool.exe)
  * [Garmin GPS File Converter Tool](https://github.com/MichaelAkridge-NOAA/archive-toolbox/blob/main/toolbox/desktop/garmin-gps-file-converter/gpxconverter_windows_standalone.exe)
  * [Heic Heif Converter Tool](https://github.com/MichaelAkridge-NOAA/archive-toolbox/blob/main/toolbox/desktop/heic-heif-converter/heic_converter.exe)
  * [Deeper Explanation of Toos and Uses](https://github.com/MichaelAkridge-NOAA/archive-toolbox/blob/main/README.md)

**A Deeper Guide:**
 * link prep and qc github page

**Related Documents:**

  * [How to: QC Your Data](https://docs.google.com/document/d/1Hv-QvBC5bwBvdr4iYivEWfJET7MEna7L9RqkOwSSXtE/edit?usp=sharing)
  * [How to: Prepare Data Files IN Database via SQL Developer](https://docs.google.com/document/d/1GFxLZqB6qMCJiyBWRE9S1hYJgz41ZH_mUAJDX63Ojjw/edit?usp=sharing) 
  * [How to: Prepare Data Files NOT IN Database](https://docs.google.com/document/d/1AybZiH03DRiLy4f5zelP8-VW6z2sEgzRJBQi8iK517M/edit?usp=sharing) 

### Step 3: Document Your Data in InPort

In order to make data accessible and digestible  you have to describe it well. This is done by creating a metadata record in **InPort**. 

**A Deeper Guide:**
 * link inport github page

**Related Documents:**

  * [How to: InPort (document your data)](https://docs.google.com/document/d/1kijqSQbISTcOO9JQ_5_AtAZuVvLc-y0y0v-KlKeO1sY/edit?usp=sharing)
  * [Collaborative InPort Template](https://docs.google.com/document/d/1MGWM3o3VRjl-HQhLoPOmRZxR0w_Qvex06gVzGvH4YEo/edit?usp=sharing)

### Step 4: Build the S2N Submission Package

With your data prepped and your InPort record done, it's time to build the package you'll send to NCEI. You'll use the **S2N** website to create a "stub" that links your data, your data dictionary, and the key metadata together for submission.

**Helpful Tools:**
* [Send2NCEI Tool](https://www.ncei.noaa.gov/archive/send2ncei/)
  
**A Deeper Guide:**
 * link s2n github page

**Related Documents:**

  * [How to: S2N (submit your data to NOAA archive)](https://docs.google.com/document/d/18nofaF7c5Bc7OIUO3kUCzYo8FFspH6um3y_xpeBtaJo/edit?usp=sharing)

### Special Cases like Imagery and Code

Not all data is a simple spreadsheet. We have specific ways to handle things like imagery and the R scripts. Big files often go to Google cloud via **NODD**, and code belongs in GitHub.

**A Deeper Guide:**
 * link special cases github page

**Helpful Tools:**
* [NODD Upload Tool and Script](https://picgitlab.nmfs.local/esd/arp/data-services/esd-archive-toolbox/-/tree/main#python-example)

**Related Documents:**

  * [How to: Get Set Up for NODD](https://docs.google.com/document/d/1Y5BXsy9-qxT5QCBOdbHN0fyZgvkAqHjR6VSl8c--zWs/edit?usp=sharing)
  * [SOP: Archiving R scripts on GitHub](https://docs.google.com/document/d/1DTgOJf6CPXxclpuO-A3KN8devmyLbtHPMu_4O27z5_k/edit?usp=sharing)

### Misc Archive Info

**Related Documents:**

  * [How to: Update Archived Data or Metadata](https://docs.google.com/document/d/10fcrn4cuUv7YmncuzOuI2JtlK8B75p40CxcLOxAhvzE/edit?usp=sharing)
  * [SOP: Request a Reserve DOI](https://docs.google.com/document/d/1rvjfUAspNcpUEH2NOgR485FJYKCkAxlIy7g7z99GyR4/edit?usp=sharing)
