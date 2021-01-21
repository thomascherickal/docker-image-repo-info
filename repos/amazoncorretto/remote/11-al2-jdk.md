## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:2761a3509de723a1da1b168ae3ed4214a92c0c2a97bab39f2b107910c7cecd93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:0887fe50a08a79e3a49905496bdc4e4e0ff3a7e46780fd2523baeb7c634b5d80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.5 MB (208538271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:702fddf65318b8961e6d70c184dc9b2420bc7c6c901ed131f096ed5af9e539da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:09 GMT
ADD file:15991ffbefc01e13f134972ce0eabc6b7901ea9ab4d56347bee5057302cf4848 in / 
# Wed, 23 Dec 2020 20:20:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 19:19:56 GMT
ARG version=11.0.10.9-1
# Thu, 21 Jan 2021 19:20:12 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 21 Jan 2021 19:20:12 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 19:20:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:4232b9ee675bb1f9a32337ec3f266a570b75c54c3c3f173b1abb998e9984ad8c`  
		Last Modified: Wed, 23 Dec 2020 20:21:42 GMT  
		Size: 62.0 MB (62007428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132220740555f6a23e53b52a8be783f695ea89bc701d7aa6eefe5cc9abc31df3`  
		Last Modified: Thu, 21 Jan 2021 19:22:07 GMT  
		Size: 146.5 MB (146530843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9d953f0f482d5e71af840bf8428b842de0c4a12942fc809aa4eab8eb09e47eda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.3 MB (208296245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cd067172ee4dd75c541ab606da819a7af951b749a414e5426c0000f8c0da199`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 19:39:59 GMT
ADD file:d991483ad4376be5e4327b3789511ab9266db8b87fc4b5327f0cabd1016ba00a in / 
# Wed, 23 Dec 2020 19:40:02 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 18:40:26 GMT
ARG version=11.0.10.9-1
# Thu, 21 Jan 2021 18:40:55 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 21 Jan 2021 18:40:57 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 18:40:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:3307d2ab2034125075f0b058dcc32d6bf3e2c0595f1306de08d9e4a0287ddd76`  
		Last Modified: Wed, 23 Dec 2020 19:40:59 GMT  
		Size: 63.7 MB (63707914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03d2b79d43eb79a680e95539063ef30a4e64bb5d44c8ae1f6984f8876a4a8cc`  
		Last Modified: Thu, 21 Jan 2021 18:42:35 GMT  
		Size: 144.6 MB (144588331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
