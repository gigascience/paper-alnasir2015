# paper-alnasir2015

Source files from Al-Nasir and Shanahan, (2015) Investigation into the 
annotation of protocol sequencing steps in the Sequence Read Archive.

DOI:10.5524/100142


Acquiring the Bioconductor SRAdb and the Timestamp
--------------------------------------------------

The Bioconductor SRAdb.sqlite database used in the publication had
a timestamp of [2013-12-03 08:29:26] and is available from:

http://doi.org/10.5524/100142

The latest version can be downloaded from the Bioconductor consortium's SRAdb 
page:

http://www.bioconductor.org/packages/release/bioc/html/SRAdb.html


Timestamp of the Bioconductor SQLite database can be obtained from the
database using the following SQL:

	$> sqlite3 SRAmetadb.sqlite [to load the database]
	sqlite> Select * from metaInfo;
	

The SQL master scripts can be run using the following command, the
individual scripts they contain can also be copied/pasted:

	$> sqlite3 SRAmetadb.sqlite < scriptname.txt


SQL Script files - description
------------------------------

SQL-SRA-QRY-all-field-anno-check.txt
SQL-SRA-QRY-anno-counts.txt
SQL-SRA-QRY-anno-distribution2.txt
SQL-SRA-QRY-anno-distribution.txt
SQL-SRA-QRY-anno-proportions.txt
SQL-SRA-QRY-cross-check.txt
SQL-SRA-QRY-date-checks.txt
SQL-SRA-QRY-lib-cons-prot-venn.txt
SQL-SRA-QRY-null.txt
SQL-SRA-QRY-reagent-kits.txt
SQL-SRA-QRY-submission-joined-anno-report.txt
SQL-SRA-QRY-submission-joined-count.txt
SQL-SRA-QRY-submission-joined-unannotated-count.txt
SQL-SRA-QRY-unjoined-anno-counts-by-type.txt
SQL-SRA-QRY-url-only-lib-cons-prot.txt
SQL-SRA-QRY-url.txt
SQL-SRA-QRY-wordlists_study-joined-by-year.txt
SQL-SRA-QRY-wordlists_study-joined-lib-cons-prot.txt
SQL-SRA-QRY-wordlists_submission-joined-lib-cons-prot.txt
SQL-SRA-QRY-wordlists_submission-joined.txt
SQL-SRA-QRY-wordlists-unjoined.txt
SQL-SRA-to-Graph.txt

Other files
-----------

Diagram-ALL-FIELDS-Check-annotation.jpg - 
Diagram-SRA-Study-Experiment-Joined-probing.jpg - 


Additional documentation
------------------------

Additional documentation on the SRA can be found at 
http://www.ncbi.nlm.nih.gov/books/NBK47528/
http://www.ebi.ac.uk/ena/submit/read-submission
http://trace.ddbj.nig.ac.jp/dra/submission_e.html
