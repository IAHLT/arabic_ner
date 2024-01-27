
# Evaluation 

## Evaluation for folds

For evaluation of the models on the folds, we use 4 folds cross-validation.
So, as we have 40k samples, we split them into 4 folds of 10k samples on the validation. And then we trained and validated on each fold separately.

### Fold 1

|                             |        metrics |
|:----------------------------|---------------:|
| eval_loss                   |     0.00446131 |
| eval_overall_precision      |     0.783601   |
| eval_overall_recall         |     0.726919   |
| eval_overall_f1             |     0.754196   |
| eval_overall_accuracy       |     0.936082   |
| eval_macro_avg.precision    |     0.665234   |
| eval_macro_avg.recall       |     0.60265    |
| eval_macro_avg.f1-score     |     0.630713   |
| eval_macro_avg.support      | 35418          |
| eval_weighted_avg.precision |     0.780372   |
| eval_weighted_avg.recall    |     0.726919   |
| eval_weighted_avg.f1-score  |     0.751985   |
| eval_weighted_avg.support   | 35418          |
| eval_micro_avg.precision    |     0.783601   |
| eval_micro_avg.recall       |     0.726919   |
| eval_micro_avg.f1-score     |     0.754196   |
| eval_micro_avg.support      | 35418          |
| eval_runtime                |  1160.95       |
| eval_samples_per_second     |    52.292      |
| eval_steps_per_second       |    26.147      |

### Fold 2

|                             |        metrics |
|:----------------------------|---------------:|
| eval_loss                   |     0.00431787 |
| eval_overall_precision      |     0.782074   |
| eval_overall_recall         |     0.712519   |
| eval_overall_f1             |     0.745678   |
| eval_overall_accuracy       |     0.933556   |
| eval_macro_avg.precision    |     0.667987   |
| eval_macro_avg.recall       |     0.58284    |
| eval_macro_avg.f1-score     |     0.620279   |
| eval_macro_avg.support      | 36959          |
| eval_weighted_avg.precision |     0.778731   |
| eval_weighted_avg.recall    |     0.712519   |
| eval_weighted_avg.f1-score  |     0.743216   |
| eval_weighted_avg.support   | 36959          |
| eval_micro_avg.precision    |     0.782074   |
| eval_micro_avg.recall       |     0.712519   |
| eval_micro_avg.f1-score     |     0.745678   |
| eval_micro_avg.support      | 36959          |
| eval_runtime                |  1255.45       |
| eval_samples_per_second     |    52.914      |
| eval_steps_per_second       |    26.457      |

### Fold 3

|                             |        metrics |
|:----------------------------|---------------:|
| eval_loss                   |     0.00460493 |
| eval_overall_precision      |     0.804563   |
| eval_overall_recall         |     0.688634   |
| eval_overall_f1             |     0.742098   |
| eval_overall_accuracy       |     0.932954   |
| eval_macro_avg.precision    |     0.694945   |
| eval_macro_avg.recall       |     0.561292   |
| eval_macro_avg.f1-score     |     0.617365   |
| eval_macro_avg.support      | 36311          |
| eval_weighted_avg.precision |     0.798574   |
| eval_weighted_avg.recall    |     0.688634   |
| eval_weighted_avg.f1-score  |     0.737633   |
| eval_weighted_avg.support   | 36311          |
| eval_micro_avg.precision    |     0.804563   |
| eval_micro_avg.recall       |     0.688634   |
| eval_micro_avg.f1-score     |     0.742098   |
| eval_micro_avg.support      | 36311          |
| eval_runtime                |  1230.3        |
| eval_samples_per_second     |    51.72       |
| eval_steps_per_second       |    25.86       |

### Fold 4

|                             |        metrics |
|:----------------------------|---------------:|
| eval_loss                   |     0.00429184 |
| eval_overall_precision      |     0.779286   |
| eval_overall_recall         |     0.728163   |
| eval_overall_f1             |     0.752858   |
| eval_overall_accuracy       |     0.936848   |
| eval_macro_avg.precision    |     0.66828    |
| eval_macro_avg.recall       |     0.604989   |
| eval_macro_avg.f1-score     |     0.632891   |
| eval_macro_avg.support      | 35639          |
| eval_weighted_avg.precision |     0.777074   |
| eval_weighted_avg.recall    |     0.728163   |
| eval_weighted_avg.f1-score  |     0.75088    |
| eval_weighted_avg.support   | 35639          |
| eval_micro_avg.precision    |     0.779286   |
| eval_micro_avg.recall       |     0.728163   |
| eval_micro_avg.f1-score     |     0.752858   |
| eval_micro_avg.support      | 35639          |
| eval_runtime                |  1220.92       |
| eval_samples_per_second     |    52.255      |
| eval_steps_per_second       |    26.128      |

### Average

Average of the folds with range(plus/minus 1.96 std, ~95% CI):

