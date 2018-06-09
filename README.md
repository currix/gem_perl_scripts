Perl scripts and auxiliary files used in the organization of a
Scientific meeting.

by Currix TM

Apps: make_tags and make_certificates

(1) make_tags

Prepare from a csv file with the following syntax:

name:surname:affiliation:country

a LaTeX file with the tags for the meeting attendees.  The resulting
LaTeX file should be compiled with pdflatex.

Auxiliary files:

test_tags.csv          csv example file
background_color.xcf   gimp file for tag background
part_background.png    png file for tag background

Examples:

make_tags -h

make_tags -o testing_tags.tex -b part_background.png test_tags.csv 

                -----------------------------------
		
(2) make_certificates 

Prepare from a csv file with the following syntax:

name:surname:payment:grant:seminar title:poster title

a LaTeX file with the certificates for the meeting attendees. If any
of the field does not apply the entry should be "NO". The resulting
LaTeX file should be compiled with pdflatex.

Auxiliary files:

test_certs.csv                           csv example file
rabida_2018_certificate_background.xcf   gimp file for certificate background
rabida_2018_certificate_background.png   png file for certificate background

Examples:

make_certificates -h

make_certificates -o testing_certificates.tex -b rabida_2018_certificate_background.png test_certs.csv 

Licenses: See LICENSE file.
