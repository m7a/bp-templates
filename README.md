---
section: 32
x-masysma-name: templates
title: Ma_Sys.ma “New File” Templates
date: 2021/02/02 19:12:11
lang: en-US
author: ["Linux-Fan, Ma_Sys.ma (Ma_Sys.ma@web.de)"]
keywords: ["mdvl", "templates", "tex", "vector", "new", "file", "ma_new_file", "cc0"]
x-masysma-version: 1.0.0
x-masysma-repository: https://www.github.com/m7a/bp-templates
x-masysma-website: https://masysma.lima-city.de/32/templates.xhtml
x-masysma-copyright: |
  Copyright (c) 2020 Ma_Sys.ma.
  For further info send an e-mail to Ma_Sys.ma@web.de.
---
Template Files
==============

This package provides a set of files that can be used to create “new” files of
the same type. The following files are noteworthy templates:

------------------------  ------------------------------------------------
`latex_document.tex`      For regular texts
`latex_presentation.tex`  For beamer presentations
`xhtml_1_page.xhtml`      XHTML 1.0 webpage template
`svg_file.svg`            SVG empty image
`empty_file`              Empty file (general purpose, new text file etc.)
------------------------  ------------------------------------------------

Additionally, there are some files to be used in conjunction with other
Ma_Sys.ma content. `build_*.xml` files instantiate
[masysmaci/build(32)](masysmaci_build.xhtml) and `overview_conf.sh` is
related to `scrapbook_overview` from [shellscripts(32)](shellscripts.xhtml).

-------------------  --------------------------------------------------
`build_file.xml`     Template `build.xml` to compile programs/documents
`build_package.xml`  Template `build.xml` to generate a package
`overview_conf.sh`   Create configuration for `scrapbook_overview`
-------------------  --------------------------------------------------

If [d5man2(32)](d5man2.xhtml) is installed, template `d5man2.md` becomes
available to create empty D5Man 2 pages.

Script `ma_new_file`
====================

## Name

`ma_new_file` -- select template file to copy to current working directory

## Synopsis

	ma_new_file

## Description

Interactively displays the list of available template files and allows the user
to select one of the files. After pressing [ENTER], the selected file is copied
to the present working directory.

## Examples

Here is an example output. If [ENTER] is pressed at this time, template
`empty_file` is copied to the present working directory.

~~~
-------------------------------------------------------------------------
 Ma_Sys.ma Template File Selector 1.0.0.3, Copyright (c) 2012 Ma_Sys.ma.
 For further info send an e-mail to Ma_Sys.ma@web.de.
-------------------------------------------------------------------------

[j] and [k] to select, [enter] or [l] to accept, [h] or [q] to abort.

 ) build_file.xml
 ) build_package.xml
 ) d5man2.md
 ) empty_dir
*) empty_file
 ) latex_document.tex
 ) latex_presentation.tex
 ) overview_conf.sh
 ) svg_file.svg
 ) xhtml_1_page.xhtml
~~~

`ma_new_file` integrates well into terminal-based file management applications
like `vifm`. If [conf-cli(32)](conf-cli.xhtml) is used, shortcut `ön` is mapped
to `ma_new_file` in `vifm`.

## Bugs

 * The script fails to display its UI properly if the window is too small.
 * Code quality could be enhanced. Given that such script is likely to already
   exist with a better implementation, it seems sensible to replace it with an
   existing alternative once such an alternative is found.

License Information
===================

Ma_Sys.ma Templates are newly licensed under CC0-1.0 to make sure that
the templates can be freely used to create documents under any license of
the respective author's choice.

See /usr/share/common-licenses/CC0-1.0 on any Debian system or
<https://creativecommons.org/publicdomain/zero/1.0/legalcode>
