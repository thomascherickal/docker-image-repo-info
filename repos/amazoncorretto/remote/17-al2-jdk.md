## `amazoncorretto:17-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:cf9b59c76cef9fc617bbcb5566e362c753fa73d5408c6e35d332d175c06a07a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:76cbed8853400663efaa608ce4a2e08815aa6b0740f845eee4a13cef200ad637
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.9 MB (213937478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3ba926ccdaa37a945dab014c4feb9051726e55ee68a7e418ca9f75c811ec98`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:19:41 GMT
ADD file:e6c6bb016423b24a28b273cc76e9fbbf81934b77a0ede797ccfd0eeac465c8a4 in / 
# Tue, 21 Jun 2022 23:19:42 GMT
CMD ["/bin/bash"]
# Tue, 19 Jul 2022 22:38:35 GMT
ARG version=17.0.4.8-1
# Tue, 19 Jul 2022 22:38:58 GMT
# ARGS: version=17.0.4.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 19 Jul 2022 22:38:58 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:38:58 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:017c82d6391f0bf122516eac436a6e8d77ac13282fdd13dde7e7e47dc71d447e`  
		Last Modified: Wed, 15 Jun 2022 22:09:36 GMT  
		Size: 62.3 MB (62294977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c297b4544f77e61a5ef202b51c7b35066efeb505d0980b8fb71af85f3a0cfb4`  
		Last Modified: Tue, 19 Jul 2022 22:46:36 GMT  
		Size: 151.6 MB (151642501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:f5dc9056a4087c1d2b878bb0d9d236a3390a0645903d0d0846ec85f1b1fd96a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.2 MB (214192612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7fc5f92a6f23afc9b55beac6b1e43c20fbc1704dc6d64a36351a3e56098a643`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
# Wed, 22 Jun 2022 01:02:23 GMT
ARG version=17.0.3.6-1
# Wed, 22 Jun 2022 01:02:38 GMT
# ARGS: version=17.0.3.6-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 22 Jun 2022 01:02:39 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jun 2022 01:02:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac67b8ab407fc666ca5cb18f894cf94d55c9a97db687078134113b9fa620ab75`  
		Last Modified: Wed, 22 Jun 2022 01:05:06 GMT  
		Size: 150.3 MB (150273970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
