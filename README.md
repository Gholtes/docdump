
[![MIT License][license-shield]][license-url]
# DocDump
### A package to extract text from common document types

DocDump aims to allow for raw text data and document metadata to be easily extracted from a 
range of commonly used document types, such as Word, PDF, PowerPoint, Excel, txt. DocDump acts as 
a wrapper for a number of existing packages: `PyPDF2`, `openpyxl`, `python-docx`, `python-pptx`.

DocDump extracts all text as a single string, and does not preserve text structure. This makes
it a useful tool in a natural language processing or search pipeline.

DocDump does not perform any preprocessing or normalisation of the extracted text.
## Getting Started

DocDump requires Python 3.7+

### Installation

```bash
pip install docdump
```

### Usage

```python
from docdump import doc_reader

document = doc_reader("sampleFile.docx")

text_dump = document.text
metadata = document.metadata
filetype = document.filetype
absolute_path = document.path
```

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Grant Holtes - gwholtes@gmail.com

Project Link: [https://github.com/Gholtes/docdump](https://github.com/Gholtes/docdump)

[license-url]: https://github.com/Gholtes/docdump/blob/master/LICENSE.txt
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=flat-square