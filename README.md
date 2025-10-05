# Image Matching Report (ORB_BF and SIFT_FLANN)

**Threshold Used**: 20

## ORB_BF Approach

- **Data_Check Accuracy**: 80.00% (16/20)

### Confusion Matrix (Data_Check)
![Confusion Matrix ORB_BF](results/confusion_matrix_orb_bf.png)

### Match Counts Plot (Data_Check)
![Match Counts ORB_BF](results/match_counts_orb_bf.png)

ORB_BF often has quite few good matches on most different fingerprints, and a lot on most of the same fingerprints. But there there are a few in each category where it is much less sure.

### Per-Pair Results (Data_Check)
| Folder | Expected | Predicted | Good Matches | Visualization |
|--------|----------|-----------|--------------|---------------|
| different_1 | No Match | No Match | 6 | ![Match](results/different_1_orb_bf_no_match.png) |
| different_10 | No Match | No Match | 19 | ![Match](results/different_10_orb_bf_no_match.png) |
| different_2 | No Match | No Match | 1 | ![Match](results/different_2_orb_bf_no_match.png) |
| different_3 | No Match | No Match | 3 | ![Match](results/different_3_orb_bf_no_match.png) |
| different_4 | No Match | No Match | 7 | ![Match](results/different_4_orb_bf_no_match.png) |
| different_5 | No Match | No Match | 1 | ![Match](results/different_5_orb_bf_no_match.png) |
| different_6 | No Match | No Match | 2 | ![Match](results/different_6_orb_bf_no_match.png) |
| different_7 | No Match | No Match | 1 | ![Match](results/different_7_orb_bf_no_match.png) |
| different_8 | No Match | No Match | 14 | ![Match](results/different_8_orb_bf_no_match.png) |
| different_9 | No Match | No Match | 10 | ![Match](results/different_9_orb_bf_no_match.png) |
| same_1 | Match | Match | 43 | ![Match](results/same_1_orb_bf_match.png) |
| same_10 | Match | Match | 34 | ![Match](results/same_10_orb_bf_match.png) |
| same_2 | Match | No Match | 18 | ![Match](results/same_2_orb_bf_no_match.png) |
| same_3 | Match | No Match | 5 | ![Match](results/same_3_orb_bf_no_match.png) |
| same_4 | Match | No Match | 9 | ![Match](results/same_4_orb_bf_no_match.png) |
| same_5 | Match | Match | 47 | ![Match](results/same_5_orb_bf_match.png) |
| same_6 | Match | Match | 23 | ![Match](results/same_6_orb_bf_match.png) |
| same_7 | Match | Match | 29 | ![Match](results/same_7_orb_bf_match.png) |
| same_8 | Match | Match | 53 | ![Match](results/same_8_orb_bf_match.png) |
| same_9 | Match | No Match | 16 | ![Match](results/same_9_orb_bf_no_match.png) |

Looking at the results per match, we see that the fingerprints that are clearly different or clearly the same, have this reflected in good matches, but the more difficult to compare images are unsure, this makes sense. Changing the threshold either way would create more false positives or false negatives.

## SIFT_FLANN Approach

- **Data_Check Accuracy**: 85.00% (17/20)

### Confusion Matrix (Data_Check)
![Confusion Matrix SIFT_FLANN](results/confusion_matrix_sift_flann.png)

### Match Counts Plot (Data_Check)
![Match Counts SIFT_FLANN](results/match_counts_sift_flann.png)

SIFT_FLANN seems to generally find more matches. But not as many more on same matches as on different matches.

### Per-Pair Results (Data_Check)
| Folder | Expected | Predicted | Good Matches | Visualization |
|--------|----------|-----------|--------------|---------------|
| different_1 | No Match | No Match | 9 | ![Match](results/different_1_sift_flann_no_match.png) |
| different_10 | No Match | No Match | 6 | ![Match](results/different_10_sift_flann_no_match.png) |
| different_2 | No Match | No Match | 5 | ![Match](results/different_2_sift_flann_no_match.png) |
| different_3 | No Match | No Match | 7 | ![Match](results/different_3_sift_flann_no_match.png) |
| different_4 | No Match | No Match | 12 | ![Match](results/different_4_sift_flann_no_match.png) |
| different_5 | No Match | No Match | 5 | ![Match](results/different_5_sift_flann_no_match.png) |
| different_6 | No Match | No Match | 11 | ![Match](results/different_6_sift_flann_no_match.png) |
| different_7 | No Match | No Match | 11 | ![Match](results/different_7_sift_flann_no_match.png) |
| different_8 | No Match | No Match | 6 | ![Match](results/different_8_sift_flann_no_match.png) |
| different_9 | No Match | No Match | 18 | ![Match](results/different_9_sift_flann_no_match.png) |
| same_1 | Match | Match | 57 | ![Match](results/same_1_sift_flann_match.png) |
| same_10 | Match | Match | 50 | ![Match](results/same_10_sift_flann_match.png) |
| same_2 | Match | Match | 41 | ![Match](results/same_2_sift_flann_match.png) |
| same_3 | Match | No Match | 12 | ![Match](results/same_3_sift_flann_no_match.png) |
| same_4 | Match | Match | 21 | ![Match](results/same_4_sift_flann_match.png) |
| same_5 | Match | Match | 36 | ![Match](results/same_5_sift_flann_match.png) |
| same_6 | Match | No Match | 8 | ![Match](results/same_6_sift_flann_no_match.png) |
| same_7 | Match | Match | 30 | ![Match](results/same_7_sift_flann_match.png) |
| same_8 | Match | Match | 82 | ![Match](results/same_8_sift_flann_match.png) |
| same_9 | Match | No Match | 19 | ![Match](results/same_9_sift_flann_no_match.png) |

Looking at the results per match, we see that it finds more incorrect good matches.

## UIA Matching

### ORB_BF Approach

- **Good Matches**: 1/20

![UIA Match](results/UIA_orb_bf_no_match.png)

ORB_BF finds next to no matches, and the found match is incorrect. This makes sense seeing as the images are so different, in perspective, location, brightness, season etc.

## SIFT_FLANN Approach

- **Good Matches**: 13/20

![UIA Match](results/UIA_sift_flann_no_match.png)

SIFT_FLANN finds more good matches, but none of them are correct still. This fits the previous trend of false positives with SIFT_FLANN.

