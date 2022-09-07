## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:c4e634a38404c34ac9f4b284bb68641df5c67ea6ff176f9022b06ceef2274a0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:71644fe2ef5416f8ceabf402da7c4174fe750599076e106d9e9e6a4f89f52892
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392646533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50ceb4a4a8fb4917a472d3255b0b9f526a6523ad4a66219e31d1aa9ad902bebc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:19:43 GMT
ADD file:5019265631ee9bf27ce7360e76e53ca31276f85743f8f89ebbae0db6682520d9 in / 
# Wed, 07 Sep 2022 19:19:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Sep 2022 19:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-398599ffb8d0f6fb08e1b8d66966668452019fb99181907d93c4c560edce242b.tar.gz"     && echo "9045a697728eafb7c14d20a4170b7906c2f813b55a5bb32635f1963318df140c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c011f68cda3c0b264e794a7a2ed6621c014d944eab2c3c47bb1260e0279aae63`  
		Last Modified: Sat, 03 Sep 2022 04:05:43 GMT  
		Size: 57.8 MB (57840745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774b64e073109e8601db92af4778785b74981d0a66bb35ed640af8a8425ce28e`  
		Last Modified: Wed, 07 Sep 2022 19:21:07 GMT  
		Size: 334.8 MB (334805788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:53c32bc4a8fea84710fbfe1933b1b84db108eb76ee3c20b3b673e6bf9e331ba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.5 MB (391452945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e68a8cd162c06fc4c4bc68291eb191aadd029d78a8e0dec6b8652231c5775f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Sep 2022 19:39:40 GMT
ADD file:14de8dca6a69b386ae8bed6870c1e376b67ce8e35574747f3faea9cf143bca6e in / 
# Wed, 07 Sep 2022 19:39:41 GMT
CMD ["/bin/bash"]
# Wed, 07 Sep 2022 19:40:00 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-398599ffb8d0f6fb08e1b8d66966668452019fb99181907d93c4c560edce242b.tar.gz"     && echo "9045a697728eafb7c14d20a4170b7906c2f813b55a5bb32635f1963318df140c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:00ee01a8a4f0d3d97470c0d349a8ee4b534ef5a20a1c1abec5e0697493d8c08d`  
		Last Modified: Wed, 07 Sep 2022 19:40:41 GMT  
		Size: 56.6 MB (56647188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b245692459684d75b294e1d16f2407220fe53f4ae799e5a91d34fe73061cd`  
		Last Modified: Wed, 07 Sep 2022 19:41:38 GMT  
		Size: 334.8 MB (334805757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
