# Explainability and Hate Speech

Official repository for _"Explainability and Hate Speech: Structured Explanations Make Social Media Moderators Faster"_.

## Annotation Scheme

The file `annotations.csv` contains the collected annotations after filtering out the outliers (see papers for details).

The csv file contains the following columns:
- _annotator_: the numerical ID assigned to the moderator who completed the annotation.
- _instance_: the ID of the annotated post. Post IDs are taken from the [PLEAD](https://github.com/Ago3/PLEAD) dataset.
- _length_: the number of characters in the post.
- _scenario_: the ID of the scenario. _s1_ corresponds to the scenario where no explanations were shown, _s2_ corresponds to the scenario with generic explanations and _s3_ refers to the scenario with structured explanations.
- _time_: the annotation time in seconds.
- _label_: 1 for posts that violate the policy, 0 for posts that comply with the policy.
- _prediction_: 1 if the moderator thought the post violates the policy, 0 otherwise.

## Reference
If you use our dataset or model, please cite our paper:
```
@article{calabrese-etal-2024-structured-explanations,
  author    = {Agostina Calabrese and
               Leonardo Neves and
               Neil Shah and
               Maarten W. Bos and
               Bj{\"{o}}rn Ross and
               Mirella Lapata and
               Francesco Barbieri},
  title     = {Explainability and Hate Speech: Structured Explanations Make Social Media Moderators Faster},
  journal   = {Proceedings of the 62nd Annual Meeting of the Association for Computational Linguistics},
  year      = {2024}
}
```
