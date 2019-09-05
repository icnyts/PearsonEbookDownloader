# This utility downloads an entire Pearson E-Book in a PDF format for a better viewing experience

The need for this utility came out of regularly wanting to read the E-Book for my Physics textbook
in places where I would have little to no internet, or where the internet would cut out randomly.

Not to mention that the E-Book sometimes doesn't even load, leading to an inability to even use the book in the first place!

# Using this utility

To use this utility, first log into the pearson website and access the E-Book. After about 10 seconds (or once the eText is loaded), copy the bookID parameter (anywhere from 5-6 digits long) and download it either using using the online downloader ("index.html" in this repository, and also available at https://NoMod-Programming.github.io/PearsonEbookDownloader/) or manually using python.

To use the python version, run this utility as follows:

	python3 downloader.py <bookid>

Where python3 points to the location of a python interpreter with the PyPDF2 module available (`pip install pypdf2`).

This will take a few minutes, downloading each individual page of the PDF (thanks, Pearson, for using *individual* pdf files for each page a thousand page book!) to a temporary directory, then merging them into a final PDF.

The output pdf will be saved into the current directory as `out.pdf`

Also... Please don't use this for piracy. I paid for my online textbook, as should you, but I paid for a working textbook, not something that takes a minute to load each page of. While I can't stop you, please only use this utility if you have paid for the textbook.
