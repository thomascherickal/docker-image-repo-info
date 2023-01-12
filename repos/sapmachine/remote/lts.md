## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:6578d7b6f2523c430a3baa2c1d85a5ed3a85032342745121841d6d75b873afce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:a3db9b76311a92ce5e404e46607a74dcea0154fe002ba2bd0d8aadcf700dd7c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234527597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe1eff4ffa2d79172bb29b776742a67f0b0b423bab7e330069230954d8580595`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 06:08:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:38 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:09:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Fri, 09 Dec 2022 06:09:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f9829f76f3bad367d27d5bf3e91e6bc0f738874c547c1b6c35ea445acb9f11`  
		Last Modified: Fri, 09 Dec 2022 06:10:29 GMT  
		Size: 7.9 MB (7912181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f782630874769148332fc6cb09cc233f9d28d10d82349f85f85cd9a5e50b80`  
		Last Modified: Fri, 09 Dec 2022 06:11:06 GMT  
		Size: 198.0 MB (198038534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `sapmachine:lts` - linux; arm64 variant v8

```console
$ docker pull sapmachine@sha256:30fb409334891779b0124a31467408aae466f9c8f860c3819a2c72d547b2c3cc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (231004756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c247c806137e8c5825cc1f5e0dab5514a744c3751506fde3ec213ff9fd1d9b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 23:47:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:56 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.5     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 23:48:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Wed, 11 Jan 2023 23:48:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c00c408cc2d94c0e75087f6aa9151688fe5b2714a5acb9a30aaf9ec603b385e`  
		Last Modified: Wed, 11 Jan 2023 23:49:41 GMT  
		Size: 7.8 MB (7754081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a4503e73ad3dbedceded998c6b620c463f436b0f7dce14fc97e80175cb8ccb`  
		Last Modified: Wed, 11 Jan 2023 23:50:14 GMT  
		Size: 196.1 MB (196057507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
