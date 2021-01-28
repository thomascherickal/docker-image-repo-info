## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:879bca18882f3883edafbdb9c599649b16ee8c69379f0ad4da488246b694476b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:983d3e4de81b1c27d66e23dcaa8a16c475d5c5b495aa385604ccb648a8058788
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542850367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e352e313d08efc3970e6993a06e67920b041e2e9e87622b5a62639aee5437d5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 27 Jan 2021 22:19:43 GMT
ADD file:bcd0b903093ee2c81a54e8bdc50176f4038662ab936aa0d94af08458d508aef6 in / 
# Wed, 27 Jan 2021 22:19:43 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 22:20:10 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-020afd68ea87fb6a4b381a6874ce0c38c6f291f66d9f9d9fda853a9bc76a954d.tar.gz"  && echo "c74f4742eb862e351271e7bceff838061332d4bba919f1944568ed779351fceb  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:62350c28fdb7b7cbd0e199dd893555ed129ed85da482d882b1eeb574988ea7d6`  
		Last Modified: Wed, 27 Jan 2021 22:21:18 GMT  
		Size: 62.0 MB (61996576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332009c39171868832b64d8784eba0fb853d50be1faf582791d991cf57a9210f`  
		Last Modified: Wed, 27 Jan 2021 22:21:53 GMT  
		Size: 480.9 MB (480853791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6cacbd9b077f697758550c31d4829614d38c59dab987c48610cb0bd58ced5964
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.6 MB (544558555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3740fa68c45d8fd254232c13f0a2c86625d1d5d968d09da972db089b71d3da32`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 27 Jan 2021 23:09:56 GMT
ADD file:7f69686262e0e0e5415d42ac0371f7d0df0330bc4f0556e5d4b73dd78ceb1197 in / 
# Wed, 27 Jan 2021 23:10:02 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 23:10:37 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-020afd68ea87fb6a4b381a6874ce0c38c6f291f66d9f9d9fda853a9bc76a954d.tar.gz"  && echo "c74f4742eb862e351271e7bceff838061332d4bba919f1944568ed779351fceb  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c6741bcf27a42820ff66e35cc842cec9a845e9e9dba4ff7bd465fc6161442a86`  
		Last Modified: Wed, 27 Jan 2021 23:11:10 GMT  
		Size: 63.7 MB (63704713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaab9e837cfac0090182588950e8eb89d67acc59cd011bdd2b5bd9e9d5f0c801`  
		Last Modified: Wed, 27 Jan 2021 23:11:56 GMT  
		Size: 480.9 MB (480853842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
