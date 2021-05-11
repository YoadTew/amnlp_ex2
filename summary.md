Student 1:
* Name: Roni Paiss
* ID: 316124833
* Username: ronipaiss

Student 2:
* Name: Nitzan Hodos
* ID: 322756123
* Username: nitzanhodos

Student 3:
* Name: Yoad Tewel
* ID: 313417172
* Username: yoadtewel

Now, for each log file that you need to submit, you will need to write its last 3 lines. For example, this is what we got for `baseline_gen.log`:
```txt
2021-04-24 17:20:46 | INFO | fairseq_cli.generate | NOTE: hypothesis and token scores are output in base 2
2021-04-24 17:20:46 | INFO | fairseq_cli.generate | Translated 7,283 sentences (165,025 tokens) in 18.5s (394.00 sentences/s, 8927.61 tokens/s)
Generate valid with beam=5: BLEU4 = 33.39, 69.1/42.8/28.5/19.4 (BP=0.934, ratio=0.937, syslen=138824, reflen=148229)
```

3 last lines from the baseline_train.log file: 
```txt
2021-05-10 15:18:28 | INFO | fairseq_cli.train | end of epoch 50 (average epoch stats below)
2021-05-10 15:18:28 | INFO | train | epoch 050 | loss 3.945 | nll_loss 2.516 | ppl 5.72 | wps 46329 | ups 4.45 | wpb 10419.8 | bsz 422.8 | num_updates 18950 | lr 0.000229718 | gnorm 0.624 | train_wall 58 | gb_free 4.8 | wall 4187
2021-05-10 15:18:28 | INFO | fairseq_cli.train | done training in 4186.5 seconds
```

3 last lines from the baseline_gen.log file: 
```txt
2021-05-10 15:20:45 | INFO | fairseq_cli.generate | NOTE: hypothesis and token scores are output in base 2
2021-05-10 15:20:45 | INFO | fairseq_cli.generate | Translated 7,283 sentences (167,540 tokens) in 16.2s (450.28 sentences/s, 10358.45 tokens/s)
Generate valid with beam=5: BLEU4 = 33.56, 68.5/42.4/28.2/19.2 (BP=0.948, ratio=0.949, syslen=140728, reflen=148229)
```

3 last lines from the baseline_mask.log file: 
```txt
2021-05-10 16:55:55 | INFO | fairseq_cli.generate | NOTE: hypothesis and token scores are output in base 2
2021-05-10 16:55:55 | INFO | fairseq_cli.generate | Translated 7,283 sentences (169,064 tokens) in 15.8s (459.89 sentences/s, 10675.59 tokens/s)
Generate valid with beam=5: BLEU4 = 32.13, 66.9/40.6/26.4/17.5 (BP=0.959, ratio=0.960, syslen=142342, reflen=148229)
```

25 last lines from the check_all_masking_options.log file: 
```txt
2021-05-10 17:27:18 | INFO | fairseq.tasks.translation | data-bin/iwslt14.tokenized.de-en valid de-en 7283 examples
2021-05-10 17:27:56 | INFO | fairseq_cli.generate | NOTE: hypothesis and token scores are output in base 2
2021-05-10 17:27:56 | INFO | fairseq_cli.generate | Translated 7,283 sentences (167,410 tokens) in 14.3s (510.70 sentences/s, 11739.07 tokens/s)
Generate valid with beam=5: BLEU4 = 33.25, 68.4/42.2/27.9/18.8 (BP=0.948, ratio=0.950, syslen=140772, reflen=148229)
table of score with masking enc-enc attention head
rows are transformer layer number and columns are head number
       0      1      2      3
0  33.52  33.39  33.24  33.33
1  33.38  33.53  33.42  33.22
2  33.48  32.90  32.32  33.42
3  33.37  33.03  29.80  33.56
table of score with masking enc-dec attention head
rows are transformer layer number and columns are head number
       0      1      2      3
0  33.42  33.31  18.29  33.10
1  32.99  33.39  33.13  33.31
2  33.21  33.32  32.74  32.57
3  32.13  32.73  32.31  32.44
table of score with masking dec-dec attention head
rows are transformer layer number and columns are head number
       0      1      2      3
0  33.44  33.36  33.33  33.42
1  33.50  33.28  33.29  33.55
2  33.67  33.58  32.54  33.36
3  33.37  33.53  33.41  33.25
```

3 last lines from the sandwich_train.log file: 
```txt
2021-05-11 16:10:22 | INFO | fairseq_cli.train | end of epoch 50 (average epoch stats below)
2021-05-11 16:10:22 | INFO | train | epoch 050 | loss 3.969 | nll_loss 2.542 | ppl 5.82 | wps 47368.8 | ups 4.55 | wpb 10419.8 | bsz 422.8 | num_updates 18950 | lr 0.000229718 | gnorm 0.623 | train_wall 57 | gb_free 4.8 | wall 4242
2021-05-11 16:10:22 | INFO | fairseq_cli.train | done training in 4242.1 seconds
```

3 last lines from the sandwich_gen.log file: 
```txt
2021-05-11 17:49:01 | INFO | fairseq_cli.generate | NOTE: hypothesis and token scores are output in base 2
2021-05-11 17:49:01 | INFO | fairseq_cli.generate | Translated 7,283 sentences (168,099 tokens) in 15.4s (473.69 sentences/s, 10933.19 tokens/s)
Generate valid with beam=5: BLEU4 = 33.21, 68.0/41.8/27.7/18.8 (BP=0.953, ratio=0.954, syslen=141381, reflen=148229)
```