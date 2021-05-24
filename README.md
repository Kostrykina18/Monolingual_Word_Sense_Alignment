# Multilingual Models for Monolingual Word Sense Alignment

Monolingual Word Sense Alignment (MWSA) — is the task of aligning the senses of words in resourses in one language. Since the word can be defined in different ways in different resources, it is required to find out which of them are somehow related to each other.

#### Code for training XLM-R model on MWSA datasets - [train_model.ipynb](https://github.com/Kostrykina18/Monolingual_Word_Sense_Alignment/blob/main/train_model.ipynb)

#### Code for training pretrained on XNLI XLM-R model on MWSA datasets - [train_on_XNLI_model.ipynb](https://github.com/Kostrykina18/Monolingual_Word_Sense_Alignment/blob/main/train_on_XNLI_model.ipynb)

#### Code for training XLM-R model on XNLI dataset - [XNLI_pretraining.ipynb](https://github.com/Kostrykina18/Monolingual_Word_Sense_Alignment/blob/main/XNLI_pretraining.ipynb)

#### Datasets CSV format [1] - [datasets](https://github.com/Kostrykina18/Monolingual_Word_Sense_Alignment/tree/main/MWSA_datasets)

## Example of a training sample:

|  lemma  |    pos    |                                  sense source                                  |                                    sense target                                    | semantic relationship |
|:-------:|:---------:|:------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------:|:---------------------:|
|  agree  |    verb   | to have the same opinion as                                                    | to say the same thing                                                              |        related        |
|  гибкий | adjective | Легко сгибаемый, упругий.                                                      | Способный легко гнуться, сгибаться, изгибаться.                                    |         exact         |
| bramido |    noun   | figurativamente, voces de ira que da una persona.                              | grito o voz fuerte y confusa del hombre cuando está colérico y furioso.            |        broader        |
|  Haus   |    noun   | eine Reihe von adligen Persönlichkeiten, Herrschern hervorgebrachtes Geschlech | Eine Familie und ihre Nachkommen, z.B. ein Königshaus.                             |        narrower       |

 
## Reference
[1] Datasets:
~~~
@inproceedings{ahmadi2020multilingual,
	title={A Multilingual Evaluation Dataset for Monolingual Word Sense Alignment},
	author="Ahmadi, Sina and McCrae, John P. and Nimb, Sanni and Khan, Fahad and Monachini, Monica and Pedersen, Bolette S. and Declerck, Thierry and Wissik, Tanja and Bellandi, Andrea and Pisani, Irene and Troelsgård, Thomas and Olsen, Sussi and Krek, Simon and Lipp, Veronika and Váradi, Tamás and Simon, László and Győrffy, András and Tiberius, Carole and Schoonheim, Tanneke and Ben Moshe, Yifat and Rudich, Maya and Abu Ahmad, Raya and Lonke, Dorielle and Kovalenko, Kira and Langemets, Margit and Kallas, Jelena and Dereza, Oksana and Fransen, Theodorus and Cillessen, David and Lindemann, David and Alonso, Mikel and Salgado, Ana and Sancho, José Luis and Ureña-Ruiz, Rafael-J. and Simov, Kiril and Osenova, Petya and Kancheva, Zara and Radev, Ivaylo and Stanković, Ranka and Perdih, Andrej and Gabrovšek, Dejan",
	booktitle="Proceedings of the 12th Language Resource and Evaluation Conference (LREC 2020)",
	year={2020},
	date="2020-05-11",
	address= "Marseille, France"
}
~~~
