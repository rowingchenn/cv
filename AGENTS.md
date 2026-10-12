# Editing this CV

- Maintain `cv.tex` as a standalone LaTeX source and keep the design restrained.
- User-provided updates are authoritative. Ask about conflicting dates or paper
  status rather than inventing facts, achievements, affiliations, or metrics.
- Distinguish personal contributions from capabilities of a collaborative project.
- Keep original attachments and private editorial notes in ignored `private/`.
- Operate Git and GitHub as `weichen`. Use author and committer identity
  `Weichen Zhang <132875964+rowingchenn@users.noreply.github.com>`.
- Before committing, check `git var GIT_AUTHOR_IDENT` and
  `git var GIT_COMMITTER_IDENT`. Before pushing, verify that
  `gh api user --jq .login` is `rowingchenn`.
- Compile after substantive edits and check page count and layout warnings.
