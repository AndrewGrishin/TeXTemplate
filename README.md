# Simple latex template

This latex project scheme should be used only for simple projects and articles. In addition, it is the author's of the repository point on structure of a latex project and should not be taken for granted as the only ground truth.
The main idea behind this work is that almost of the simple math/stats/fin.math/probability theory/etc classes
requires Home Assignments to be complied in LaTeX. This project provides a solution
for this commonly known issue.

The structure of the project is as follows (here you can see that result of linux `tree` command):

```bash
.
├── README.md
├── main.tex
└── source
    ├── bibliography
    │   └── bibliography.bib
    └── tex
        ├── Q1.tex
        ├── Q2.tex
        ├── Q3.tex
        ├── Q4.tex
        └── Q5.tex

4 directories, 8 files
```

## Detailed explanation

The `main.tex` is a file with all imports and required libraries (that could be changed if necessary). In addition the `source` folder contains all imported files structured by the topic (e.g. `Q1.tex` - stands for Question 1). All of the file-names could be changes. If so, it is also important to change names in `main.tex` to make it possible for LaTeX compiler to work properly.

## Bibliography explanation

In the `source/bibliography` folder there is a file called `bibliography.bib` that includes all references that will be used in you project. So, to add a citation adjust `bibliography.tex` file with BibTex reference in the following form:

```BibTeX
@article{vaswani2017attention,
  title={Attention is all you need},
  author={Vaswani, Ashish and Shazeer, Noam and Parmar, Niki and Uszkoreit, Jakob and Jones, Llion and Gomez, Aidan N and Kaiser, {\L}ukasz and Polosukhin, Illia},
  journal={Advances in neural information processing systems},
  volume={30},
  year={2017}
}
```

And be confident to use the `vaswani2017attention` in your latex file. Note, that you should NOT add any text into `main.tex`, as it is the main file with all the required imports and technical settings (e.g. the style of you cover-page, page numeration, style of table of contents, etc.).

## How to use

To use this project just:

1. `git clone` the repository into your desired directory.
2. open your favorite TeX editor.
3. select `main.tex` downloaded at step i.
4. you are ready to go and write your project.
