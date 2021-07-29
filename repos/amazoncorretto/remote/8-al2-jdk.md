## `amazoncorretto:8-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:e517b1051888b935855f19740cdd69faf76b1a5eb5f6ea8c34989c04671f91fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:99383180a63638b69ccce247aa6b7dbb770cf2b108e0d219f0b5f0c9a4e7299f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137299042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1c4e3803af8fd91c9b8a4f45546ba5c654ab65a15b1e7bff1627cba43a1fd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:19:45 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:19:46 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:19:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed3eb17202682b67a716d65d9a7b156337c35c258c7d56eaf2f6025921237a4`  
		Last Modified: Wed, 28 Jul 2021 23:20:45 GMT  
		Size: 75.3 MB (75333036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c3ae270b98b9fe18e7eda62aede47ca5834bc4ad804e848b5c0d590e0f36b7c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122952748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3949d0817afd993fb56e0c6cb2c60acbb4815eec064750beeb2379fc2c090c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 28 Jul 2021 23:39:42 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Jul 2021 23:39:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Jul 2021 23:39:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5230c70e909e8047c9eadb7a1e0fecdf1baf98003a2f6a56063922975157258e`  
		Last Modified: Wed, 28 Jul 2021 23:40:44 GMT  
		Size: 59.4 MB (59384856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
