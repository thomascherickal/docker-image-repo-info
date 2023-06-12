## `amazoncorretto:20-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:64e3b9429922e13a3f92d80e98f09ba5165f147f508c129796a492eb8eac2a9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:0046bd9d51d5c18087a6afa06afdb73b8f24e605feef3e51e54971cc95392d39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.3 MB (223256793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff735a29168a2da83dab5dbb1e955d1f815831d83e0e7b8f19edc6f8ec7aa31`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:20:12 GMT
COPY dir:fcef1a58ca6f7120ef8bf5af7158a168707c721bb2ebb75f4483ac8ec6174c3f in / 
# Mon, 12 Jun 2023 19:20:13 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 19:41:51 GMT
ARG version=20.0.1.9-1
# Mon, 12 Jun 2023 19:42:18 GMT
# ARGS: version=20.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Jun 2023 19:42:18 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jun 2023 19:42:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:8c8d630364ddfad51ca27951f43586450b97e006740d3139ac1c7fc1fa1a48ab`  
		Last Modified: Wed, 07 Jun 2023 18:46:43 GMT  
		Size: 62.5 MB (62493283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f4ed3d4d0eb7d73c0959e9ffc09d21d9096ba38bd73921c68ed7745cd383c6`  
		Last Modified: Mon, 12 Jun 2023 19:47:31 GMT  
		Size: 160.8 MB (160763510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0bc53809922fd3d19a3042ee87b58e9b08dd36a4fd29a7400913c303edfe0f1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.9 MB (222925343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:291d8f9ea4a96010a1bf11549deaa9e0dd37415e6a10c13f4856111cc4e2a4c6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:39:41 GMT
COPY dir:51df2295aa01017be94f36c53673ecd4aa152aa99ad3c20338f5409440ff57f7 in / 
# Mon, 12 Jun 2023 19:39:42 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 19:59:11 GMT
ARG version=20.0.1.9-1
# Mon, 12 Jun 2023 19:59:33 GMT
# ARGS: version=20.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Jun 2023 19:59:35 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jun 2023 19:59:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:7943399bb3e529e35dfa651db084f8cbc0868d64a866e4cc4c88d2f0043943a8`  
		Last Modified: Wed, 07 Jun 2023 18:37:02 GMT  
		Size: 64.1 MB (64139660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371c45046361446db5da0f6ce4e2e9d5ed459efdb264a7c4ee89145a89c33456`  
		Last Modified: Mon, 12 Jun 2023 20:04:09 GMT  
		Size: 158.8 MB (158785683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
