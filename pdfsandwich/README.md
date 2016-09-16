# build
docker build -t pdfsandwich .

# usage
docker run -v /some_path_containing_pdfs:/data pdfsandwich /data/this_doc_has_no_ocr.pdf
