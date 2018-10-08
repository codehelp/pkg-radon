:Version: 2.3.1
:Copyright: 2012-2017 Michele Lacchia
:Title: radon
:subtitle: Python tool to compute code metrics
:Manual section: "1"

Description
============

``radon`` is a Python tool which computes various code metrics.

Summary
#######

Radon is a Python tool which computes various code metrics. Supported metrics are:

* raw metrics: SLOC, comment lines, blank lines, etc.
* Cyclomatic Complexity (i.e. McCabe's Complexity)
* Halstead metrics (all of them)
* the Maintainability Index (a Visual Studio metric)

Radon can be used either from the command line or programmatically through its API.

Usage
#####

radon [-h] [-v] {cc,raw,mi,hal} ...

positional arguments
####################

  {cc,raw,mi,hal}

    cc             Analyze the given Python modules and compute Cyclomatic Complexity (CC).

    raw            Analyze the given Python modules and compute raw metrics.

    mi             Analyze the given Python modules and compute the Maintainability Index.

    hal            Analyze the given Python modules and compute their Halstead metrics.

optional arguments
##################

  -h, --help       show this help message and exit
  -v, --version    show program's version number and exit

Links
#####

https://dzone.com/articles/what-exactly-is-mccabe-cyclomatic-complexity

Cyclomatic Complexity can be seen simply as the number of independent paths that exist between the input of the function and its output

``radon`` output consists of columns. The first column indicates ``F M C`` - or ``function`` ``method`` ``class``.

Use --exclude ``"*/filename.py"`` to skip a particular file(s)
