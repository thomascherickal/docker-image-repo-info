## `maven:3-sapmachine-17`

```console
$ docker pull maven@sha256:b6177604f6ec93669dc73e25c9d4248b627def2770fdafb9892df45e9ecf5941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `maven:3-sapmachine-17` - linux; amd64

```console
$ docker pull maven@sha256:7961b7ee151bb20b73b82ebad0ef61796e533d6cab51f88151fe4dac26e9dd25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.0 MB (275049169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcedd87a7d3e27b2b4ae1eeb61520a84e1435b6e1128f72315bae7d874edb09`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:09:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:10:23 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.4.1     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:10:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Wed, 05 Oct 2022 18:10:25 GMT
CMD ["jshell"]
# Thu, 06 Oct 2022 03:05:39 GMT
RUN apt-get update     && apt-get install -y curl git     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 03:05:39 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 06 Oct 2022 03:05:39 GMT
ARG USER_HOME_DIR=/root
# Thu, 06 Oct 2022 03:05:40 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 06 Oct 2022 03:05:40 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 06 Oct 2022 03:05:41 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 06 Oct 2022 03:05:41 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 06 Oct 2022 03:05:41 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 06 Oct 2022 03:05:41 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 06 Oct 2022 03:05:42 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 06 Oct 2022 03:05:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 06 Oct 2022 03:05:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0b13da87099833442bbfa96ea98ecb8c17f08743ed487859d5091012fa27a9`  
		Last Modified: Wed, 05 Oct 2022 18:11:18 GMT  
		Size: 7.9 MB (7920113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b09c52e9c3c0090d0a17bb00c88daf0b5ff8c10d40087dd5f1fd895bd349a`  
		Last Modified: Wed, 05 Oct 2022 18:11:56 GMT  
		Size: 197.8 MB (197764237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90678f52dbdd74e8d40fe85692e6e350fbecbd380e80458340a6ccedfaf5bfb6`  
		Last Modified: Thu, 06 Oct 2022 03:11:38 GMT  
		Size: 32.0 MB (32049653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa49b6aed07f141206c41964f4fb80c9efc6c81104e804c34e205d6f178ce94`  
		Last Modified: Thu, 06 Oct 2022 03:11:34 GMT  
		Size: 8.7 MB (8739503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ed915299e34ad04303874c8216296772a1040536411ed96515a647ecec1a5c`  
		Last Modified: Thu, 06 Oct 2022 03:11:33 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f461b37729f3970e2fe322ccaa2d03306356bb61375b5e97845ccb1497a6396`  
		Last Modified: Thu, 06 Oct 2022 03:11:33 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
