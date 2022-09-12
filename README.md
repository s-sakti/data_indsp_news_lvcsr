# INDspeech03: INDspeech_NEWS_LVCSR

This is the first Indonesian speech dataset for large vocabulary continuous speech recognition (LVCSR). R&D Division of PT Telekomunikasi Indonesia developed the data in 2005-2006, in collaboration with [Advanced Telecommunication Research Institute International (ATR) Japan](https://www.atr.jp/), as the continuation of the Asia-Pacific Telecommunity (APT) project [[Sakti et al., 2004](https://www.isca-speech.org/archive_v0/interspeech_2004/i04_1037.html)]. It has also been successfully used for developing Indonesian LVCSR in the Asian speech translation advanced research (A-STAR) project [[Sakti et al., 2013](https://www.sciencedirect.com/science/article/pii/S0885230811000404)].

## Text and Speech Resources

The raw text source is based on Indonesian daily news and consists of more than 3160 articles with about 600,000 sentences. It was then further processed to generate a clean text corpus. 

We then selected phonetically-balanced sentences from the raw text data, which was assumed to cover almost all phonetic contexts used in the Indonesian language. A total of 3,168 sentences are produced using [the greedy search algorithm](https://www.internationalphoneticassociation.org/icphs-proceedings/ICPhS2003/papers/p15_3145.pdf). The table below shows the number of units and coverage rate.

|       Phone     | # Units | # Sentences | 
| --------------- | ------- |------------ |
| Monophones      |      33 |           6 | 
| Left Biphones   |     809 |         240 | 
| Right Biphones  |     809 |         242 | 
| Triphones       |    9667 |        2878 | 

After that, 400 speakers (200 males and 200 females) with Batak, Javanese, and Sundanese accents, plus standard Indonesian (no accent), uttered 110 sentences resulting in a total of 44,000 speech utterances or about 43.35 hours of speech. The recording is conducted in parallel for both clean and telephone speech, but we open only the clean speech due to quality issues on telephone speech. Each audio file is a single-channel 16-bit PCM WAV with a sample rate of 16 kHz.

## File Format

```
"Ind001_F_B_C_news_0065.wav" 
```

- Speaker ID: IndXXX
- Gender ID: F or M
- Accent ID: B (Batak), J (Javanese), S (Sundanese), or U (Umum)
- Type ID: C (Clean) 
- Utterance ID: XXXX 

## License

This data is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) International License (see LICENSE_CC-BY-NC-SA-4.0.txt). You can use the data free for non-commercial purposes, but you have to cite our paper if your work uses our data in your publication. If you remix, transform or build upon the material, you must distribute your contributions under the same license as the original. Furthermore, you are not allowed to create a copy of this dataset and share it publicly in your own repository without our permission.

## Citation

Please cite the following papers:

[[Sakti et al., 2008](https://aclanthology.org/I08-8004/)]:

```
@inproceedings{sakti-tcast-2008,
    title = "Development of {I}ndonesian Large Vocabulary Continuous Speech Recognition System within {A-STAR} Project",
    author = "Sakti, Sakriani and Kelana, Eka and Riza, Hammam and Sakai, Shinsuke and Markov, Konstantin and Nakamura, Satoshi",
    booktitle = "Proc. IJCNLP Workshop on Technologies and Corpora for Asia-Pacific Speech Translation (TCAST)",
    year = "2008",
    pages = "19--24"
    address = "Hyderabad, India"
}
```

[[Sakti et al, 2004](https://www.isca-speech.org/archive_v0/interspeech_2004/i04_1037.html)]:

```
@inproceedings{sakti-icslp-2004,
    title = "Indonesian Speech Recognition for Hearing and Speaking Impaired People",
    author = "Sakti, Sakriani and Hutagaol, Paulus and Arman, Arry Akhmad and Nakamura, Satoshi",
    booktitle = "Proc. International Conference on Spoken Language Processing (INTERSPEECH - ICSLP)",
    year = "2004",
    pages = "1037--1040"
    address = "Jeju Island, Korea"
}
```

[[Sakti et al., 2013](https://www.sciencedirect.com/science/article/pii/S0885230811000404)]
```
@article{sakti-s2st-csl-2013,
    title = "{A-STAR}: Toward Tranlating Asian Spoken Languages",
    author = "Sakti, Sakriani and Paul, Michael and Finch, Andrew and Sakai, Shinsuke and Thang, Tat Vu, and Kimura, Noriyuki 
    and Hori, Chiori and Sumita, Eiichiro and Nakamura, Satoshi and Park, Jun and Wutiwiwatchai, Chai and Xu, Bo and Riza, Hammam 
    and Arora, Karunesh and Luong, Chi Mai and Li, Haizhou",
    journal = "Special issue on Speech-to-Speech Translation, Computer Speech and Language Journal",
    volume = "27",
    number ="2",
    pages = "509--527",
    year = "2013",
    publisher = "Elsevier"
}
```
