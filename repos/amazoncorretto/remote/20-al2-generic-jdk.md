## `amazoncorretto:20-al2-generic-jdk`

```console
$ docker pull amazoncorretto@sha256:6307922a61462199ce85774d81c455e699e0e431c6b86432c90802579a2d6e43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-al2-generic-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:dff0a66d464c5bf0084cf9bdd14c3934f4846ab4f5a965564590e28f554d8000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.4 MB (223388099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5684a03aa31facae1c7ab543487129ef8d27a04a849bfdb8a28db3af62b81139`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:59:12 GMT
COPY dir:a1cfeec8f9b5a4b857222f4bbc7f5fb80ef351168a5f48841d4545523a0a3e1c in / 
# Mon, 07 Aug 2023 19:59:13 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:59:24 GMT
ARG version=20.0.2.9-1
# Mon, 07 Aug 2023 20:59:48 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 07 Aug 2023 20:59:48 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:59:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:c0184eb4a5d5dddba3605f9adcde7e4af58050e9e4ed44751e74957c2ad0f1b4`  
		Last Modified: Tue, 01 Aug 2023 21:03:56 GMT  
		Size: 62.5 MB (62467383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36072a9da080e6da91896aa5694045bd081eed643720b50126352b308923c15b`  
		Last Modified: Mon, 07 Aug 2023 21:09:53 GMT  
		Size: 160.9 MB (160920716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-al2-generic-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:be3d585543a13ff9a8f7f01b2f78d7a66d1fd849596291b25adefb89b3570b53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.1 MB (223097678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:178db0115785ad7168004b4b152bac02006f2108094cb8d453c6e2a3b87165f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:40:56 GMT
COPY dir:95dabd7a234aac70a826a1e3c0eafa3928b0be72717af1dea469f66b7db891d5 in / 
# Mon, 07 Aug 2023 19:40:57 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:30:15 GMT
ARG version=20.0.2.9-1
# Mon, 07 Aug 2023 20:30:35 GMT
# ARGS: version=20.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-20-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-20-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 07 Aug 2023 20:30:37 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:30:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-20-amazon-corretto
```

-	Layers:
	-	`sha256:c3b5a1e75067e9d540ad8d844cad5a291a8cce89e1a3ed8e0f362a5736d3030c`  
		Last Modified: Wed, 02 Aug 2023 19:26:38 GMT  
		Size: 64.1 MB (64129548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d2b58a5a8eb917eca483f0151d4bfb004afc304f83d70f02b5cf2d0d4ec70d`  
		Last Modified: Mon, 07 Aug 2023 20:45:29 GMT  
		Size: 159.0 MB (158968130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
