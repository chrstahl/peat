
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

**PDF Entity Annotation Tool (PEAT)**

**Version 1.0**

1. Select the PDF and Schema (tags.json is included in the test folder.)

2. Annotate PDF
    1.	Highlight text you wish to annotate and select *Add Annotation*.
    ![Alt text](user_guide_images/image022.png?raw=true "AddAnnotation")
    2.	Select the annotation type.

    ![Alt text](user_guide_images/image024.png?raw=true "AddAnnotation")
    3. Hit save

    ![Alt text](user_guide_images/image026.png?raw=true "AddAnnotation")

    ![Alt text](user_guide_images/image028.png?raw=true "AddAnnotation")

3. Save Annotations
    1.	Click *File* in the menu bar and select *Save Annotations*.

    ![Alt text](user_guide_images/image030.png?raw=true "AddAnnotation")

    2.	Select a save location on your computer and click *Save Annot File*.

    ![Alt text](user_guide_images/image032.png?raw=true "AddAnnotation")

4. Load Annotations
    1.	Click File in the menu bar and select Load Annotations.

    ![Alt text](user_guide_images/image034.png?raw=true "AddAnnotation")

    2.	Select an annotation file

    ![Alt text](user_guide_images/image036.png?raw=true "AddAnnotation")

    ![Alt text](user_guide_images/image038.png?raw=true "AddAnnotation")

5. Delete Annotations
    1. Select annotation you wish to delete from the table in the side bar.

    ![Alt text](user_guide_images/image040.png?raw=true "AddAnnotation")

    2. Click *Delete selected row* button

    ![Alt text](user_guide_images/image042.png?raw=true "AddAnnotation")