
# SavannahML: Wildlife Image Analysis with Microsoft Fabric

An end-to-end data engineering and machine learning pipeline for analyzing large-scale wildlife image metadata from camera traps in the African Savannah, built on Microsoft Fabric.

##  Project Goals

- Ingest and organize JSON metadata into a Fabric Lakehouse
- Process and analyze data using Apache Spark
- Prepare datasets for machine learning
- Train and evaluate classification models to identify wildlife patterns

##  Technologies Used

- Microsoft Fabric (Lakehouse, Data Factory, Spark, ML)
- Apache Spark (PySpark)
- Python (Pandas, Scikit-learn)
- JSON, Parquet

#  Project Walkthrough: SavannahML with Microsoft Fabric

This walkthrough documents each stage of the project, including screenshots and brief descriptions.

---

## 1. Loading Data into the Lakehouse

###  Configure a Data Factory Pipeline to Copy Data

Use Data Factory to set up a pipeline that ingests the raw JSON metadata.

📸 **Screenshot:**
![Data Factory Pipeline]
![89c95f53-701e-471b-aca9-e481df3a99c2](https://github.com/user-attachments/assets/f23ba8b0-945a-41bf-b575-d230e830bf6f)

---

###  Explore the Data in the Lakehouse

After loading, verify and preview the data within the Lakehouse Files section.

📸 **Screenshot:**
![Lakehouse View]

---
![6424c31d-2564-4ae7-bd22-e0d2d7ccbc05](https://github.com/user-attachments/assets/d4d65f78-c2d1-4f24-8ff1-e659e0c1831c)

###  Convert the JSON Files into Parquet Files

Use a Spark notebook to read the JSON and convert to Parquet for efficient querying.

📸 **Screenshot:**


---
![54743cb2-af6b-4d09-a8e1-8bc1025870bf](https://github.com/user-attachments/assets/81f8b1e3-08cd-48d9-a067-8ffef15d1bd4)

### 🗃 Load the Parquet Files into Delta Tables

Register the Parquet files as Delta tables to enable SQL exploration.

📸 **Screenshot:**
![87ac38fb-65cb-40a0-879e-23a172cbeb45](https://github.com/user-attachments/assets/d9e7f357-4a3f-4707-9182-df8dd9dcb843)


---



---

## 3. Semantic Model

(Optional) Build a semantic layer if needed for downstream data consumption or ML feature clarity.

![2486d040-633a-4d90-b253-1b16708efca5](https://github.com/user-attachments/assets/45b04493-962a-40d5-b675-aed38faa60e0)


---

## 6. Data Analysis & Transformation with Apache Spark in Fabric

Perform transformations such as flattening, feature extraction, and filtering.

These steps are documented in the following notebook:

https://github.com/GadAugust/FabricWild-From-Camera-Traps-to-ML-Models/blob/main/analyze-and-transform-data.ipynb

Data Analysis & Transformation with Apache Spark in Fabric

Download the image files into the Lakehouse

Preparing your data for Training

Training and Evaluating the Machine Learning model

All of these steps are documented in the notebook linked above.


This walkthrough demonstrates how to build a scalable wildlife analytics pipeline using Microsoft Fabric’s integrated data and ML tools.





