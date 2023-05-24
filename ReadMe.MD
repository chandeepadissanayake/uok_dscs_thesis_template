# LaTeX Thesis Template DSCS/UoK

This is a LaTeX thesis template used by the undergraudates at Department of Statistics & Computer Science for final year undergraduate research project.
Mostly in compliance with BSc. (Hons) Computer Science, BSc. (Hons) Computer Studies, BA. (Hons) Computer Studies requirements.

Please note that this is by no means official and merely created by student(s) themselves. The department bears no responsibility or liability regarding this template and may change depending on the requirements of the department.

Use at your own discretion.

# Instructions for Usage

1. Update the contents of the following pages as per the instructions found in them:
    - Thesis Information: `thesis_info.tex`
    - Personnel Information (involved with the research): `personnel_info.tex`

2. Add contents to the following pages with your own customized writings:
    - Dedication: `pages/dedication.tex`
    - Acknowledgement: `pages/acknowledgements.txt`

3. Add definitions of terms that you anticipate using in the thesis in `definitions.tex`.
    - The instructions have been provided in the file.

4. Add the list of abbreviations that you anticipate using in the thesis in `abbreviations.tex`.
    - The instructions have been provided in the file.

5. Write the abstract of your work in `research/abstract.tex`.
    - Instructions and guidelines are found in the file.

6. Craft the contents in the following files which correspond to your research work:
    - 6.1 Introduction: `research/introduction/index.tex`
        - 6.1.1 Background: `research/introduction/background.tex`
        - 6.1.2 Objectives: `research/introduction/objectives.tex`
        - 6.1.3 Significance: `research/introduction/significance.tex`
        - Any other sub-sections could be added as guided in the file.

    - 6.2 Literature Review: `research/literature_review/index.tex`
        - Any sub-sections could be added as guided in the file.

    - 6.3 Methodology: `research/methodology/index.tex`
        - Any sub-sections could be added as guided in the file.

    - 6.4 Results and Discussion: `research/results_and_discussion/index.tex`
        - Any sub-sections could be added as guided in the file.

    - 6.5 Conclusions: `research/conclusions/index.tex`
        - 6.5.1 Limitations: `research/conclusions/limitations.tex`
        - 6.5.2 Future Work: `research/conclusions/future_work.tex`
        - Any other sub-sections could be added as guided in the file.

    - 6.6 Appendices: `research/appendices/index.tex`
        - Follow the in-file instructions for adding appendices.

    - Following guidelines must be followed when compiling the contents in the pages under 6:
        - Tables:
            - Use the `table` tag to define all tables. Borders must be visible and 1pt.
            - Headers must be in boldface.
            - Tables must be captioned and centered.
            - Padding must be such that the borders don't touch the text in every cell.
            - Text in each cell must be left-aligned (flushed left).
        - Figures:
            - Use the `figure` tag to define all figures.
            - Figures must be captioned.
            - All figures must ONLY be uploaded to the `resources/figures` folder.
        - References:
            - All reference material that is used must be defined in `research/references.tex`. This can be achieved in either of the following methods:
                - Defined as a list in `references.tex` using `\bibitem`. Refer to: [Bibliography Management with BibTeX](https://www.overleaf.com/learn/latex/Bibliography_management_with_bibtex).
                - Defined in a .bib file, typically exported from a reference management tool. Steps are as follows:
                    1. Upload all .bib files into the `resources/references` folder.
                    2. Add all files as references into `research/references.tex` file using the tag: `\bibliography{bib_file_name.bib}`.

**Important NOTE:**
- Add any packages that you need to use in your compilation in `settings/user_dependencies.tex`.

**Additional Notes:**
- Do NOT attempt to change the contents of portions of markup where it is explicitly specified not to do so unless you're assured about what you're doing.
- Contents inside `settings/global.tex` are better left intact. Changing them would cause large and possibly catastrophic changes to the styles.
- Do not change any template dependencies in `settings/template_dependencies.tex` as well.
- It's better not to change the folder structure.
- You can add any custom environments inside the `envs` folder, but be cautious in doing so.
