## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:315462f770bd4e555084770d78d1367c02d40369e539d72324dfe7a7b6dc96d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:cf0c97bfefde579ddafe8f1c1f2468918419a78181a3ea9b265ccbd2703bf84a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210281600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:884f49128e993028e24877c72a76750bea6364fcf63dfc666a6343dc3b1efe6c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 13 May 2023 00:19:34 GMT
COPY dir:7a824a76678fb4ef17879dcecd9fac65df3d1efbef31a3b874da9f49f49b6814 in / 
# Sat, 13 May 2023 00:19:34 GMT
CMD ["/bin/bash"]
# Sat, 13 May 2023 01:33:37 GMT
ARG version=11.0.19.7-1
# Sat, 13 May 2023 01:34:02 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 13 May 2023 01:34:03 GMT
ENV LANG=C.UTF-8
# Sat, 13 May 2023 01:34:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:bf72c394abb748707ec4590d5017f36ad47098c9b92adc1b04c3ea3ba0b395f6`  
		Last Modified: Fri, 12 May 2023 00:07:44 GMT  
		Size: 62.5 MB (62494714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca57aa3ff41998ba7cda3aea10ad664a82e3fde09396157d1b38c91a39590`  
		Last Modified: Sat, 13 May 2023 01:37:04 GMT  
		Size: 147.8 MB (147786886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:4f6dbe98d26092a86992323828e3ce128f68dffdea534a42b3ed9041df4d90f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.1 MB (209085067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14ce302b2f3248524e9a58b0ef0daca41798a53fe2ad08b2d41da0dace35ff9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 May 2023 20:02:54 GMT
COPY dir:dcba415a4a8d9f29c0f5914e2b9ce92b35bd4109c9cd4a8feba13044e94360bf in / 
# Thu, 04 May 2023 20:02:55 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 21:16:20 GMT
ARG version=11.0.19.7-1
# Thu, 04 May 2023 21:16:38 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 04 May 2023 21:16:40 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 21:16:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:7691241ca28307f278612dad94d3164926fb17e58a2302a47349e0d6e001249e`  
		Last Modified: Tue, 25 Apr 2023 06:49:36 GMT  
		Size: 64.1 MB (64130990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9410ea473ac2fdcf5a9f1c5e36b37c7693a3f37b9e2ea71d5e3fdd2bf25b8626`  
		Last Modified: Thu, 04 May 2023 21:21:16 GMT  
		Size: 145.0 MB (144954077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
