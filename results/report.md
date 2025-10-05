# Image Matching Report (ORB_BF and SIFT_FLANN)

**Threshold Used**: 20

## ORB_BF Approach

- **Data_Check Accuracy**: 80.00% (16/20)
- **Data_Check Avg Time**: 0.0171s (±0.0324s)

### Confusion Matrix (Data_Check)
![Confusion Matrix ORB_BF](confusion_matrix_orb_bf.png)

### Match Counts Plot (Data_Check)
![Match Counts ORB_BF](match_counts_orb_bf.png)

### Per-Pair Results (Data_Check)
| Folder | Expected | Predicted | Good Matches | Visualization |
|--------|----------|-----------|--------------|---------------|
| different_1 | No Match | No Match | 6 | <img src="different_1_orb_bf_no_match.png" width="200"> |
| different_10 | No Match | No Match | 19 | <img src="different_10_orb_bf_no_match.png" width="200"> |
| different_2 | No Match | No Match | 1 | <img src="different_2_orb_bf_no_match.png" width="200"> |
| different_3 | No Match | No Match | 3 | <img src="different_3_orb_bf_no_match.png" width="200"> |
| different_4 | No Match | No Match | 7 | <img src="different_4_orb_bf_no_match.png" width="200"> |
| different_5 | No Match | No Match | 1 | <img src="different_5_orb_bf_no_match.png" width="200"> |
| different_6 | No Match | No Match | 2 | <img src="different_6_orb_bf_no_match.png" width="200"> |
| different_7 | No Match | No Match | 1 | <img src="different_7_orb_bf_no_match.png" width="200"> |
| different_8 | No Match | No Match | 14 | <img src="different_8_orb_bf_no_match.png" width="200"> |
| different_9 | No Match | No Match | 10 | <img src="different_9_orb_bf_no_match.png" width="200"> |
| same_1 | Match | Match | 43 | <img src="same_1_orb_bf_match.png" width="200"> |
| same_10 | Match | Match | 34 | <img src="same_10_orb_bf_match.png" width="200"> |
| same_2 | Match | No Match | 18 | <img src="same_2_orb_bf_no_match.png" width="200"> |
| same_3 | Match | No Match | 5 | <img src="same_3_orb_bf_no_match.png" width="200"> |
| same_4 | Match | No Match | 9 | <img src="same_4_orb_bf_no_match.png" width="200"> |
| same_5 | Match | Match | 47 | <img src="same_5_orb_bf_match.png" width="200"> |
| same_6 | Match | Match | 23 | <img src="same_6_orb_bf_match.png" width="200"> |
| same_7 | Match | Match | 29 | <img src="same_7_orb_bf_match.png" width="200"> |
| same_8 | Match | Match | 53 | <img src="same_8_orb_bf_match.png" width="200"> |
| same_9 | Match | No Match | 16 | <img src="same_9_orb_bf_no_match.png" width="200"> |

### UiA Images Results
- **Predicted**: No Match
- **Good Matches**: 1
- **Time**: 0.0239s
![UiA Match](UIA_orb_bf_no_match.png)

## SIFT_FLANN Approach

- **Data_Check Accuracy**: 85.00% (17/20)
- **Data_Check Avg Time**: 0.0621s (±0.0034s)

### Confusion Matrix (Data_Check)
![Confusion Matrix SIFT_FLANN](confusion_matrix_sift_flann.png)

### Match Counts Plot (Data_Check)
![Match Counts SIFT_FLANN](match_counts_sift_flann.png)

### Per-Pair Results (Data_Check)
| Folder | Expected | Predicted | Good Matches | Visualization |
|--------|----------|-----------|--------------|---------------|
| different_1 | No Match | No Match | 9 | <img src="different_1_sift_flann_no_match.png" width="200"> |
| different_10 | No Match | No Match | 6 | <img src="different_10_sift_flann_no_match.png" width="200"> |
| different_2 | No Match | No Match | 5 | <img src="different_2_sift_flann_no_match.png" width="200"> |
| different_3 | No Match | No Match | 7 | <img src="different_3_sift_flann_no_match.png" width="200"> |
| different_4 | No Match | No Match | 12 | <img src="different_4_sift_flann_no_match.png" width="200"> |
| different_5 | No Match | No Match | 5 | <img src="different_5_sift_flann_no_match.png" width="200"> |
| different_6 | No Match | No Match | 11 | <img src="different_6_sift_flann_no_match.png" width="200"> |
| different_7 | No Match | No Match | 11 | <img src="different_7_sift_flann_no_match.png" width="200"> |
| different_8 | No Match | No Match | 6 | <img src="different_8_sift_flann_no_match.png" width="200"> |
| different_9 | No Match | No Match | 18 | <img src="different_9_sift_flann_no_match.png" width="200"> |
| same_1 | Match | Match | 57 | <img src="same_1_sift_flann_match.png" width="200"> |
| same_10 | Match | Match | 50 | <img src="same_10_sift_flann_match.png" width="200"> |
| same_2 | Match | Match | 41 | <img src="same_2_sift_flann_match.png" width="200"> |
| same_3 | Match | No Match | 12 | <img src="same_3_sift_flann_no_match.png" width="200"> |
| same_4 | Match | Match | 21 | <img src="same_4_sift_flann_match.png" width="200"> |
| same_5 | Match | Match | 36 | <img src="same_5_sift_flann_match.png" width="200"> |
| same_6 | Match | No Match | 8 | <img src="same_6_sift_flann_no_match.png" width="200"> |
| same_7 | Match | Match | 30 | <img src="same_7_sift_flann_match.png" width="200"> |
| same_8 | Match | Match | 82 | <img src="same_8_sift_flann_match.png" width="200"> |
| same_9 | Match | No Match | 19 | <img src="same_9_sift_flann_no_match.png" width="200"> |

### UiA Images Results
- **Predicted**: No Match
- **Good Matches**: 13
- **Time**: 0.2536s
![UiA Match](UIA_sift_flann_no_match.png)

