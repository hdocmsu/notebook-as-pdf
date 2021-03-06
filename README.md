# Jupyter Notebooks as PDF

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/betatim/notebook-as-pdf/master)

This Jupyter notebook extension allows you to save your notebook as a PDF.

Three new features compared to the official "save as PDF" extension:
1. produce a PDF with the smallest number of page breaks,
1. the original notebook is attached to the PDF; and
1. this extension does not require LaTex.

The created PDF will have as few pages as possible, in many cases only one. This is useful if you are exporting your notebook to a PDF for sharing with others who will view it on a screen.

To make it easier to reproduce the contents of the PDF at a later date the original notebook is attached to the PDF. Not all PDF viewers know how to deal with attachments. This mean you need to use Acrobat Reader or pdf.js to be able to get the attachment from the PDF. Preview for OSX does not know how to display/give you access to PDF attachments.


## Install

To use this bundler you need to install it:
```
python -m pip install notebook-as-pdf
pyppeteer-install
```
The second command will download and setup Chromium. It is used to perform
the HTML to PDF conversion.


## Use it

Create a notebook and the click "File -> Download As". Click the new menu entry
called "PDF via HTML". Your notebook will be converted to a PDF on the fly
and then downloaded.

You will have to use Acrobat Reader to see the attachment to your PDF. Preview
on OSX can not display PDF attachments.
