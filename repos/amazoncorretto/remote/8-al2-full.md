## `amazoncorretto:8-al2-full`

```console
$ docker pull amazoncorretto@sha256:a9c629bd52430dd465344442331280e31e0766710f56954f71df9ee0c42f9485
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:39cc5a8909e54ade3e44c2f6843d8202dc135877bcc53c968394791f26e1f5e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137800688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76e226e1441a4acbb69218f0030ceb99722a4889847b11429b51ff6e48676cf6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:19:57 GMT
ADD file:4eb88d9d977dadb40c630d693a07ca066069b30b9751b7a421dfb4ba0b99d862 in / 
# Thu, 21 Apr 2022 22:19:58 GMT
CMD ["/bin/bash"]
# Fri, 22 Apr 2022 01:15:33 GMT
ARG version=1.8.0_332.b08-1
# Fri, 22 Apr 2022 01:15:54 GMT
# ARGS: version=1.8.0_332.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 22 Apr 2022 01:15:54 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 01:15:54 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:ac1397dc8419bf1767b60a5cc5849b7130406030581d4542e48965801c303a70`  
		Last Modified: Thu, 21 Apr 2022 22:08:36 GMT  
		Size: 62.3 MB (62265199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a11637ae889799601bbbd711feecf5399cb26c4ae3a2fd22adcf7ed4950edb`  
		Last Modified: Fri, 22 Apr 2022 01:20:07 GMT  
		Size: 75.5 MB (75535489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e3b1888a3604fb0ccd8e68ce7802da9dc739fbe27ae67052c9dd26249950eeab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123483708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5977975e2e62da06d6cabffc63f6835f190f26f04c43e342c95101a3713b0f21`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:57:49 GMT
ADD file:76e1ee72575f50a75573a46483631e239d3b6afda9fdd53086883bd03db5364b in / 
# Thu, 21 Apr 2022 22:57:51 GMT
CMD ["/bin/bash"]
# Fri, 22 Apr 2022 02:35:19 GMT
ARG version=1.8.0_332.b08-1
# Fri, 22 Apr 2022 02:35:34 GMT
# ARGS: version=1.8.0_332.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 22 Apr 2022 02:35:34 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 02:35:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:86bcd0b49e3391c117b5e27756fdf585aadc1a7b9054d19af0faa050839a6633`  
		Last Modified: Thu, 21 Apr 2022 22:59:02 GMT  
		Size: 63.9 MB (63888157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc4795546ab74e3da82aba602b4bca21dd23b6c7323a9f1e763f11191a57642`  
		Last Modified: Fri, 22 Apr 2022 02:37:53 GMT  
		Size: 59.6 MB (59595551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
