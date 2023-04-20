## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:c494f0d7acf28a7d9d41bf799bfd10a5cc314c786d7f0e033a9441a6455e324b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:070793da82a0ae2dcd6d08daf66ec5223f143d207a5cd4569fa60e38f2879c6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210265879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc51ffa390bf2a80dade1190c7620e7b46730f03602f0c160808174b7c8b7f4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Mar 2023 18:20:51 GMT
COPY dir:d74df4759bcd6e2619baa3ec354d8703c77c836345c6a887554df76aaf1d9965 in / 
# Tue, 28 Mar 2023 18:20:52 GMT
CMD ["/bin/bash"]
# Tue, 28 Mar 2023 19:10:20 GMT
ARG version=11.0.18.10-1
# Tue, 28 Mar 2023 19:10:43 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 28 Mar 2023 19:10:44 GMT
ENV LANG=C.UTF-8
# Tue, 28 Mar 2023 19:10:44 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:128d54f2c9b134270b406c5f3a41296da7c1111d3a6927f0b4451131d636151e`  
		Last Modified: Thu, 23 Mar 2023 21:24:22 GMT  
		Size: 62.5 MB (62483466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d663a74fb097421df1cf86ff5f92ae32b85d0b4a379327fb2a1d45646fc0e7`  
		Last Modified: Tue, 28 Mar 2023 19:16:37 GMT  
		Size: 147.8 MB (147782413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:3dcce35eb24667edeee2e3ad217e324e3304ec11b8cf338d6d24521bb97b08c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.1 MB (209078440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9fc23149ca1c17e172f97aa9a5f26e3058a562e43b3e0f02b444b5a9a8aeafe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Mar 2023 18:40:10 GMT
COPY dir:1d0df99dbb2a961dca382ec30c27f40e06635a9186a0715c0d2a629262a04288 in / 
# Tue, 28 Mar 2023 18:40:10 GMT
CMD ["/bin/bash"]
# Thu, 20 Apr 2023 17:40:45 GMT
ARG version=11.0.19.7-1
# Thu, 20 Apr 2023 17:41:07 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 20 Apr 2023 17:41:08 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:41:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:949542da27c3c0ab979766d37f455344960f838d9f661b9db50bec634ca7149e`  
		Last Modified: Thu, 23 Mar 2023 21:25:53 GMT  
		Size: 64.1 MB (64126936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc8a98f0e7be7c6120b0be56d2c543357756e751174d0d3d40efee7e82d0527`  
		Last Modified: Thu, 20 Apr 2023 17:50:08 GMT  
		Size: 145.0 MB (144951504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
