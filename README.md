# ia368v_dd_class_05
IA368v DD 5th class ― Fine tuning a Causal Language Model (CLM)

[LM_training_dataset_preparation.ipynb](LM_training_dataset_preparation.ipynb): this notebook prepares the mc4 pt dataset samples to be used for the **facebook/opt-135m** Causal Language Model fine-tuning. Shall be executed first.

[LM_training.ipynb](LM_training.ipynb): this notebook performs the actual fine-tuning of **facebook/opt-135m** Causal Language Model using 512-byte chunks of each training sample.

[LM_training_2048.ipynb](LM_training.ipynb): this notebook performs the actual fine-tuning of **facebook/opt-135m** Causal Language Model using 2048-byte chunks of each training sample.

[test_LM.ipynb](test_LM.ipynb): this notebook performs some text generation tests using the best models (based on the evaluation loss) trained using both chunk sizes.

## Final results

Here are the results for the executed trainings:

|    | eval loss | perplexity |
|----|:---: |:---: |
| 512-byte chunks | 1.981 | 7.251 |
| 2048-byte chunks | 1.242 | 3.462 |
| 2048-byte chunks<br />from scratch | ??? | ??? |


Check [here a presentation](https://docs.google.com/presentation/d/1x6j2YxTE9TBakxe6aTPegLxCDhYtQ5p4QrXjMwpQymI/edit?usp=share_link) commenting this exercise resolution.
