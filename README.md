
# NodeJS and Yarn Requirement
NodeJS: https://nodejs.org/
Yarn: https://yarnpkg.com/

# Download devDependencies
`yarn`

# Run
`yarn start`

# Package
`yarn package`


# Statement of Need

PEAT is a portable, standalone application built off the Electron software framework and can be used on all major operating systems (Windows, Linux, and Macintosh) and provides an interface for users to annotate PDFs.  

PEAT was designed to take advantage of the latest advancements in PDF text extraction methods while also allowing the user to annotate and label the data directly in PDF format. This approach allows a user to work in a document structure they are familiar with, improving the user experience and facilitating the creation of labeled data for machine consumption and training of future machine learning models.

The application allows users to load PDFs directly from their file system along with data annotation forms with standard or customizable annotation types, labels, entities, and other features such as custom color highlighting. The application also includes features for users to edit and import/export data extraction schemas, export annotations of X and Y PDF coordinal structure (based on the image layer of the PDF), search and manipulate annotations, and save/load progress. Once a user has completed document annotation, the labeled data, full text, and all associated metadata is exportable in JSON format that can be processed by a variety of NLP model building applications such as Spacy or PyTorch.

# User Guide

January 2023

Version 1.0

![colorful abstract painting](./media/image1.jpg){width="6.5in"
height="3.6555555555555554in"}

# Table of Contents

