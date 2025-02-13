# UFC Fight Statistics Dataset (2016-2024)

## Metadata Overview
This dataset contains fight statistics from UFC events between 2016 and 2024

## Data Source
- **Source:** [Kaggle.com](https://www.kaggle.com/datasets/alexmagnus24/ufc-fight-statistics-july-2016-nov-2024?select=UFC+Fight+Statistics+%28July+2016+-+Nov+2024%29.csv)
- **Collected by:** Alex Magnus
- **Data Format:** `.csv`

## Data Collection and Extraction
- Data was webscraped by the original uploader and made available on Kaggle.
- Downloaded from Kaggle as a `.csv` file.
- No major transformations occurred during extraction.

## Data Cleaning Process
- Data was cleaned using Python (`pandas`).
- NA values only appeared in the referee column, these rows were not excluded.
- The dataset was reduced from 194 columns to 23 by aggregating total strikes landed, total strikes missed, knockdowns, takedowns completed, takedowns missed, submission attempts, and total control time per fight.
- Column names were standardized
- fighter_a, fighter_b, method, fight_time, referee, weight_class, event = `object`
- winner = `int`
- total_strike_landed_a, total_strike_landed_b, total_strike_missed_a, total_strike_missed_b, knockdowns_a, knockdowns_b, td_completed_a, td_completed_b, td_missed_a, td_missed_b, sub_att_a, sub_att_b, ctrl_time_minutes_a, ctrl_time_minutes_b_, rounds = `float`
