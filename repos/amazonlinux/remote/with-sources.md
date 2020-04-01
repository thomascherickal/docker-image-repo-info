## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:26c08e4d8fcf09bfad0c3c35f1608e8acfb07cbef8d5ac87c111ce10579d11d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:50c28a33157555b4372c1e98cd9c70c161e78e944683322bbfb2b8f44c7729ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.8 MB (476800172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c25bb04918e2ddc50ce74762ffbc0c89b25cd45ba721f2798a172c42234316c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Feb 2020 23:19:52 GMT
ADD file:c43f05fa78d78f998cd8e2e45f089e0572877490c7df425e514d44f15d958fad in / 
# Wed, 19 Feb 2020 23:19:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Feb 2020 23:20:16 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9d577ed8f0e2cbd076b6f144ec0c470c9c81012109b3d19515b8287114f96859.tar.gz"  && echo "88b2385d08e0f3df72a3d6b411c6b418af927ef411549cea48a3dfd887bf0f29  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a7583ef20c9db3e6539d4160e9914383701901b24979656a228000718b0d5bea`  
		Last Modified: Wed, 19 Feb 2020 23:20:55 GMT  
		Size: 61.7 MB (61669860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2696d5ea6c170fee8b13d7cc50cf08e8da5934fb7ebec062fbcd1db4171450be`  
		Last Modified: Wed, 19 Feb 2020 23:21:19 GMT  
		Size: 415.1 MB (415130312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:20b1a9fe34ca33f2c1aacc4343fa97b0771d30ca2205167addab44c976fd726c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478210702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e2dcdd719c4bfad05508a36c20f7d8100b941816a39367f4b3b4cedb6d39431`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 05:22:43 GMT
ADD file:40b8f329ad6d591029e1a4cde76c1d097315b136796d31bb9d3df35183423c14 in / 
# Wed, 01 Apr 2020 05:22:46 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 05:23:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-4cda1b0d98865d12f61886af2ff052cf2cb4a48734bded0ac84d2664a0361220.tar.gz"  && echo "c53ef45b008bcb392f9ecbd229a6fa38f69cfe536d630560a8e1a8daaa8b68e6  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:01d0a3bd5b98a6512409a10e5e5b065e87b794f924f3f9f7662939925aac631b`  
		Last Modified: Wed, 01 Apr 2020 05:24:01 GMT  
		Size: 63.1 MB (63072580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f5263e197d28b470047a0d5a85c7de9ceb69e2107bcc4eba8d080aef3bfa95`  
		Last Modified: Wed, 01 Apr 2020 05:24:46 GMT  
		Size: 415.1 MB (415138122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
