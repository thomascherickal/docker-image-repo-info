## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:c7b999c4dafbef559f121d77f919a775db13ddcea68a31d846b4d3e9ef317469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2fb367b85dcc2797239921217f62d98c66b4e614609ae8130d85ea12fa2be3cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.1 MB (489146951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8572b53c2976082cbb5f61cdd5677e4d8f173f835f7f46f692f85743b824f0c1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 22:06:49 GMT
ADD file:0e00ccd2daf7fcbf2c4b6c87fc4c7426cb4744220d4688380b712b0a10b1ce17 in / 
# Wed, 30 Mar 2022 22:06:49 GMT
CMD ["/bin/bash"]
# Wed, 30 Mar 2022 22:07:13 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-feddddadaa0ca95e9807903d234b2e9192782e81abe4ae95c969d9acf5d1a223.tar.gz"  && echo "a2450fe78ed3b89a144721743a282fcb5041783247ae040872007c08d36a83e1  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:51621d34d545ca53a75f5f765d89feed132eed23e837845dab564cd60d3c4a8d`  
		Last Modified: Wed, 30 Mar 2022 22:07:49 GMT  
		Size: 70.6 MB (70551902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4592a6a3eb2786610fec5f2359858c714b4968d2e854cde2a0adedbc33b2cf`  
		Last Modified: Wed, 30 Mar 2022 22:08:17 GMT  
		Size: 418.6 MB (418595049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:e2dd86254b03868c5c0566669f828081a230149217b93dedce7902ae792d910f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.7 MB (487701029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15709e43976d58175cbdcb7b62bb8d5a6a1b1618c7ba82580e570e92909e68`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 30 Mar 2022 18:25:19 GMT
ADD file:b4343bb7616f343b9a7343c7512a69010bd7f36e2c2e218e0eea2f57382746cf in / 
# Wed, 30 Mar 2022 18:25:20 GMT
CMD ["/bin/bash"]
# Wed, 30 Mar 2022 18:26:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-feddddadaa0ca95e9807903d234b2e9192782e81abe4ae95c969d9acf5d1a223.tar.gz"  && echo "a2450fe78ed3b89a144721743a282fcb5041783247ae040872007c08d36a83e1  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:1539c116c8b0d4e18a17732583c333362ac930b6eb4be2833fff8a8ab2ea6b8b`  
		Last Modified: Wed, 30 Mar 2022 18:26:53 GMT  
		Size: 69.1 MB (69106021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51ff1c75bc99c531f890a7b86060bf09ced222193f634e9f1b029ae55afb22c`  
		Last Modified: Wed, 30 Mar 2022 18:27:28 GMT  
		Size: 418.6 MB (418595008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
