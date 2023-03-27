## `openjdk:21-ea-15-jdk-slim-buster`

```console
$ docker pull openjdk@sha256:9c0b6524c546757d4432c4f40ef91df41fb07ee0c90d24e81d12c1a7c15e327b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:21-ea-15-jdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:0a46c96abc15d363d5b648b6055ea72c2665593b7c27573cc5f46525a547817c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.5 MB (229471958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d3e68d7c6fdcd971d60bad9d0ac092582540417191aefcbd46d9666cb29e67a`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:23 GMT
ADD file:44e400cc6a1bc5df5a57bda478c9accf9b58950fa2fd069cc7620128fe786770 in / 
# Thu, 23 Mar 2023 00:45:23 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 09:33:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:33:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Thu, 23 Mar 2023 09:33:59 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:33:59 GMT
ENV LANG=C.UTF-8
# Mon, 27 Mar 2023 22:48:35 GMT
ENV JAVA_VERSION=21-ea+15
# Mon, 27 Mar 2023 22:48:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='0fec1002b8c8975b181bd6966a817028d6b373cbc759254231f9b96db1fe6edd'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93cc1eb6202093a127f1f9ed2e866a51dff29321f878085c18f317cefb113ffc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 27 Mar 2023 22:48:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:cfe0f778e53ce031ef449bc02975a07f2568716dea807ed2f390d352c0001972`  
		Last Modified: Thu, 23 Mar 2023 00:48:45 GMT  
		Size: 25.9 MB (25922660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7dd89b802d8cb9cc5435e5f3b74e44a0eb080ad95666566ad37b9821083291`  
		Last Modified: Thu, 23 Mar 2023 09:36:08 GMT  
		Size: 3.1 MB (3131724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f00e59d978a21928880ee67f665e2650759a8c0c7a90bb22760616293f42ee3`  
		Last Modified: Mon, 27 Mar 2023 22:52:06 GMT  
		Size: 200.4 MB (200417574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
