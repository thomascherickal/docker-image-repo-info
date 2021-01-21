## `amazoncorretto:8-al2-full`

```console
$ docker pull amazoncorretto@sha256:0de32cab53565592434db5368a580060daa176f14daee0635f44524511560bf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:59c8903ef83ed1f10cd55047666a029088bff338c4ae972cfc40187f880d6a51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137284163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e72afafb4d20afe3d117fd70a544e8e97d0074185838573d16214da6c67dda0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:09 GMT
ADD file:15991ffbefc01e13f134972ce0eabc6b7901ea9ab4d56347bee5057302cf4848 in / 
# Wed, 23 Dec 2020 20:20:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 19:19:37 GMT
ARG version=1.8.0_282.b08-1
# Thu, 21 Jan 2021 19:19:51 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 21 Jan 2021 19:19:51 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 19:19:51 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:4232b9ee675bb1f9a32337ec3f266a570b75c54c3c3f173b1abb998e9984ad8c`  
		Last Modified: Wed, 23 Dec 2020 20:21:42 GMT  
		Size: 62.0 MB (62007428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638373d2fdada0614a24cd0be71916ad9ea4352fef0d34bdbad351b04607dbc3`  
		Last Modified: Thu, 21 Jan 2021 19:21:40 GMT  
		Size: 75.3 MB (75276735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:481d7d20235deae616ffe6c47d252710641c2ec206e60f03e9c852b7e052a208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123054872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d715113edd46309a55014ebe016e5deb142aefc371342c1afaf23af21d075edf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 19:39:59 GMT
ADD file:d991483ad4376be5e4327b3789511ab9266db8b87fc4b5327f0cabd1016ba00a in / 
# Wed, 23 Dec 2020 19:40:02 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 18:39:41 GMT
ARG version=1.8.0_282.b08-1
# Thu, 21 Jan 2021 18:40:14 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 21 Jan 2021 18:40:15 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 18:40:16 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:3307d2ab2034125075f0b058dcc32d6bf3e2c0595f1306de08d9e4a0287ddd76`  
		Last Modified: Wed, 23 Dec 2020 19:40:59 GMT  
		Size: 63.7 MB (63707914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb58219db59f1e5124e1253221af1a76e61b1327094d34728bc493a7b761bd0`  
		Last Modified: Thu, 21 Jan 2021 18:41:54 GMT  
		Size: 59.3 MB (59346958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
