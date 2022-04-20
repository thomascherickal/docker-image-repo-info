## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:44432160cf82ae36757f58e88d3f5990f2f28ee0573cde1ae1f00c20afc7d0d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:777822638df1bfb605d4c74c30ebfbe32330815ced7603ff6e6636fe1fe5b765
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.2 MB (209201838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecdb39e70adf3d9ab7180c1429371a2ef372447cfadb101b7d05e20efc3dea1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Apr 2022 21:26:09 GMT
ADD file:7fa33984010a56e1ee5aa401253e0d989c79d49005db9c39461482307d209f33 in / 
# Wed, 13 Apr 2022 21:26:10 GMT
CMD ["/bin/bash"]
# Tue, 19 Apr 2022 22:23:46 GMT
ARG version=11.0.15.9-1
# Tue, 19 Apr 2022 22:24:11 GMT
# ARGS: version=11.0.15.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 19 Apr 2022 22:24:11 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:24:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:b4b6ff8728329c46c11473e599b18813271c5059023956140f08ecaf87f7859a`  
		Last Modified: Wed, 13 Apr 2022 02:49:33 GMT  
		Size: 62.2 MB (62237641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc29cbad79c9bc29a9b354015dfe8b079799bd5426b5a8c0f03816c7613e4193`  
		Last Modified: Tue, 19 Apr 2022 22:32:26 GMT  
		Size: 147.0 MB (146964197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:79fffd74efbf0cab3216d6d382428f85efaec537d87f23b1a47d66c2b41982f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.1 MB (208059221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d909745c8f1f81aaa272f6c6c58d1e5499081488ecbba56e7f772f35e54ffc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Apr 2022 21:39:23 GMT
ADD file:b2ebb2642f1562a48fcb84ac23c60719e85ce47ae98e58a9c3b80e90779c96bc in / 
# Wed, 13 Apr 2022 21:39:24 GMT
CMD ["/bin/bash"]
# Tue, 19 Apr 2022 21:39:43 GMT
ARG version=11.0.15.9-1
# Tue, 19 Apr 2022 21:40:01 GMT
# ARGS: version=11.0.15.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 19 Apr 2022 21:40:01 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 21:40:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:7072f8fc5d0e256808f60aaf5dc2a7b918f5094683b66be0a216b4e8a859ee10`  
		Last Modified: Wed, 13 Apr 2022 02:49:29 GMT  
		Size: 63.9 MB (63870281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85077095d5a2c473594b77c6d23a963d73bf0a7e6accf188af15b4161ddc8213`  
		Last Modified: Tue, 19 Apr 2022 21:42:31 GMT  
		Size: 144.2 MB (144188940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
