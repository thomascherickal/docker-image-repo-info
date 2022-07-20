## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:792b7c50398519ec4411dfef70038d402a668f3108b0ef47eb8e927378e071db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:9ceb039b9df62cb366ee4a1e5e64e88ac7b3f15f9bbe84ddbe38849d518b20d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137858529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8f21f9dfa65907c6bc93b64ead3a2315c052a65c4fb74deb023e85f0332c2c1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:19:41 GMT
ADD file:e6c6bb016423b24a28b273cc76e9fbbf81934b77a0ede797ccfd0eeac465c8a4 in / 
# Tue, 21 Jun 2022 23:19:42 GMT
CMD ["/bin/bash"]
# Tue, 19 Jul 2022 22:36:33 GMT
ARG version=1.8.0_342.b07-1
# Tue, 19 Jul 2022 22:36:54 GMT
# ARGS: version=1.8.0_342.b07-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 19 Jul 2022 22:36:54 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:36:54 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:017c82d6391f0bf122516eac436a6e8d77ac13282fdd13dde7e7e47dc71d447e`  
		Last Modified: Wed, 15 Jun 2022 22:09:36 GMT  
		Size: 62.3 MB (62294977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd37f0436307adbc991266c16ac0946094a406db7dfe6c1a0d7765554f698e3`  
		Last Modified: Tue, 19 Jul 2022 22:41:57 GMT  
		Size: 75.6 MB (75563552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:f340835eb6358a789db16b54a58c24dd85d217e1226f3f7215c839661cf039bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123522114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6d359d6ad207ea12926b604d0bdc1f273831069ea9d3dd2c74d1012fab7b8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
# Wed, 20 Jul 2022 06:00:43 GMT
ARG version=1.8.0_342.b07-1
# Wed, 20 Jul 2022 06:00:58 GMT
# ARGS: version=1.8.0_342.b07-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 20 Jul 2022 06:00:58 GMT
ENV LANG=C.UTF-8
# Wed, 20 Jul 2022 06:00:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9978870d57c2fafcab27c898466e98f17375a4054a178bd86a10691f12e56ebc`  
		Last Modified: Wed, 20 Jul 2022 06:03:08 GMT  
		Size: 59.6 MB (59603472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
