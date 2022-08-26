## `amazoncorretto:latest`

```console
$ docker pull amazoncorretto@sha256:523aab36d0bcb0ff182ee907af8fc3d29669e2902fa2d05f5505f00c1ff69dfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:latest` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3ff9755fdb04187c4abc386b8452ef42a24ad0a82b63111c901ebcd27d6adbc6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137906580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be79e949281f9829880b4f6079c37c85add7084df9dd7386c9009653eabbc05e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 01:19:36 GMT
ADD file:ebfd33425a17b16a9e560de15c91108bf2ee740f284a1482a7105b420ff22678 in / 
# Fri, 26 Aug 2022 01:19:37 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 02:02:55 GMT
ARG version=1.8.0_342.b07-4
# Fri, 26 Aug 2022 02:03:17 GMT
# ARGS: version=1.8.0_342.b07-4
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 26 Aug 2022 02:03:18 GMT
ENV LANG=C.UTF-8
# Fri, 26 Aug 2022 02:03:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:fd06b60db4951fd95b43a9e73fb084fe7d2afcd4ff464472ead5548cd1c28717`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 62.3 MB (62326701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6626eeeb161e510cb277ee5c8edd4e8c33de2e80145c25c54050fc21e1d357e2`  
		Last Modified: Fri, 26 Aug 2022 02:07:06 GMT  
		Size: 75.6 MB (75579879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:latest` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:35d469f6bc7db479515c673257367f1cdc3e9d29ed4371255b5e7270d0a55a09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123541007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84e049975ebb65a84149ca58cb0026fa252d6ed2edbc521286b8410bed7f91a8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Aug 2022 00:39:31 GMT
ADD file:a0918d3dfd5c1b4e0594c53d0dfc4c97f1ebaf14085279c79f36f06cf7ed95ee in / 
# Fri, 26 Aug 2022 00:39:32 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 01:01:01 GMT
ARG version=1.8.0_342.b07-4
# Fri, 26 Aug 2022 01:01:18 GMT
# ARGS: version=1.8.0_342.b07-4
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 26 Aug 2022 01:01:18 GMT
ENV LANG=C.UTF-8
# Fri, 26 Aug 2022 01:01:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:12df598bc31e0ff3cadc2667d34dc645b837d712e7e15ce3e9080ae91744dcd0`  
		Last Modified: Mon, 22 Aug 2022 22:09:44 GMT  
		Size: 63.9 MB (63938765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b3384c6fc6a4bb8506747a4edc13e891c8719d6ac5f3e846350bc2080b93b`  
		Last Modified: Fri, 26 Aug 2022 01:03:31 GMT  
		Size: 59.6 MB (59602242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
