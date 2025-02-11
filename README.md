# masterdata-template
A template to create and work with Masterdata definitions in the BAM Data Store.

## Getting started

1. Click on **Use this template** button on the top right and create a new Masterdata repository. 

![Use this template highlight](https://github.com/BAMresearch/masterdata-template/assets/use-this-template.png)

2. The next screen will prompt you to chose a Github organization or profile for the new repository, as well as a name. We recommend you naming the repository starting with `masterdata-`, so it is easy to be recognized.
3. After creating your new repository, you can:
    1. Open in Github Codespace
    2. Clone it locally
4. You need to [install `cruft`](https://cruft.github.io/cruft/#creating-a-new-project).
5. Run the following command to create the structure of the new Masterdata project:
```sh
cruft create https://github.com/BAMresearch/masterdata-generator
```

This will prompt you with some questions to be filled in:
```sh
<questions here>
```

6. After filling the questionnaire, you will have a new repository with:
```sh
masterdata-<name>/
├── LICENSE (MIT)
├── README.md
├── pyproject.toml
├── src/
│   └── masterdata-<name>/
│       ├── __init__.py
#        if Python is selected as an option
│       ├── object_types.py
│       ├── property_types.py
│       ├── vocabulary_types.py
#       if Excel is selected as an option
│       ├── masterdata.xlsx
#       if RDF/XML is selected as an option
│       └── masterdata.owl
└── tests/
    ├── __init__.py
    └── test.py
```