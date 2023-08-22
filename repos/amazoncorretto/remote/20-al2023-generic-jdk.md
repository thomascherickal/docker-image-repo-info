## `amazoncorretto:20-al2023-generic-jdk`

```console
$ docker pull amazoncorretto@sha256:9501725004f21f38ec4029977f6595eaf3b410d43dc8378a5472a43c7b046b8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-al2023-generic-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:190ad18be79c24d1dd5063c7eb24aa296a39223d99e8abe5012569dae29adcaa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.5 MB (260460404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf6857a8165eb824cc2fdd54c17723ed1d8be8a7056b33f47b135f567bc0914`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 20:19:35 GMT
COPY dir:c2400bc0d1a5c32eb725de8e35d10b308c821586fa71a0a3f5ba3aa5cf9bb127 in / 
# Tue, 22 Aug 2023 20:19:35 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:35:44 GMT
ARG version=20.0.2.9-1
# Tue, 22 Aug 2023 21:36:11 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && dnf install gnupg2 -y --allowerasing     && dnf install findutils -y     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && dnf install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && dnf remove -y findutils     && dnf install -y fontconfig freetype libjpeg dejavu-sans-fonts dejavu-serif-fonts dejavu-sans-mono-fonts libjpeg     && dnf clean all
# Tue, 22 Aug 2023 21:36:12 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:36:12 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:1e6dafe971b21b19c13aac9adec0ca5084ccd36d780a9b704ea649071d8e7bb9`  
		Last Modified: Thu, 10 Aug 2023 03:05:52 GMT  
		Size: 52.3 MB (52305790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7049dc0d822e17072d80ca0bba2258903d210d9aca499fac2ad4b2cd82b7c0a`  
		Last Modified: Tue, 22 Aug 2023 21:45:07 GMT  
		Size: 208.2 MB (208154614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-al2023-generic-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:fe54a89346669eca877fddbc76a099d9b9285bd3d4ffc4e34d807ccba50a2624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.4 MB (257448029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf0afda3a2a59d2ca0ad217528db410126fa74e13d1711d87052419a060b0f61`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 19:39:35 GMT
COPY dir:92c63817c19adbcfee66efbdf593beff7587a951a074d0392645d3c4900d19b4 in / 
# Tue, 22 Aug 2023 19:39:36 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:14:05 GMT
ARG version=20.0.2.9-1
# Tue, 22 Aug 2023 21:14:28 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && dnf install gnupg2 -y --allowerasing     && dnf install findutils -y     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && dnf install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && dnf remove -y findutils     && dnf install -y fontconfig freetype libjpeg dejavu-sans-fonts dejavu-serif-fonts dejavu-sans-mono-fonts libjpeg     && dnf clean all
# Tue, 22 Aug 2023 21:14:31 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:14:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:9fbecb9d3a17a188c49f0cab3521b4c760f46722f3e0e83726ccf3f972d8acbf`  
		Last Modified: Thu, 10 Aug 2023 03:04:18 GMT  
		Size: 51.3 MB (51348140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba7e0e0d49b41776f1b14e84acb557fe54d795131140ff925f87ed4f4bf07b4`  
		Last Modified: Tue, 22 Aug 2023 21:22:32 GMT  
		Size: 206.1 MB (206099889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
