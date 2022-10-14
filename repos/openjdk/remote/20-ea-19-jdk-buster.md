## `openjdk:20-ea-19-jdk-buster`

```console
$ docker pull openjdk@sha256:f42faa91d9fb916530d3aaec9aee391d10bf22b66f832b7ff8d42082a2d58333
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:20-ea-19-jdk-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:c5c41292b2dc74e6ca28f2a731a9cb9e66e333988fa82b4c2709f1f4d7e9869a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.2 MB (331237812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a312a0566e778fd1571202ef181818d5c7037216e82a2f62e38e852d3aec28db`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:01:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:01:29 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 05 Oct 2022 13:01:29 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 13:01:30 GMT
ENV LANG=C.UTF-8
# Fri, 14 Oct 2022 01:48:48 GMT
ENV JAVA_VERSION=20-ea+19
# Fri, 14 Oct 2022 01:48:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/19/GPL/openjdk-20-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='872bf878e925d040e586f05723275d769f00f5718745e0758e6345ab2ffa0b66'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/19/GPL/openjdk-20-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='3ea4c7aa0de5ed4d0e5e0d55d2ef9cfa261087e65af3fdf849ecb2186a414c0d'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 14 Oct 2022 01:48:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce765e1cc6c0bfde215679620f9f3d420f1eb249616a359ee107cce6ba3971`  
		Last Modified: Wed, 05 Oct 2022 13:06:58 GMT  
		Size: 13.9 MB (13924265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbc6249e639e7b142c0a2e71aac89da82cd8ce262686690245728f8bc20b02f`  
		Last Modified: Fri, 14 Oct 2022 01:54:42 GMT  
		Size: 197.2 MB (197172580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
