## `amazoncorretto:17-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:baaf23281606d8fd6473342b64118627781949ac2443bace8b0636aa75e59d16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:30aa0c595a2230ec8de77d30cde3b78d5afd215a937caaa7bc63e5fcd4a4dcbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.0 MB (213966142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54d5e84fad68f80999086d65754705da81f6d41ef649c8389666175b4bee8dd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 Aug 2022 00:20:15 GMT
ADD file:56a385790046ac5dfb85932009eb1e99c8593221e306b937274c477c05cc9886 in / 
# Fri, 12 Aug 2022 00:20:15 GMT
CMD ["/bin/bash"]
# Tue, 16 Aug 2022 23:20:42 GMT
ARG version=17.0.4.9-1
# Tue, 16 Aug 2022 23:21:09 GMT
# ARGS: version=17.0.4.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 16 Aug 2022 23:21:10 GMT
ENV LANG=C.UTF-8
# Tue, 16 Aug 2022 23:21:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:5e0be87f98fb0e8a6ecddb6b717178ddc6555638e6e89d39929d47654b79739d`  
		Last Modified: Mon, 01 Aug 2022 22:09:03 GMT  
		Size: 62.3 MB (62316216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770928b554525a62da2f76fbf0ce0131918c7ff35efabb69df5cbb3b9bf044cd`  
		Last Modified: Tue, 16 Aug 2022 23:25:47 GMT  
		Size: 151.6 MB (151649926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:7804761e5f33122b4e78a0d68f0c86874c213dcbc7078f96c970a0a9edb6705f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.1 MB (214073843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dadc26f76553f2034eb29e354e278a2ac127487a9dbfc198aa3aa5abc5ea0a1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 Aug 2022 00:39:26 GMT
ADD file:3ec97c6bec2a8682b0b4088021da97853effeb7dfafb69329cfcb5686c3dee30 in / 
# Fri, 12 Aug 2022 00:39:28 GMT
CMD ["/bin/bash"]
# Tue, 16 Aug 2022 22:39:58 GMT
ARG version=17.0.4.9-1
# Tue, 16 Aug 2022 22:40:15 GMT
# ARGS: version=17.0.4.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 16 Aug 2022 22:40:16 GMT
ENV LANG=C.UTF-8
# Tue, 16 Aug 2022 22:40:16 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:9f9c648afd7976bdc42d03595d6a1c1c502c47f18abb3f42a9a20b38e7d6e161`  
		Last Modified: Mon, 01 Aug 2022 22:09:01 GMT  
		Size: 63.9 MB (63927916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d890038e0e09913d19ab53ed7c992a7d688997807114e7c4a6a1ab986100ba79`  
		Last Modified: Tue, 16 Aug 2022 22:42:03 GMT  
		Size: 150.1 MB (150145927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
