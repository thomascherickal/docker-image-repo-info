## `amazoncorretto:20-al2023-generic`

```console
$ docker pull amazoncorretto@sha256:11b18c4332e933f20f7da71e7d350c5dd3b94e38604baac38bb11fd64f2af476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-al2023-generic` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3ac398a17f755cde2fda916aa5fc0852073395c312d3d34725c322cec1e4ec3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.5 MB (260479681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7e2ab9efdd4c9ef59323612545a4c5d4365d596e9d3bc21f3095d718edab64a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Jul 2023 19:20:08 GMT
COPY dir:acd83a6b32519bdad84d6a4d016402a3bfbd7ec8056e92d01a2222fd4cc63d9d in / 
# Wed, 26 Jul 2023 19:20:08 GMT
CMD ["/bin/bash"]
# Fri, 04 Aug 2023 00:20:49 GMT
ARG version=20.0.2.9-1
# Fri, 04 Aug 2023 00:21:19 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && dnf install gnupg2 -y --allowerasing     && dnf install findutils -y     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && dnf install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && dnf remove -y findutils     && dnf install -y fontconfig freetype libjpeg dejavu-sans-fonts dejavu-serif-fonts dejavu-sans-mono-fonts libjpeg     && dnf clean all
# Fri, 04 Aug 2023 00:21:20 GMT
ENV LANG=C.UTF-8
# Fri, 04 Aug 2023 00:21:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:0ccf2bf65eb109135ce4e32ed827c8fd4df1396c406122da0b40d4fd7f088839`  
		Last Modified: Thu, 20 Jul 2023 17:41:27 GMT  
		Size: 52.3 MB (52310872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887ef5e5aa4f9ae3a00631b226a36530899cd3dfcc9d667d3c1f95bdc987cee0`  
		Last Modified: Fri, 04 Aug 2023 00:23:51 GMT  
		Size: 208.2 MB (208168809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-al2023-generic` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:921255ecb9504c85c45445deee9156a249ea5ed1d25b1c459fa9cf528ea1ee81
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.5 MB (257450428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9fa7a9d5d9955696a95a9955ea2c90a4af402b8e3d4f981eb30e0828f3ef0c1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Jul 2023 19:39:44 GMT
COPY dir:ab5df2603dbae327b5eecbb1ba196f5a1f17cd096f7248968ddb73809ff1f45c in / 
# Wed, 26 Jul 2023 19:39:44 GMT
CMD ["/bin/bash"]
# Fri, 04 Aug 2023 00:50:32 GMT
ARG version=20.0.2.9-1
# Fri, 04 Aug 2023 00:50:57 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && dnf install gnupg2 -y --allowerasing     && dnf install findutils -y     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && dnf install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && dnf remove -y findutils     && dnf install -y fontconfig freetype libjpeg dejavu-sans-fonts dejavu-serif-fonts dejavu-sans-mono-fonts libjpeg     && dnf clean all
# Fri, 04 Aug 2023 00:51:00 GMT
ENV LANG=C.UTF-8
# Fri, 04 Aug 2023 00:51:00 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:91b7fefd504f27afc9eac17100f8e7fa41446c3fdfe003e74025c20a9adb95f3`  
		Last Modified: Fri, 21 Jul 2023 03:06:49 GMT  
		Size: 51.3 MB (51349707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4244381e9ac02492c89706b7fbb5fc25bbc484d3d9dbb4a2fe761011e40deb8b`  
		Last Modified: Fri, 04 Aug 2023 00:53:18 GMT  
		Size: 206.1 MB (206100721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
