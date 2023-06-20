## `amazoncorretto:20-al2-full`

```console
$ docker pull amazoncorretto@sha256:3b228d754e35d672aa63a1402116732598c7f2c669dd0b76c3ea101ba3f9df3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:62a06b483db4c7a7d4d1fc37843fc12d6681d2af147b1cdd88ac957e1e7870ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.3 MB (223250837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b766ed728338578bd5539a307af2450f7d3465dce3aac7fdf0a0a56d811fbd7c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 20 Jun 2023 22:20:15 GMT
COPY dir:129c77392b447afbaa234a34f434bed5ec790278efd165e1d59d4425216de49b in / 
# Tue, 20 Jun 2023 22:20:16 GMT
CMD ["/bin/bash"]
# Tue, 20 Jun 2023 22:57:14 GMT
ARG version=20.0.1.9-1
# Tue, 20 Jun 2023 22:57:37 GMT
# ARGS: version=20.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Jun 2023 22:57:38 GMT
ENV LANG=C.UTF-8
# Tue, 20 Jun 2023 22:57:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:0086aac11276884f299f6c13a98f93369cc50f7c0518989c2d4a29dd999feb70`  
		Last Modified: Fri, 16 Jun 2023 00:07:41 GMT  
		Size: 62.5 MB (62487611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a67431843d9e5854a588042bb3ab1dea757eb095a929ea60bef489fc4f13e9`  
		Last Modified: Tue, 20 Jun 2023 23:03:25 GMT  
		Size: 160.8 MB (160763226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-al2-full` - linux; arm64 variant v8

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
