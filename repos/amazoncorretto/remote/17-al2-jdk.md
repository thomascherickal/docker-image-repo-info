## `amazoncorretto:17-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:7e6fe5702ac591f0ec9c69c582d6f177672249c7865061812f1d02ae9d55c43f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f9fd23a2fb9c78de9722bfd95e35dc7098f78493bc2a7cf33f160c3651994f57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214455645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:751302ba469679688ea5ac04d02c44a589aa98927961dc2f9650e586267a2bce`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 20 Jun 2023 22:20:15 GMT
COPY dir:129c77392b447afbaa234a34f434bed5ec790278efd165e1d59d4425216de49b in / 
# Tue, 20 Jun 2023 22:20:16 GMT
CMD ["/bin/bash"]
# Tue, 20 Jun 2023 22:55:38 GMT
ARG version=17.0.7.7-1
# Tue, 20 Jun 2023 22:56:03 GMT
# ARGS: version=17.0.7.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Jun 2023 22:56:04 GMT
ENV LANG=C.UTF-8
# Tue, 20 Jun 2023 22:56:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:0086aac11276884f299f6c13a98f93369cc50f7c0518989c2d4a29dd999feb70`  
		Last Modified: Fri, 16 Jun 2023 00:07:41 GMT  
		Size: 62.5 MB (62487611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63560138ab92e35f069c08d4c0c90d11daf6f7600a77676c4ae84382c0ca5e6`  
		Last Modified: Tue, 20 Jun 2023 23:01:52 GMT  
		Size: 152.0 MB (151968034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:a7856308ee11c2956b3e28f1f9e126d402d38d71e0a72f06d771e717f036d0ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.6 MB (214613732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1369ec8cc2fd85703a881d0a7a9559d611ae10c2f2d325f19c627bfaf62233f6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:39:41 GMT
COPY dir:51df2295aa01017be94f36c53673ecd4aa152aa99ad3c20338f5409440ff57f7 in / 
# Mon, 12 Jun 2023 19:39:42 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 19:57:51 GMT
ARG version=17.0.7.7-1
# Mon, 12 Jun 2023 19:58:10 GMT
# ARGS: version=17.0.7.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Jun 2023 19:58:11 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jun 2023 19:58:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:7943399bb3e529e35dfa651db084f8cbc0868d64a866e4cc4c88d2f0043943a8`  
		Last Modified: Wed, 07 Jun 2023 18:37:02 GMT  
		Size: 64.1 MB (64139660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646a9e09ff10513c3f197bdd57ba45acd9d119c8fd2abb9a7fe9c04f690c4dfa`  
		Last Modified: Mon, 12 Jun 2023 20:02:48 GMT  
		Size: 150.5 MB (150474072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
