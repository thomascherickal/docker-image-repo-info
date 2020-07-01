## `amazoncorretto:8-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:f02ab1693a28c294c510134b561f4d512c9b580d753273af15fb3e8a9e155849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:728580cf6d37d1ff257bfa81218bbd9b68b5ddf7673d8a4d23f54dc622b93aa5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.9 MB (135946990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5693ce88e0758b986a348bc3ace1d950a79d5b0c890ddd80b1ce95b6ce06fe34`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:04 GMT
ADD file:788af9048b1c163347d7a8349f8ecf5721b4d8b63395ec8c6ca6d0732f57acdd in / 
# Tue, 30 Jun 2020 20:20:05 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 20:54:42 GMT
ARG version=1.8.0_252.b09-1
# Tue, 30 Jun 2020 20:55:15 GMT
# ARGS: version=1.8.0_252.b09-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 30 Jun 2020 20:55:16 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:3d24604292f287c31563b1f563e83307e7915909506659401fb07c1c3e6e164c`  
		Last Modified: Tue, 30 Jun 2020 20:21:31 GMT  
		Size: 61.7 MB (61684682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad451488ff0da625370ff1d3271c04a3cb41612f102190260b80adb679ab8c7`  
		Last Modified: Tue, 30 Jun 2020 20:56:16 GMT  
		Size: 74.3 MB (74262308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:547c64acb34a3cfd27a7cf8dbd8e696ffe2e0711d49433cfc79eb51fa5349400
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121498577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0114aa043373c2e90e9df85f3fc120ffc49a03a729db1b34f4f5d3ec3ab0dea0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 21:59:07 GMT
ADD file:c597ed16b945b44bdc9a607ac9730b470dd169fb94a5ca4e000d07318157d4f8 in / 
# Tue, 30 Jun 2020 21:59:09 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 23:33:05 GMT
ARG version=1.8.0_252.b09-1
# Tue, 30 Jun 2020 23:33:33 GMT
# ARGS: version=1.8.0_252.b09-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 30 Jun 2020 23:33:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6c0fd36c9881cb99dbcd7fe98cfd04a4a653e35c4c1195b7cb7d339eaec9dd79`  
		Last Modified: Tue, 30 Jun 2020 22:00:22 GMT  
		Size: 63.2 MB (63163782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2537c1d3f49f055fc608476205912e3f27f2b8dffe6a1a001cffedbbfa14de24`  
		Last Modified: Tue, 30 Jun 2020 23:34:43 GMT  
		Size: 58.3 MB (58334795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
