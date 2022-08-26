## `amazoncorretto:18-al2-full`

```console
$ docker pull amazoncorretto@sha256:1e816e092174dc281fcd248d598a880fdc4825d387161b9c2bd2a94a422112e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:18-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:abd184a8c063f46e926c51191511c59728aec81a3deece9ab21a5082ce25c1cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.0 MB (215029980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9334228bb59ed1d5d15b28a265eb7b8a2cceb9dbc6854df7abd9a9680e2233f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 01:19:36 GMT
ADD file:ebfd33425a17b16a9e560de15c91108bf2ee740f284a1482a7105b420ff22678 in / 
# Fri, 26 Aug 2022 01:19:37 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 02:05:00 GMT
ARG version=18.0.2.9-1
# Fri, 26 Aug 2022 02:05:25 GMT
# ARGS: version=18.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 26 Aug 2022 02:05:26 GMT
ENV LANG=C.UTF-8
# Fri, 26 Aug 2022 02:05:26 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
```

-	Layers:
	-	`sha256:fd06b60db4951fd95b43a9e73fb084fe7d2afcd4ff464472ead5548cd1c28717`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 62.3 MB (62326701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00fc559e0f0c1b0fda19aaa7b981bc21b53461481a104b5cd5310320a51223c`  
		Last Modified: Fri, 26 Aug 2022 02:08:57 GMT  
		Size: 152.7 MB (152703279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:18-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:7b586d734f779754dc7ce1b1a1677b509816364345db9765524bee7c69323da4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.3 MB (215313616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:564b3e40a87cd59cbf8655cd1dcdbe60e912057972a5c408b2c8c23c94dae93a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 00:39:31 GMT
ADD file:a0918d3dfd5c1b4e0594c53d0dfc4c97f1ebaf14085279c79f36f06cf7ed95ee in / 
# Fri, 26 Aug 2022 00:39:32 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 01:02:14 GMT
ARG version=18.0.2.9-1
# Fri, 26 Aug 2022 01:02:31 GMT
# ARGS: version=18.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 26 Aug 2022 01:02:32 GMT
ENV LANG=C.UTF-8
# Fri, 26 Aug 2022 01:02:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
```

-	Layers:
	-	`sha256:12df598bc31e0ff3cadc2667d34dc645b837d712e7e15ce3e9080ae91744dcd0`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 63.9 MB (63938765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa256c032ea30a19222d09b401bfe7a023caac99781de9f6a7de8ecd30a8b3c`  
		Last Modified: Fri, 26 Aug 2022 01:05:19 GMT  
		Size: 151.4 MB (151374851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
