# README.md

## Introduction
This repository introduces the data format specification for passing table data between the backend and frontend. Use this specification to achieve the following goals:

1. **Benefit from efficiency**: Aim for standardization within your team or individually.
2. **Reduce development costs**: Aim for standardization with external teams within the company to lower development costs.
3. **Facilitate talent acquisition**: Aim for standardization between companies to make talent acquisition easier.

## Update Policy for Specifications
1. Update if there are reasonable specifications.
2. If there are similar specifications, either differentiate, adopt, or learn from them.
3. As much as possible, create specifications not only for one function but also for other functions.

## Overview of Data Specifications
As a first step, we have decided on the data specifications for representing tables for both the backend and frontend. This allows for the creation of input screens with minimal adjustments and provides database functions (CRUD functions) similar to those found in cloud services.

While this specification is designed with web systems in mind, it can be applied to other contexts as well. We aim to update it to accommodate non-web systems as much as possible.

Currently, we are developing a sample library with CRUD functions using the Laravel framework based on this specification. We plan to make this sample library publicly available.

## List of Data Specification Properties

## List of Data Specification Properties

| Property Name           | Description                                                          |
|-------------------------|----------------------------------------------------------------------|
| label                   | Display name                                                         |
| width                   | Column width                                                         |
| class                   | Additional CSS class                                                 |
| inputType               | Type of input field                                                  |
| order                   | Order                                                                |
| col                     | Number of columns for 12-grid division                               |
| step                    | Number of decimal places allowed                                     |
| maxLength               | Maximum number of input characters (for input screens)               |
| maxDigits               | Maximum number of input digits (for input screens)                   |
| options                 | Selection list for radio or select                                   |
| optionsTable            |                                                                      |
| optionsColumn           |                                                                      |
| optionsTableRef         |                                                                      |
| defaultValue           | Default value                                                        |
| validate                | Validation rules                                                     |
| referenceForeignKey     |                                                                      |
| referenceField          | Field to record the ID of the referenced record                      |
| referenceLabel          | Display name of the referenced record                                |
| referenceLink           | Link to the referenced record                                        |
| localTableName          |                                                                      |
| joinModel               | Parent model in a master-detail relationship                         |
| parentField             |                                                                      |
| parentLabel             |                                                                      |
| parentLink              |                                                                      |
| omittedTableName        | Omitted table                                                        |
| fileInfo                | Parent property for file upload (see fileInfo section for details)   |
| >fileUploadType         | Upload type (local or bucket)                                        |
| >pathType               | Relative or absolute path                                            |
| >save_folder            | Directory for saving files                                           |
| >save_file_name         | File name for saving                                                 |
| >display_text           | File name for display                                                |
| >icon                   | Icon for display                                                     |
| >remoteBucketName       | Bucket name                                                          |
| createDisplay           | Whether to display on the create/update screen                       |

## Handling Gaps with Requirements
Please follow the specifications as a basic guideline. If the specifications do not meet your requirements, feel free to not use them or add custom properties. We plan to refine the ambiguous points of this specification in the future, but there may be cases where it no longer meets certain requirements. Please indicate the version of the specification you are using and note any deviations from the specification.