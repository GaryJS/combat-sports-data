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
- fighter_a, fighter_b, method, referee, weight_class, event = `string`
- winner, rounds = `int`
- fight_time = `timedelta`
- total_strike_landed_a, total_strike_landed_b, total_strike_missed_a, total_strike_missed_b, knockdowns_a, knockdowns_b, td_completed_a, td_completed_b, td_missed_a, td_missed_b, sub_att_a, sub_att_b, ctrl_time_minutes_a, ctrl_time_minutes_b_, rounds = `float`

## Data Units and Column Definitions
| Column Name                 | Description                                              | Data Type  |
|-----------------------------|----------------------------------------------------------|------------|
| `fighter_a`                 | Name of Fighter 1                                       | String     |
| `fighter_b`                 | Name of Fighter 2                                       | String     |
| `winner`                    | Winner of the fight (1 = Fighter A, 0 = Fighter B)      | Category   |
| `method`                    | How the fight was won (KO/TKO, Submission, Decision)    | String     |
| `fight_time`                | Total duration of the fight (MM:SS or rounds-based)     | Timedelta  |
| `referee`                   | Name of the referee for the fight                       | String     |
| `weight_class`              | Weight class of the fight (e.g., Lightweight, Heavyweight) | String  |
| `event`                     | Name of the UFC event                                   | String     |
| `total_strike_landed_a`     | Total strikes landed by Fighter A                      | Float      |
| `total_strike_landed_b`     | Total strikes landed by Fighter B                      | Float      |
| `total_strike_missed_a`     | Total strikes missed by Fighter A                      | Float      |
| `total_strike_missed_b`     | Total strikes missed by Fighter B                      | Float      |
| `knockdowns_a`              | Knockdowns scored by Fighter A                         | Float      |
| `knockdowns_b`              | Knockdowns scored by Fighter B                         | Float      |
| `td_completed_a`            | Takedowns successfully completed by Fighter A          | Float      |
| `td_completed_b`            | Takedowns successfully completed by Fighter B          | Float      |
| `td_missed_a`               | Takedown attempts missed by Fighter A                  | Float      |
| `td_missed_b`               | Takedown attempts missed by Fighter B                  | Float      |
| `sub_att_a`                 | Submission attempts by Fighter A                       | Float      |
| `sub_att_b`                 | Submission attempts by Fighter B                       | Float      |
| `ctrl_time_minutes_a`       | Total control time in minutes for Fighter A            | Float      |
| `ctrl_time_minutes_b`       | Total control time in minutes for Fighter B            | Float      |
| `rounds`                    | Total number of rounds in the fight (3 or 5)           | Integer    |

## Data Validation and Regulations
- Data was cross-checked against UFC official results.
- This data set is for **educational purposes only**.
- UFC data usage policies must be followed (if applicable).

## References 
- [Original Dataset on Kaggle](https://www.kaggle.com/datasets/alexmagnus24/ufc-fight-statistics-july-2016-nov-2024)
---
-[UFC official Website](https://www.ufc.com/events)
---
-**Author** Gary San Angelo
-**Date** 02/12/2025
