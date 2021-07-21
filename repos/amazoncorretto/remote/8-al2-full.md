## `amazoncorretto:8-al2-full`

```console
$ docker pull amazoncorretto@sha256:81956f584cab7299043125c9a3b92f11d6d82658bc5d4683cde24543999f62ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c0b919781ba3a5562647ef462498de174c06355a3aa2c494dd5a61b5a93cb58f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137298994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940da094e12101ea77abd14cd1f07fedc72d6b7d2c8db7af8c3e415f653f2b3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jul 2021 23:38:14 GMT
ADD file:87c0c8c13a50d18c9b35e048d635d04fcd6fc06e9416c68a5c3024c83b166177 in / 
# Thu, 15 Jul 2021 23:38:15 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:19:58 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:20:19 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:20:19 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:20:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:430235fb155c55a4e5a8c494a918c1d1bf2473e93cc35c4242ae089785dc1a42`  
		Last Modified: Fri, 09 Jul 2021 13:29:48 GMT  
		Size: 62.0 MB (61966006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb7345e871527554f60a16d3ccbb1227c55c86687fe1b3a27de765c1dd3b461`  
		Last Modified: Wed, 21 Jul 2021 00:22:06 GMT  
		Size: 75.3 MB (75332988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:177857b0ae589b166ff820384a1b64b3004c2eea938b5d7d805e61f34732f1f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122953715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8d5108387d4b26fa217560ed9f0048bcdae56151829645d3ef7477a19ff43f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 16 Jul 2021 00:09:26 GMT
ADD file:555fe2ebaf4a5e69a533b39ac234d3f7c6d7de6333e2882558b1b92f1320c8a9 in / 
# Fri, 16 Jul 2021 00:09:27 GMT
CMD ["/bin/bash"]
# Wed, 21 Jul 2021 00:39:20 GMT
ARG version=1.8.0_302.b08-1
# Wed, 21 Jul 2021 00:39:37 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 21 Jul 2021 00:39:38 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:39:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:6bc2b81b61fecbd717658fab4af4ed0a6b9e5a2e28323439c47d57a34db1908f`  
		Last Modified: Fri, 16 Jul 2021 00:10:24 GMT  
		Size: 63.6 MB (63567892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8400adb2e143e69e28d625f26dcb11c7261437ddaf5acd161e70e5fe4c60ed`  
		Last Modified: Wed, 21 Jul 2021 00:41:00 GMT  
		Size: 59.4 MB (59385823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
