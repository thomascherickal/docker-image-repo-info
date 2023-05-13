## `amazoncorretto:20-al2-full`

```console
$ docker pull amazoncorretto@sha256:2b12f75ab046b7434f80117fafeba3d5e0e92287840751d22e7cb9937646e9cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f9987a02cd5b1a774a2fcf7d4ac7e372fbad8f004675497b9ad089f295e7f47a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.3 MB (223258855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:527fd3dc04b85056ddaba7b34cf89bf7210d0277944ceb62e3c7a69234da5c1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 13 May 2023 00:19:34 GMT
COPY dir:7a824a76678fb4ef17879dcecd9fac65df3d1efbef31a3b874da9f49f49b6814 in / 
# Sat, 13 May 2023 00:19:34 GMT
CMD ["/bin/bash"]
# Sat, 13 May 2023 01:34:57 GMT
ARG version=20.0.1.9-1
# Sat, 13 May 2023 01:35:25 GMT
# ARGS: version=20.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 13 May 2023 01:35:25 GMT
ENV LANG=C.UTF-8
# Sat, 13 May 2023 01:35:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:bf72c394abb748707ec4590d5017f36ad47098c9b92adc1b04c3ea3ba0b395f6`  
		Last Modified: Fri, 12 May 2023 00:07:44 GMT  
		Size: 62.5 MB (62494714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41f68f57cf18fd2a37785b55a0470e3bd816e7d529c0a63c580e3c49cdbd784`  
		Last Modified: Sat, 13 May 2023 01:38:09 GMT  
		Size: 160.8 MB (160764141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c3c0b61c46629d30d04703593ebd8dd517470b182fd16ceb1aece2c08d7a56d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.9 MB (222934738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309e783ce21b7f5b20edb5bee97cb9347e1980a137fce6f6f0cd1bde0afe7d2b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 May 2023 20:02:54 GMT
COPY dir:dcba415a4a8d9f29c0f5914e2b9ce92b35bd4109c9cd4a8feba13044e94360bf in / 
# Thu, 04 May 2023 20:02:55 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 21:19:01 GMT
ARG version=20.0.1.9-1
# Thu, 04 May 2023 21:19:19 GMT
# ARGS: version=20.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 04 May 2023 21:19:21 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 21:19:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:7691241ca28307f278612dad94d3164926fb17e58a2302a47349e0d6e001249e`  
		Last Modified: Tue, 25 Apr 2023 06:49:36 GMT  
		Size: 64.1 MB (64130990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56aea19d8d42e5ab5271a0231d569c7f1dce63fd2948821b144eaa4ed690f2e`  
		Last Modified: Thu, 04 May 2023 21:23:56 GMT  
		Size: 158.8 MB (158803748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
