## Dataset
**Bluebook for Bulldozers** — [Kaggle Competition Page](https://www.kaggle.com/competitions/bluebook-for-bulldozers/overview)

## Option 1: Manual Download
1. Go to the [competition data page](https://www.kaggle.com/competitions/bluebook-for-bulldozers/data).
2. Sign in to Kaggle (free account) and accept the competition rules.
3. Click **Download All** to get the dataset ZIP file.
4. Extract the contents into this `data/` folder. You should end up with files like:
   ```
   data/
   ├── Train.csv
   ├── Valid.csv
   ├── Test.csv
   └── Data Dictionary.xlsx
   ```

## Option 2: Kaggle API (faster, scriptable)
1. Install the Kaggle CLI:
   ```bash
   pip install kaggle
   ```
2. Get your API token from your [Kaggle account settings](https://www.kaggle.com/settings) → **Create New API Token**. This downloads a `kaggle.json` file.
3. Place `kaggle.json` in `~/.kaggle/` (Linux/Mac) or `C:\Users\<username>\.kaggle\` (Windows).
4. Run:
   ```bash
   kaggle competitions download -c bluebook-for-bulldozers -p data/
   unzip data/bluebook-for-bulldozers.zip -d data/
   ```

## After Downloading
Once the files are in place, update the file paths in the notebook if they don't already point to `data/Train.csv`, etc., then run the notebook as described in the main [README](../README.md).
