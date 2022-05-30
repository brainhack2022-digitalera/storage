# BrainHack 2022 - Team: DigitalEra (Storage)

This GitHub Repository is intended to hold resources that the DigitalEra team may need.

Currently, it's used to re-host the datasets from `falldataset.com` as the original download links take too long to download.

Each dataset can be downloaded individually from the [releases page](https://github.com/brainhack2022-digitalera/storage/releases), or they can be downloaded using a Metalink 4.0-compatible downloader such as `aria2c`.

To download all of the datasets using `aria2c`:

```sh
aria2c --check-integrity \
  https://github.com/brainhack2022-digitalera/storage/raw/main/combined-datasets.meta4
```

Certain datasets are missing certain files. To download all of the fixed and not-broken datasets using `aria2c`:

```sh
aria2c --check-integrity \
  https://github.com/brainhack2022-digitalera/storage/raw/main/combined-datasets-fixed.meta4
```

Note that we may move the Metalink files around, and it's recommended that you pin to a specific Git Commit Hash (i.e. replace `main` with a hash). However, we'll try to keep the download links in the GitHub release as-is.

Confusingly, the file is called `combined-datasets.meta4` even though each dataset archive is still downloaded individually. Hence it should probably be called `all-datasets.meta4` to more-accurately reflect its purpose.

`test-datasets.meta4`, `train-datasets.meta4`, `unclassified-dataset.meta4`, and `validate-dataset.meta4` can be used instead if only those specific datasets are required. Likewise, those ending with `-fixed.meta4` can be used to download only those specific fixed and non-broken datasets.

For the fixed dataset archives, their extracted directory name is the original directory. For example, `1373-fixed.tar.gz` would extract a top-level `1373` directory, not `1373-fixed`.

Metalinks are useful because they allow one-shot downloads and checksum verification.

With the `--check-integrity` flag, `aria2c` will not re-download files if they already already exist in the working (or specified) directory, have the same file size, and has a matching hash.

The datasets are also listed below with their MD5 and SHA-1 hash digests: 

## Datasets

| Source | Title | Type | Download URL | MD5 | SHA-1
|-|-|-|-|-|-
falldataset.com | 489  | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%23439/489.tar.gz) | 46c09938b83d4585c007028e2da7e910 | ccacec096f7aa62478edabf633eb5438483c6a77
falldataset.com | 569  | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%23569/569.tar.gz) | 8f5efd3453c75a4cf6a33a268e68d636 | 785bf644c10a38ff6618f59a3bb70ae797e144c0
falldataset.com | 581  | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%23581/581.tar.gz) | da8e9a2bc20d17b6d277bfce37aab1ef | 47e170343b975d20ab8c5dd276728ce7bbdbc4a2
falldataset.com | 722  | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%23722/722.tar.gz) | faa23335696db09f5fbae4f40be759c3 | ec82cdb177523891b67702e26cdc476fc959175a
falldataset.com | 731  | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%23731/731.tar.gz) | b3caa539ad90bc6e201ed6ec8875f46e | 796b53cada0c61c3f6a64d4e2f0757a22fb8fe63
falldataset.com | 758  | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%23758/758.tar.gz) | 74ccf32fe7b6bf8f09992c80e5e04068 | 21f11fd1b8da619949c908d9d95d9d7726020120
falldataset.com | 786  | Test     | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%23786/786.tar.gz) | 48425ef5b3cf85a6f2819a0886be9cdc | 30aa1665b51ecad5d17db152b51d213c260732c8
falldataset.com | 807  | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%23807/807.tar.gz) | a7f49238799740f763c3194c4bf0bb30 | 62a7edf96a9a6bb6fdb7db52447a47cf2ab31b1f
falldataset.com | 832  | Test     | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/%23dataset-fall-%23832/832.tar.gz) | 2ffb24981459d363b16c789f74448e36 | 9d77ef0ae59702cc1128b05c87ab10a7562f4adc
falldataset.com | 925  | Test     | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%23925/925.tar.gz) | fd17e009a6020c9bbe88412d680af360 | 8ce5a6fbb5200c11f7f19d5746f2bbdc60706d01
falldataset.com | 1176 | Validate | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231176/1176.tar.gz) | 56e5013f678b8b626c9d94a25b7d7deb | 6d6fda9132505d0286a071357a75ba37f26a5c61
falldataset.com | 1219 | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231219/1219.tar.gz) | 5719d3296582103dd6dc3ef61621f7e1 | ec420ad45281ff492ec0687e247e8d0f6976924b
falldataset.com | 1260 | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231260/1260.tar.gz) | 529d7da0cd48332c2c9c5323ee37038b | bebcb60246df350e6cf6fd695f635657acb8e6f7
falldataset.com | 1301 | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231301/1301.tar.gz) | 9812af94c3a89469030cf51a78a205a1 | 463bae7e7af3c0fa026f7950da7a1d6eb2c51da7
falldataset.com | 1373 | ???      | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231373/1373.tar.gz) | 870af0cef3b8026f3cd7b888c4b495df | 278f5b3d3143a0f9a69c8e7cea022782dffc0135
falldataset.com | 1373-fixed | ???      | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231373/1373-fixed.tar.gz) | 7de82b38fa3c335ab5eefdba4e94eb5f | 8b27039fa2709109ae3ed55313234cd91521ae8c
falldataset.com | 1378 | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231378/1378.tar.gz) | 6cbd1945bb5e0038ea650ed6c6e4a83f | 1ffb2616ca6d3bd9833110ac71cf97c9cd2dfe5f
falldataset.com | 1392 | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231392/1392.tar.gz) | 9be9f2cf50e1284c6242ffc703bc3157 | 60c05293dff710d0567e1dde2b1ed58766464906
falldataset.com | 1790 | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231790/1790.tar.gz) | 1f8540475738ddd31816be363e601e39 | e45f38bfb427adb803374be75a905907af683da1
falldataset.com | 1790-fixed | Train      | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231790/1790-fixed.tar.gz) | 4013cfed2a80d5a633af6a75b9bea966 | 46ae84f32922aa32fd1704878aff850707069789
falldataset.com | 1843 | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231843/1843.tar.gz) | 30c2a314364260af94907fa3bbc12925 | 196e27f3415321d1c21453a67e4ee24bbc5a8e1d
falldataset.com | 1843-fixed | Train      | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231843/1843-fixed.tar.gz) | be71b420496fdcbeb26e58f7f21c310b | bdc4f92aa50758fcdd632695b069cb4118270150
falldataset.com | 1954 | Train    | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%231954/1954.tar.gz) | 2e5c1789b03eb305835eefc7e757757b | 40928b715ada91638f19d00990a65904ad91ccbb
falldataset.com | 2123 | Validate | [Link](https://github.com/brainhack2022-digitalera/storage/releases/download/dataset-fall-%232123/2123.tar.gz) | a9c13a26ed4cd460e39aa3ddcec2976f | e649415fff97293f3b8bed17e8a722004bd20aa3
