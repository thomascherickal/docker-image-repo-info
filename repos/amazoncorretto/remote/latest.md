## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:32b77b51e2376783c7462e7e2be3ee7dd462eab2a812503e55000d32e7188e73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3ec35b5b986a2b1a19cdc3dc504ae77a4a2d81cf0a871bb6ea8265e12f4acfb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138039085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e2d3d1065e3e23a2508836bab9fa76ce10c7c1ff11960919cb9cde82ff9eb3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 20 Jun 2023 22:20:15 GMT
COPY dir:129c77392b447afbaa234a34f434bed5ec790278efd165e1d59d4425216de49b in / 
# Tue, 20 Jun 2023 22:20:16 GMT
CMD ["/bin/bash"]
# Tue, 20 Jun 2023 22:52:35 GMT
ARG version=1.8.0_372.b07-1
# Tue, 20 Jun 2023 22:52:56 GMT
# ARGS: version=1.8.0_372.b07-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 20 Jun 2023 22:52:57 GMT
ENV LANG=C.UTF-8
# Tue, 20 Jun 2023 22:52:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:0086aac11276884f299f6c13a98f93369cc50f7c0518989c2d4a29dd999feb70`  
		Last Modified: Fri, 16 Jun 2023 00:07:41 GMT  
		Size: 62.5 MB (62487611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55da7f32caedeb9b4242fec7746bd814425912c9d0cdb7a32b853b91de5bd1fa`  
		Last Modified: Tue, 20 Jun 2023 22:58:57 GMT  
		Size: 75.6 MB (75551474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:3aa364d4b5eb06e76fcd174d18cc07f036c3069ca251f2a115ed15cb04402b99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123711448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39594af0373883a2cc96b79a957bb00e058111a34cd3dcde722760b5f0470fcd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:39:41 GMT
COPY dir:51df2295aa01017be94f36c53673ecd4aa152aa99ad3c20338f5409440ff57f7 in / 
# Mon, 12 Jun 2023 19:39:42 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 19:55:31 GMT
ARG version=1.8.0_372.b07-1
# Mon, 12 Jun 2023 19:55:48 GMT
# ARGS: version=1.8.0_372.b07-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Jun 2023 19:55:49 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jun 2023 19:55:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:7943399bb3e529e35dfa651db084f8cbc0868d64a866e4cc4c88d2f0043943a8`  
		Last Modified: Wed, 07 Jun 2023 18:37:02 GMT  
		Size: 64.1 MB (64139660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cdb010d403a63e0b0e10671dbcd3572181bd263d55bc103b2550947fcd0765`  
		Last Modified: Mon, 12 Jun 2023 20:00:39 GMT  
		Size: 59.6 MB (59571788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
