## `photon:latest`

```console
$ docker pull photon@sha256:9405cf4dba128f2f1659f5b46a4cfbc8e4849938e1398e5dec9f07ad0c23c365
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:370f0c6ffa232c2809eb3f7060cb0c9ace11c7b94dd69dee6f458c3fdb2e7723
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15777820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b522614211e9ca4c7a27bdfc7e8e79aaa5b476b3b2e69ad236b5740919cf7e06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Jun 2021 17:27:47 GMT
ADD file:6a5dab57aa13fd82100b17d6232dec9261ccf91af6df61a73173ed759e16fc3f in / 
# Tue, 01 Jun 2021 17:27:47 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20210528
# Tue, 01 Jun 2021 17:27:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1e47377d8a0eaf0bf6e2365ebfef3e5ab30da3b7fdd0e7574a8b65a0ade47109`  
		Last Modified: Tue, 01 Jun 2021 17:28:37 GMT  
		Size: 15.8 MB (15777820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:be3305419f87c3906c52c768f189642f1bbc1ea29820a114227a780e167f4db7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14811614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b4b554bdacd727f5fd3ae3bd36941f27779ee5814251b86e841189a613ce09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Jun 2021 17:51:23 GMT
ADD file:564aedc8c2b63162a87dc1077419c60ba1d2e112879aafca58dae55a8f2368eb in / 
# Tue, 01 Jun 2021 17:51:23 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20210528
# Tue, 01 Jun 2021 17:51:23 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7411be4436a42639f1f62ff752bcc56d5ef61dc848e812b53ddc84698c0641c0`  
		Last Modified: Tue, 01 Jun 2021 17:51:52 GMT  
		Size: 14.8 MB (14811614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