[Table of Contents [2](#table-of-contents)](#table-of-contents)

[Document Revision [3](#document-revision)](#document-revision)

[1 Installation [3](#installation)](#installation)

[1.1 Scope and Purpose [4](#scope-and-purpose)](#scope-and-purpose)

[1.2 Source Code Access [4](#source-code-access)](#source-code-access)

[1.2 Installation MacOSX \* need to work out zip issue
[4](#installation-mac-osx)](#installation-mac-osx)

[1.3 Installation Windows
[4](#installation-windows)](#installation-windows)

[2 Application [7](#application)](#application)

[2.0 Load PDF [7](#load-pdf)](#load-pdf)

[2.1 Annotate PDF [9](#annotate-pdf)](#annotate-pdf)

[2.4 Save Annotations [11](#save-annotations)](#save-annotations)

[2.5 Load Annotations [12](#load-annotations)](#load-annotations)

[2.6 Delete Annotations [13](#delete-annotations)](#delete-annotations)

[2.6 Edit Schema [15](#edit-schema)](#edit-schema)

[2.7 Auto Annotation [16](#auto-annotation)](#auto-annotation)

# Document Revision

  ----------------------- ----------------------- -----------------------
  Date                    Version Number          Document Changes

  01/05/2021              0.1.0                   Initial draft

  07/20/2021              0.1.1                   Updated to beta PEAT
                                                  0.1.1

  09/29/2021              0.1.2                   Update to beta PEAT
                                                  0.1.2

  05/10/2022              0.1.3                   Update to beta PEAT
                                                  0.1.3

  01/24/2023              1.0.1                   Updated to release PEAT
                                                  1.0.1
  ----------------------- ----------------------- -----------------------

# 1 Installation

## 1.1 Scope and Purpose

The purpose of this project is to further the research and development
of tools that NCEA can use in their creation of machine-readable
datasets and machine learning research. This effort consists of the
following objectives:

-   Research and develop software for NCEA that provides the ability to
    annotate scientific publications for use in machine learning
    algorithms. This software should be able to accept a list of tags
    provided by NCEA, allow the user to apply these tags to PDF
    documents in a web interface, and then extract out the information
    needed in machine-readable formats that can be used for machine
    learning.

## 1.2 Source Code Access

This describes the process of accessing the source code.

1\. <https://github.com/USEPA/peat>

## 1.2 Installation Mac OSX

1\. Download latest version from

2\. Double click 'mac.zip' to unzip the file.

  -----------------------------------------------------------------------
  ![](./media/image2.png){width="6.361110017497813in"
  height="0.41944444444444445in"}

  -----------------------------------------------------------------------

3\. Double click 'ElectronReact' to launch the application.

  -----------------------------------------------------------------------
  ![Graphical user interface, application Description automatically
  generated](./media/image3.png){width="4.027777777777778in"
  height="0.5118055555555555in"}

  -----------------------------------------------------------------------

## 1.3 Installation Windows

1\. Download latest version from (PEAT_1.1.0)

[https://usepa.sharepoint.com/sites/DOEORNLCPAD/Shared%20Documents/General/Release%20Candidate/PANDHA_1.1.0.zip](https://usepa.sharepoint.com/sites/DOEORNLCPAD/Shared%20Documents/General/Release%20Candidate/PANDHA_RC1.zip)

2\. Right click PANDHA_1.0.0.zip' and select 'Extract All'

  -----------------------------------------------------------------------
  ![](./media/image4.png){width="3.1458333333333335in"
  height="3.7708333333333335in"}

  -----------------------------------------------------------------------

3\. Select location and hit *Extract*

  -----------------------------------------------------------------------
  ![](./media/image5.png){width="5.0in" height="3.75in"}

  -----------------------------------------------------------------------

4\. From the extracted location double click the *PANDHA_1.1.0*Folder

  -----------------------------------------------------------------------
  ![](./media/image6.png){width="5.0in" height="3.75in"}

  -----------------------------------------------------------------------

5\. Double click *PEAT.exe* to start the application

  -----------------------------------------------------------------------
  ![](./media/image7.png){width="5.0in" height="3.7604166666666665in"}

  -----------------------------------------------------------------------

7\. Select the PDF and Schema (tags.json is including in the PEAT/test
folder) and click *Load*

  -----------------------------------------------------------------------
  ![](./media/image8.png){width="6.35in" height="4.7659722222222225in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

# 2 Application

## 2.0 Load PDF

1.  Click *File* in the menu bar and select *Load PDF*.

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application, Word Description
  automatically
  generated](./media/image9.png){width="6.361111111111111in"
  height="4.050694444444445in"}

  -----------------------------------------------------------------------

2.  Select the PDF file from your computer and click *Open*.

  -----------------------------------------------------------------------
  ![Graphical user interface, application Description automatically
  generated](./media/image10.png){width="6.361111111111111in"
  height="4.018055555555556in"}

  -----------------------------------------------------------------------

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application, Word Description
  automatically generated](./media/image11.png){width="6.35in"
  height="4.013194444444444in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

## 2.1 Annotate PDF

1.  Highlight text you wish to annotate and select *Add Annotation*.

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application Description automatically
  generated](./media/image12.png){width="6.35in"
  height="4.004166666666666in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

2.  Select the annotation type.

  -----------------------------------------------------------------------
  ![](./media/image13.png){width="6.35in" height="4.008333333333334in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

3.  Hit save

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application Description automatically
  generated](./media/image14.png){width="6.35in"
  height="4.039583333333334in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

  -----------------------------------------------------------------------
  ![](./media/image15.png){width="6.35in" height="4.007638888888889in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

## 2.4 Save Annotations

1.  Click *File* in the menu bar and select *Save Annotations*.

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application Description automatically
  generated](./media/image16.png){width="6.35in"
  height="4.0055555555555555in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

2.  Select a save location on your computer and click *Save Annot File*.

  -----------------------------------------------------------------------
  ![Graphical user interface, application Description automatically
  generated](./media/image17.png){width="6.35in"
  height="3.997916666666667in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

## 2.5 Load Annotations

1.  Click *File* in the menu bar and select *Load Annotations*.

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application, Word Description
  automatically generated](./media/image18.png){width="6.35in"
  height="4.013888888888889in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

2.  Select an annotation file and click *Open*

  -----------------------------------------------------------------------
  ![Graphical user interface, text Description automatically
  generated](./media/image19.png){width="6.35in"
  height="3.984722222222222in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application Description automatically
  generated](./media/image20.png){width="6.35in"
  height="4.007638888888889in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

## 2.6 Delete Annotations

1\. Select annotation you wish to delete from the table in the side bar.

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application, Word Description
  automatically generated](./media/image21.png){width="6.35in"
  height="4.013888888888889in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

2\. Click *Delete selected row* button.

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application, Word Description
  automatically generated](./media/image22.png){width="6.35in"
  height="4.010416666666667in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

## 2.6 Edit Schema

1\. Click *Edit Schema* hyper-link

  -----------------------------------------------------------------------
  ![Graphical user interface Description automatically
  generated](./media/image23.png){width="6.35in"
  height="3.9895833333333335in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

-   Change existing entity

    -   Click the text of any entity to edit that entities type.

    -   Click the color selector to change the annotation color.

    -   Click the trash can icon to delete that entity.

-   Add new entity type

    -   Click Add Entity Type to add a new entity.

-   Save changes

    -   Click the Save button.

## 2.7 Auto Annotation

1\. Type word or phrase to be searched for in *Find in document* search
bar

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application Description automatically
  generated](./media/image24.png){width="6.35in"
  height="4.004166666666666in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

2\. Using the arrows (Up or Down) a yellow highlight will cycle through
matches found in the document.

3\. Select entity type from the dropdown box.

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application, Word Description
  automatically generated](./media/image25.png){width="6.35in"
  height="4.002777777777778in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------

4\. Click Annotate to add an annotation for the current selection.

  -----------------------------------------------------------------------
  ![Graphical user interface, text, application Description automatically
  generated](./media/image26.png){width="6.35in"
  height="4.009027777777778in"}
  -----------------------------------------------------------------------

  -----------------------------------------------------------------------
