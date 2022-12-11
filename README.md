# Name Entity Recognition for Medical Transcripts

Performing NER on MEdical Datasets

## Running the Project

### Creating the Environment

1. Install Pytorch

   Pytorch is a requirement for running some of the libraries. However, pytorch implementation varies according to machine, so it has to be done manually.

   Refer to <https://pytorch.org/get-started/locally/> for installation.

2. Installing requirements

    Requirements can be installed using pipenv dependency manager. Install pipenv using command:

    ```shell
    pip install pipenv
    ```

    Then you can install the requirements using the command:

    ```shell
    pipenv install
    ```

    *Note: The dependencies are a bit large so a stable internet connection and a bit of patience is required*

3. Installing language model

   We need to download a spacy model. We can download it by the command:

   ```shell
   python -m spacy download en_core_web_lg
   ```

### Running the Notebook

1. We need jupyter installed to run the notebook

    ```shell
    pip install jupyter
    ```

2. Launch the notebook interface using command

    ```shell
    jupyter notebook
    ```

3. Navigate to the required notebook to view

### Running From CLI

We can run the NER data extractor from the cli too by using the command from the base dir

```shell
python ner/medical_ner.py <location-to-file>
```

For instance,

```shell
python ner/medical_ner.py assets/txt_reports/report_0.txt
```
