## `amazoncorretto:17-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:151c795fd72fc4e5b9a28f919c0715e6a636682e4f6213d1c55896a6ca2b8d03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6e89f81fc1aa2d45cd6d3a6256b75e7467f4c10dd47a741b35601dadfa889ea5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.9 MB (213945704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6159c9aeafe692639af5a614081f0e4351282e6da49772c9ea687a298846a576`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:19:57 GMT
ADD file:4eb88d9d977dadb40c630d693a07ca066069b30b9751b7a421dfb4ba0b99d862 in / 
# Thu, 21 Apr 2022 22:19:58 GMT
CMD ["/bin/bash"]
# Fri, 22 Apr 2022 01:16:52 GMT
ARG version=17.0.3.6-1
# Fri, 22 Apr 2022 01:17:19 GMT
# ARGS: version=17.0.3.6-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 22 Apr 2022 01:17:19 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 01:17:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:ac1397dc8419bf1767b60a5cc5849b7130406030581d4542e48965801c303a70`  
		Last Modified: Thu, 21 Apr 2022 22:08:36 GMT  
		Size: 62.3 MB (62265199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf7ca9cf92ccf91b6fdf53584ee5def54541ef36351c78396c2b41750f87117`  
		Last Modified: Fri, 22 Apr 2022 01:21:27 GMT  
		Size: 151.7 MB (151680505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d84fc1a70065913233c9316ea4bc3b636bbcdf17bf247d768836fec44dc42a0e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.2 MB (214171282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ca340235bc7ba3e14f7e2cb570d9b87d32341fd7c12cbfcec05504cc3bf64f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:57:49 GMT
ADD file:76e1ee72575f50a75573a46483631e239d3b6afda9fdd53086883bd03db5364b in / 
# Thu, 21 Apr 2022 22:57:51 GMT
CMD ["/bin/bash"]
# Fri, 22 Apr 2022 02:36:14 GMT
ARG version=17.0.3.6-1
# Fri, 22 Apr 2022 02:36:34 GMT
# ARGS: version=17.0.3.6-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 22 Apr 2022 02:36:35 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 02:36:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:86bcd0b49e3391c117b5e27756fdf585aadc1a7b9054d19af0faa050839a6633`  
		Last Modified: Thu, 21 Apr 2022 22:59:02 GMT  
		Size: 63.9 MB (63888157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2619635dcee07409b401931bb71ef9647d40094f623b2db2769a24d066190d0`  
		Last Modified: Fri, 22 Apr 2022 02:39:02 GMT  
		Size: 150.3 MB (150283125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
