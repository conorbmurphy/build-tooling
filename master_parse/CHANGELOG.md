# Change Log for Master Parse Tool

Version 1.3.0:

* Master parser now generates _three_ broad kinds of notebooks: instructor, 
  exercises, and answers. 
    - The _exercises_ notebook is what used to be called the "student" notebook.
      It omits any cells marked `ANSWER`, and it omits any `INSTRUCTOR_NOTE`
      cells.
    - The _instructor_ notebook is what used to be called the "answers" notebook.
      It omits any `TODO` cells, contains all `ANSWER` cells, and contains
      reformatted `INSTRUCTOR_NOTE` cells.
    - The _answers_ notebook is almost identical to the _instructor_ notebook,
      except that it does not contain `INSTRUCTOR_NOTE` cells.
* Added deprecation warnings for `PRIVATE_TEST`, `INLINE` and 
  `IPYTHON_ONLY` labels.
* Added change log.