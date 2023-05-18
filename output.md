
 ## DataFrame info befor process :
|    |   index | Name             |   Count | Non-Null   | Dtype   |
|---:|--------:|:-----------------|--------:|:-----------|:--------|
|  0 |       0 | image_name       |   33126 | non-null   | object  |
|  1 |       1 | patient_id       |   33126 | non-null   | object  |
|  2 |       2 | sex              |   33061 | non-null   | object  |
|  3 |       3 | age_approx       |   33058 | non-null   | float64 |
|  4 |       4 | anatomy_sites    |   32599 | non-null   | object  |
|  5 |       5 | diagnosis        |   33126 | non-null   | object  |
|  6 |       6 | benign_malignant |   33126 | non-null   | object  |
|  7 |       7 | target           |   33126 | non-null   | int64   |



 ## Missing values befor & aftre  process :
|                  |   Befor |   After |
|:-----------------|--------:|--------:|
| image_name       |       0 |       0 |
| patient_id       |       0 |       0 |
| sex              |      65 |       0 |
| age_approx       |      68 |       0 |
| anatomy_sites    |     527 |       0 |
| diagnosis        |       0 |       0 |
| benign_malignant |       0 |       0 |
| target           |       0 |       0 |



 ## Unique values befor & aftre  process :
|                  |   Befor |   After |
|:-----------------|--------:|--------:|
| image_name       |   33126 |   33126 |
| patient_id       |    2056 |    2056 |
| sex              |       2 |       2 |
| age_approx       |      18 |      20 |
| anatomy_sites    |       6 |       6 |
| diagnosis        |       9 |       9 |
| benign_malignant |       2 |       2 |
| target           |       2 |       2 |



 ## Value counts befor & aftre  process :
|    | Column           | Value           |   Count Befor |   Count After |
|---:|:-----------------|:----------------|--------------:|--------------:|
|  0 | sex              | male            |         17080 |         17145 |
|  1 | sex              | female          |         15981 |         15981 |
|  2 | anatomy_sites    | torso           |         16845 |         17372 |
|  3 | anatomy_sites    | lower extremity |          8417 |          8417 |
|  4 | anatomy_sites    | upper extremity |          4983 |          4983 |
|  5 | anatomy_sites    | head/neck       |          1855 |          1855 |
|  6 | anatomy_sites    | palms/soles     |           375 |           375 |
|  7 | anatomy_sites    | oral/genital    |           124 |           124 |
|  8 | benign_malignant | benign          |         32542 |         32542 |
|  9 | benign_malignant | malignant       |           584 |           584 |
| 10 | target           | 0               |         32542 |         32542 |
| 11 | target           | 1               |           584 |           584 |



 ## Descriptive statistics befor and after the process:
|       |   age_approx |        target |   age_approx |        target |
|:------|-------------:|--------------:|-------------:|--------------:|
| count |   33058      | 33126         |   33126      | 33126         |
| mean  |      48.87   |     0.0176297 |      48.8691 |     0.0176297 |
| std   |      14.3804 |     0.131603  |      14.3656 |     0.131603  |
| min   |       0      |     0         |       0      |     0         |
| 25%   |      40      |     0         |      40      |     0         |
| 50%   |      50      |     0         |      50      |     0         |
| 75%   |      60      |     0         |      60      |     0         |
| max   |      90      |     1         |      90      |     1         |


