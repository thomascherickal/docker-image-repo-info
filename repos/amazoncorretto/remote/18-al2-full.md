## `amazoncorretto:18-al2-full`

```console
$ docker pull amazoncorretto@sha256:bf51a65227c2fb599f4ef9709149f16694072cfef6e3d2b8933f64fb7f43ea8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:18-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5036560fafd316ce321a3a2f4dcc8c250398e371062eeaa99beb3790e3392056
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.0 MB (215010316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d288c3a05517e71058fa928d253a5f85723887731851da354e9f423cfc3444`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
# Wed, 04 May 2022 00:04:00 GMT
ARG version=18.0.1.10-1
# Wed, 04 May 2022 00:04:23 GMT
# ARGS: version=18.0.1.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 04 May 2022 00:04:24 GMT
ENV LANG=C.UTF-8
# Wed, 04 May 2022 00:04:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea513dd92a36de870cc4626f3cdaf11518603c6b369e3bea008282720eaacfae`  
		Last Modified: Wed, 04 May 2022 00:08:16 GMT  
		Size: 152.7 MB (152719174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:18-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:51b583038a4fcb9f6b89c4caf3cce9a7aacef6353f928d892f5e1d0d7fc22ad9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.3 MB (215267350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5252f1ad1a8687c460e0011ee37eb7a00d5375ce242c8cf293690a2769b52e3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
# Wed, 04 May 2022 00:22:02 GMT
ARG version=18.0.1.10-1
# Wed, 04 May 2022 00:22:19 GMT
# ARGS: version=18.0.1.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 04 May 2022 00:22:19 GMT
ENV LANG=C.UTF-8
# Wed, 04 May 2022 00:22:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e4b006e4296412de23db80958843b6fb204408bbb0567c787c90b5bc821204`  
		Last Modified: Wed, 04 May 2022 00:25:04 GMT  
		Size: 151.4 MB (151365171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
