<!--- This file was automatically generated. Do not modify it manually but use the docs/options/generate.sh script instead. -->

`preprocess.lua` options:

* `-h`<br/>This help.
* `-md`<br/>Dump help in Markdown format.
* `-config <string>`<br/>Load options from this file.
* `-save_config <string>`<br/>Save options to this file.

## Preprocess options

* `-data_type <string>` (accepted: `bitext`, `monotext`; default: `bitext`)<br/>Type of data to preprocess. Use 'monotext' for monolingual data. This option impacts all options choices.
* `-save_data <string>`<br/>Output file for the prepared data.

## Data options

* `-train_src <string>`<br/>Path to the training source data.
* `-train_tgt <string>`<br/>Path to the training target data.
* `-valid_src <string>`<br/>Path to the validation source data.
* `-valid_tgt <string>`<br/>Path to the validation target data.
* `-src_vocab <string>`<br/>Path to an existing source vocabulary.
* `-tgt_vocab <string>`<br/>Path to an existing target vocabulary.
* `-src_vocab_size <string>` (default: `50000`)<br/>Comma-separated list of source vocabularies size: `word[,feat1[,feat2[,...] ] ]`. If = 0, vocabularies are not pruned.
* `-tgt_vocab_size <string>` (default: `50000`)<br/>Comma-separated list of target vocabularies size: `word[,feat1[,feat2[,...] ] ]`. If = 0, vocabularies are not pruned.
* `-src_words_min_frequency <string>` (default: `0`)<br/>Comma-separated list of source words min frequency: `word[,feat1[,feat2[,...] ] ]`. If = 0, vocabularies are pruned by size.
* `-tgt_words_min_frequency <string>` (default: `0`)<br/>Comma-separated list of target words min frequency: `word[,feat1[,feat2[,...] ] ]`. If = 0, vocabularies are pruned by size.
* `-src_seq_length <number>` (default: `50`)<br/>Maximum source sequence length.
* `-tgt_seq_length <number>` (default: `50`)<br/>Maximum target sequence length.
* `-features_vocabs_prefix <string>`<br/>Path prefix to existing features vocabularies.
* `-time_shift_feature <number>` (default: `1`)<br/>Time shift features on the decoder side.
* `-sort <number>` (default: `1`)<br/>If = 1, sort the sentences by size to build batches without source padding.
* `-shuffle <number>` (default: `1`)<br/>If = 1, shuffle data (prior sorting).

## Logger options

* `-log_file <string>`<br/>Output logs to a file under this path instead of stdout.
* `-disable_logs`<br/>If set, output nothing.
* `-log_level <string>` (accepted: `DEBUG`, `INFO`, `WARNING`, `ERROR`; default: `INFO`)<br/>Output logs at this level and above.

## Other options

* `-seed <number>` (default: `3425`)<br/>Random seed.
* `-report_every <number>` (default: `100000`)<br/>Report status every this many sentences.

