# CS6101 Exploration of Computer Science Research: Deep Reinforcement Learning

This repository is adapted from [StanfordVL's CS131 repository](https://github.com/StanfordVL/cs131_notes.git)

## Instructions for creating class notes

As a scribe for the course, you have been assigned to the scribe role by Min and Wee Sun for a specific lecture as indicated in the Google Sheet that is pinned to the [Slack channel](https://cs6101.slack.com).  The below instructions then apply when this duty is rotated to you.

### Overall workflow
1. Fork this repository by clicking the "Fork" button on the top right of [this
page](https://github.com/j0/cs6101_notes).

2. Next, clone your forked repository into your local machine:
```
git clone github.com/YOUR_GITHUB_ACCOUNT/cs6101_notes.git
```
3. Give others permission to commit to your forked repository by clicking on
"Settings" and then "Collaborators".
3. Write up the class notes.
4. Push your changes to your forked repository.
5. Send a pull request to the official
[repository](https://github.com/j0/cs6101_notes).

### Downloading the software and testing the repository.
1. Download [pdflatex](https://www.tug.org/applications/pdftex/) so that you can
compile the tex documents. You can also use [Overleaf](overleaf.com) or
[Sharelatex](sharelatex.com) to compile your tex documents.

2. Go into the template folder and compile the format and template files:
```
cd template

pdflatex format.tex
bibtex format
pdflatex format.tex

pdflatex template.tex
bibtex template
pdflatex template.tex
```

3. Make sure that template.pdf and format.pdf have been generated and are correctly
displayed. Read format.pdf to understand how we expect the class notes to be
formatted.

### Writing class notes for a given lecture
1. Create a folder called `wXX` where `XX` is `03` for the first lecture (since the course starts on Week 3
or `13` for the final, thirteenth lecture.  For the recess week, the naming should be 'w-recess'.  These names 
should be congruent to those in the Slack preparation channels.  

2. Copy over template.tex and bibliography.bib to your folder.
```
cp template/template.tex wXX/wXX.tex
cp template/bibliography.bib wXX/bibliography.bib
```

3. Write the lecture notes. Make sure to include pictures, references and
tables. If you add images, make sure to give credit to the source of those
images.

4. Compile your lecture template to make sure that it formats correctly.
```
cd wXX
pdflatex wXX.tex
bibtex wXX
pdflatex wXX.tex
```

5. Submit a pull request to have your lecture notes merged.
