## `amazoncorretto:20-al2023-generic-jdk`

```console
$ docker pull amazoncorretto@sha256:47b038730f63bbd795ec56ce81ab4a0ff0f4aad6822158f2ab268fc010ba5cbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-al2023-generic-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e0882521be6a30feded877b0a13a1d09803a3a600e7bec00a7e1591b0e2afba9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.5 MB (260474189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ca9fb360e5be1b302404b80a0901c68a1e78a8c96230735ce055b7f48d572f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:58:54 GMT
COPY dir:1f2861cb5cb66982b608640300c5c9fa18eb5f3b855ebdd670700b8f8998b047 in / 
# Mon, 07 Aug 2023 19:58:55 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:59:53 GMT
ARG version=20.0.2.9-1
# Mon, 07 Aug 2023 21:00:20 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && dnf install gnupg2 -y --allowerasing     && dnf install findutils -y     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && dnf install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && dnf remove -y findutils     && dnf install -y fontconfig freetype libjpeg dejavu-sans-fonts dejavu-serif-fonts dejavu-sans-mono-fonts libjpeg     && dnf clean all
# Mon, 07 Aug 2023 21:00:21 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 21:00:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:f87c7e5d5d0812576f02b4bd88ec48dfecf7a6fa89ac4925de3439f1546d8bda`  
		Last Modified: Thu, 27 Jul 2023 17:50:07 GMT  
		Size: 52.3 MB (52309413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce1914d282000d155eec52ead9e4250ad1d839c9c441d5268120a49584e1178`  
		Last Modified: Mon, 07 Aug 2023 21:10:33 GMT  
		Size: 208.2 MB (208164776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-al2023-generic-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0331611ab15f198714346012c2822a72a3595ea44ccc20859a102e329cc0c465
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.4 MB (257448036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee80aac51195dd48504fb8619e5a2a5d12639dadc472b8fe80ded26dd7776d5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:40:41 GMT
COPY dir:d866155bb3759779912648033754c105594f55cc5e898364d07a4900eb79c222 in / 
# Mon, 07 Aug 2023 19:40:41 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:30:39 GMT
ARG version=20.0.2.9-1
# Mon, 07 Aug 2023 20:31:02 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && dnf install gnupg2 -y --allowerasing     && dnf install findutils -y     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && dnf install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && dnf remove -y findutils     && dnf install -y fontconfig freetype libjpeg dejavu-sans-fonts dejavu-serif-fonts dejavu-sans-mono-fonts libjpeg     && dnf clean all
# Mon, 07 Aug 2023 20:31:05 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:31:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:28978a1daafcb3277e8070ffe6b95fb9b5a83e6ffe571c09bd0354db9d3da1cd`  
		Last Modified: Thu, 27 Jul 2023 17:49:44 GMT  
		Size: 51.3 MB (51348282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0845029434c4387cd4284038ad4876bebffb640cda92990b647a7d57e8c7060d`  
		Last Modified: Mon, 07 Aug 2023 20:46:09 GMT  
		Size: 206.1 MB (206099754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
