Whow_UCCA
=========

Whow_UCCA is a corpus of English [WikiHow](https://wikihow.com) instructional guides semantically annotated with [Universal Conceptual Cognitive Annotation (UCCA)](http://www.cs.huji.ac.il/~oabend/ucca.html). It is comprised of 12 documents about varying topics, which also have been annotated with an array of linguistic (POS, syntax, discourse structure and more) and document-structure information as part of the [GUM](https://corpling.uis.georgetown.edu/gum/) project ([github](https://github.com/amir-zeldes/gum)).

The annotations were carried out by the students and instructor of the course Advanced Semantic Representations (LING/COSC-672) at Georgetown University in the Fall semester 2018.

---

Files and directories
---------------------

* ucca-guidelines.pdf: The version of the UCCA annotation guidelines used for the compilation of this corpus.
* unreviewed/xml: Annotated passages before review/adjudication.
* raw/txt: Passages in raw text format (tokenized).

Documents and passages
----------------------

The corpus contains 12 documents with token counts 656-1160. For comparability and to facilitate annotation, we split each document into 2-4 passages ranging between 104 and 355 tokens each. At least 2 passages / 607 tokens of each document have been annotated with UCCA by at least one annotator.
Files are named after the schema 

`whow_<DOCUMENT>_<PASSAGE>_<XXXX>.xml`.

So the file `whow_ballet_2_orig.xml`, for instance, contains the annotation for the 2nd passage of document "whow_ballet".

Multiple annotations per passage
--------------------------------

In order to compute inter-annotator agreement (IAA), one randomly selected passage per document has been annotated by two additional annotators. In the file naming schema described above, <XXXX> (one out of {orig, iaa1, iaa2}) indicates whether the annotation of this passage was done by the annotator originally assigned to it (primary annotator), or one of the secondary annotators.

---

Annotation Web-App
------------------

The annotations were carried out through the web-based annotation tool UCCAApp ([demo](http://ucca-demo.cs.huji.ac.il/)).


UCCA API
--------

UCCA Python API by Daniel Hershcovich and Amit Beka provides all you need to read, analyse, manipulate, and write the annotations provided in .xml format.
To get it, you can clone the following github repository:

`git clone https://github.com/danielhers/ucca.git`,

or install the package via pip:

`pip install ucca`.

---

References
----------

* [Universal Conceptual Cognitive Annotation (UCCA)](http://www.cs.huji.ac.il/~oabend/papers/ucca_acl.pdf)
  Omri Abend and Ari Rappoport (2013). ACL 2013.
* [UCCAApp: Web-application for Syntactic and Semantic Phrase-based Annotation](http://www.cs.huji.ac.il/~oabend/papers/ucca_app_demo_cameraready.pdf)
  Omri Abend, Shai Yerushalmi and Ari Rappoport (2017). ACL 2017.
* [The GUM Corpus: Creating Multilayer Resources in the Classroom](http://dx.doi.org/10.1007/s10579-016-9343-x)
  Amir Zeldes (2017). Language Resources and Evaluation 51(3), 581–612.
