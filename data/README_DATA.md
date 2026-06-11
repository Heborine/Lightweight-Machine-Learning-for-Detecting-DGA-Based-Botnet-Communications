The notebooks download data with Kaggle Hub. Backup copies are included in `data/backup_csvs/`.

| File | Kaggle source | Rows |
|------|------|------:|
| `data/backup_csvs/top-1m.csv` | `adebayo/cisco-umbrella-list` | 1,000,000 |
| `data/backup_csvs/dga_data.csv` | `gtkcyber/dga-dataset` | 160,003 |

To refresh the data:

```python
import kagglehub

print(kagglehub.dataset_download("adebayo/cisco-umbrella-list"))
print(kagglehub.dataset_download("gtkcyber/dga-dataset"))
```
