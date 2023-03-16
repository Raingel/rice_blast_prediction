# Prediction Results of BlastDT, BLASTAM, BlastTF, and BlastGRU-TW Models

This repository contains the daily prediction results generated by four models, namely BlastDT, BLASTAM, BlastTF, and BlastGRU-TW, on the server in NCHU. 
Each model generates a daily prediction result that is saved as a CSV file. 
The naming convention of the CSV file is as follows: "YYYYMMDD_MODEL.csv" where "YYYYMMDD" represents the date and "MODEL" represents the name of the model.

## Models
The following are brief descriptions of each model:

- **BlastDT**: A decision tree model developed by Yi-Nian Chen from the Taiwan Agricultural Research Institute.
- **BLASTAM**: A model developed by Mr. Koshimizu from Japan. 
    >   越水幸男. 1988. 「アメダス資料による葉いもち発生予察法」. https://agriknowledge.affrc.go.jp/RN/2030411788
- **BlastTF**: A deep learning model developed by the Fungal Biology Laboratory at National Chung Hsing University. The neural network architecture uses the Transformer model.
- **BlastGRU-TW**: A deep learning model developed by the Fungal Biology Laboratory at National Chung Hsing University. The neural network architecture uses the gated recurrent unit (GRU) model and is trained on the Taiwan dataset.
    > Ou, J. H., Kuo, C. H., Wu, Y. F., Lin, G. C., Lee, M. H., Chen, R. K., ... & Chen, C. Y. (2023). Application-oriented deep learning model for early warning of rice blast in Taiwan. Ecological Informatics, 73, 101950. https://doi.org/10.1016/j.ecoinf.2022.101950
## File Structure
The repository is structured as follows:


```
├── data
│   ├── 20190218_BLASTDT.csv
│   ├── 20190219_BLASTDT.csv
│   ├── ...
│   ├── 20190218_BLASTAM.csv
│   ├── 20190219_BLASTAM.csv
│   ├── ...
│   ├── 20190218_BlastTF.csv
│   ├── 20190219_BlastTF.csv
│   ├── ...
│   ├── 20190218_BlastGRU-TW.csv
│   ├── 20190219_BlastGRU-TW.csv
│   ├── ...
```

The top-level directory contains four subdirectories, one for each model. Within each subdirectory are the CSV files containing the prediction results for each day.

## Usage
To use the prediction results, simply download the CSV file for the desired day and model. Each CSV file contains the predicted outcomes for a specific day.

## Acknowledgments
- Thanks to the developers of BlastDT, BLASTAM, BlastTF, and BlastGRU-TW for providing their models.
- Thanks to the developers of the data processing pipeline for generating the daily prediction results. Especially [Open-meteo](https://github.com/open-meteo/open-meteo) and [NCDR](https://watch.ncdr.nat.gov.tw/watch_user) 
