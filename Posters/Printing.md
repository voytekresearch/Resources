# Printing a Poster at UCSD

UCSD ACMS services offers cheap and pretty quick poster printing, which is usually the preferred option to print a poster.

## Print From a UCSD Computer Lab (more reliable)

Log into remote printing
https://sdacs.ucsd.edu/accttools-cgi-bin/rpauth.cgi

Open pdf in adobe and print
Instructions: https://acms.ucsd.edu/services/printing/posters/win-pdf.html

Choose HP Designjet T1100ps
Actual size
Properties>advanced
Papersize > postscript custop page size > 42 x 60 or whatever
Truetype fotn: download as softfont

Check print np
http://ieng9.ucsd.edu/~lp/cplot1_np42/?C=M;O=D

Note: When attempting to check print result using no-print, the np printer has to match the width you want (np or np42 for 42-inch wide), otherwise it gives you the wrong estimate and the preview looks cut off

Check jobs in queue
http://cplot.ucsd.edu/lp-cgi-bin/checkqueue.cgi

## Print from Local Computer (only works sometimes)

Before you can print a poster from your laptop, you must install the necessary drivers, instructions are here: https://acms.ucsd.edu/students/print/remoteprint.html and here: https://acms.ucsd.edu/services/printing/posters/win-driver.html

If that does not work, use a lab computer in the basement of the Applied Math building (follow instructions above).

If it does, continue here:

Then you can print a pdf by following the instructions here:
(Windows) https://acms.ucsd.edu/services/printing/posters/win-pdf.html
(Mac) https://acms.ucsd.edu/services/printing/posters/osx-pdf.html

In step one, you will need to log into the remote printing authorization here: https://sdacs.ucsd.edu/accttools-cgi-bin/rpauth.cgi using the
It is useful to first try printing to the \_np (no print) printers and checking the output here: http://ieng9.ucsd.edu/~lp/cplot1_np42/?C=M;O=D  to make sure that everything looks right

In the past we’ve had to convert key → png → pdf to get it to print correctly

The login will be something like ‘cg42sc’ and the pw is in an email you received

If you don’t have a login, then Brad needs to email ACMS, as described here: http://acms.ucsd.edu/info/recharge.html

Once you are logged in, you open up the pdf in Adobe Reader and make sure you print ‘actual size’, the orientation is ‘auto’, and you change the paper size to match your needs

After you click ‘print’, the poster should show up in the queue here: https://acms.ucsd.edu/info/cplotqueue.html and you will get an email when it starts printing and finishes printing