|                             | metrics                            |
|:----------------------------|:-----------------------------------|
| eval_loss                   | 0.00 ± 0.00                        |
| eval_ANG.precision          | 0.81 ± 0.04                        |
| eval_ANG.recall             | 0.77 ± 0.04                        |
| eval_ANG.f1                 | 0.79 ± 0.04                        |
| eval_ANG.number             | 237, 243, 219, 243                 |
| eval_DUC.precision          | 0.69 ± 0.02                        |
| eval_DUC.recall             | 0.57 ± 0.04                        |
| eval_DUC.f1                 | 0.62 ± 0.02                        |
| eval_DUC.number             | 597, 555, 563, 551                 |
| eval_EVE.precision          | 0.61 ± 0.05                        |
| eval_EVE.recall             | 0.58 ± 0.03                        |
| eval_EVE.f1                 | 0.59 ± 0.01                        |
| eval_EVE.number             | 792, 937, 791, 833                 |
| eval_FAC.precision          | 0.62 ± 0.04                        |
| eval_FAC.recall             | 0.47 ± 0.03                        |
| eval_FAC.f1                 | 0.53 ± 0.01                        |
| eval_FAC.number             | 1399, 1393, 1302, 1321             |
| eval_GPE.precision          | 0.86 ± 0.01                        |
| eval_GPE.recall             | 0.82 ± 0.01                        |
| eval_GPE.f1                 | 0.84 ± 0.01                        |
| eval_GPE.number             | 8524, 8840, 8537, 8483             |
| eval_INFORMAL.precision     | 0.00 ± 0.00                        |
| eval_INFORMAL.recall        | 0.00 ± 0.00                        |
| eval_INFORMAL.f1            | 0.00 ± 0.00                        |
| eval_INFORMAL.number        | 10, 15, 12, 14                     |
| eval_LOC.precision          | 0.66 ± 0.02                        |
| eval_LOC.recall             | 0.56 ± 0.03                        |
| eval_LOC.f1                 | 0.61 ± 0.02                        |
| eval_LOC.number             | 1631, 1644, 1626, 1644             |
| eval_MISC.precision         | 0.70 ± 0.02                        |
| eval_MISC.recall            | 0.59 ± 0.01                        |
| eval_MISC.f1                | 0.64 ± 0.01                        |
| eval_MISC.number            | 2398, 2535, 2575, 2616             |
| eval_ORG.precision          | 0.74 ± 0.02                        |
| eval_ORG.recall             | 0.67 ± 0.02                        |
| eval_ORG.f1                 | 0.71 ± 0.01                        |
| eval_ORG.number             | 6265, 6411, 6415, 6326             |
| eval_PER.precision          | 0.88 ± 0.00                        |
| eval_PER.recall             | 0.83 ± 0.02                        |
| eval_PER.f1                 | 0.85 ± 0.01                        |
| eval_PER.number             | 6946, 7451, 7394, 7148             |
| eval_TIMEX.precision        | 0.82 ± 0.01                        |
| eval_TIMEX.recall           | 0.75 ± 0.02                        |
| eval_TIMEX.f1               | 0.78 ± 0.01                        |
| eval_TIMEX.number           | 3082, 3216, 3126, 2969             |
| eval_TTL.precision          | 0.69 ± 0.04                        |
| eval_TTL.recall             | 0.63 ± 0.05                        |
| eval_TTL.f1                 | 0.66 ± 0.01                        |
| eval_TTL.number             | 2815, 2980, 3025, 2768             |
| eval_WOA.precision          | 0.69 ± 0.03                        |
| eval_WOA.recall             | 0.41 ± 0.03                        |
| eval_WOA.f1                 | 0.52 ± 0.02                        |
| eval_WOA.number             | 722, 739, 726, 723                 |
| eval_overall_precision      | 0.79 ± 0.01                        |
| eval_overall_recall         | 0.71 ± 0.02                        |
| eval_overall_f1             | 0.75 ± 0.01                        |
| eval_overall_accuracy       | 0.93 ± 0.00                        |
| eval_macro_avg.precision    | 0.67 ± 0.01                        |
| eval_macro_avg.recall       | 0.59 ± 0.02                        |
| eval_macro_avg.f1-score     | 0.63 ± 0.01                        |
| eval_macro_avg.support      | 35418.0, 36959.0, 36311.0, 35639.0 |
| eval_weighted_avg.precision | 0.78 ± 0.01                        |
| eval_weighted_avg.recall    | 0.71 ± 0.02                        |
| eval_weighted_avg.f1-score  | 0.75 ± 0.01                        |
| eval_weighted_avg.support   | 35418.0, 36959.0, 36311.0, 35639.0 |
| eval_micro_avg.precision    | 0.79 ± 0.01                        |
| eval_micro_avg.recall       | 0.71 ± 0.02                        |
| eval_micro_avg.f1-score     | 0.75 ± 0.01                        |
| eval_micro_avg.support      | 35418.0, 36959.0, 36311.0, 35639.0 |
| eval_runtime                | 1216.91 ± 40.05                    |
| eval_samples_per_second     | 52.292, 52.914, 51.72, 52.255      |
| eval_steps_per_second       | 26.147, 26.457, 25.86, 26.128      |
| fold                        | fold_1, fold_2, fold_3, fold_4     |
