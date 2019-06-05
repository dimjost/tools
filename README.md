# How to split a big file larget then 100 MB to commit to GitHub

	split -b 50M <archive-name>.tar.gz "parts-prefix"
	split -b 50M jdk-8u181-linux-x64.tar.gz "jdk-8u181-linux-x64"


# How to join splited files

	cat "parts-prefix"* > <archive-name>.tar.gz
	cat jdk-10.0.2_linux-x64* > jdk-10.0.2_linux-x64.tar.gz


