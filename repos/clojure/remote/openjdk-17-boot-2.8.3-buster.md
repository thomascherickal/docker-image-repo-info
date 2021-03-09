## `clojure:openjdk-17-boot-2.8.3-buster`

```console
$ docker pull clojure@sha256:e4bbebaaa15c5752b43b1066cf70d1a4f5ffbf02a6744d880ee5b55104c0765b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-boot-2.8.3-buster` - linux; amd64

```console
$ docker pull clojure@sha256:ba170cbdd545c4046a65c9e79d792fba964d40477ac5effe889ac46979a11149
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.6 MB (378635491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea584e04e167f2512d5609ffcc0e71c02a36c835e157100dd4a8aa6ad45ad03e`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:35:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 20:56:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 20:56:37 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 09 Mar 2021 20:56:38 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:56:38 GMT
ENV LANG=C.UTF-8
# Tue, 09 Mar 2021 20:56:38 GMT
ENV JAVA_VERSION=17-ea+12
# Tue, 09 Mar 2021 20:56:48 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/12/GPL/openjdk-17-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='e281f7d1fd2aaa858b02d5be451c51a9ed836c78d002cb82b114e6c36041eebf'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/12/GPL/openjdk-17-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='e2ae713390655d0cfd8302cb2c840553404a3e366162ba5b9a2410ea7b6f1c27'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 20:56:48 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:53:55 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 09 Mar 2021 21:53:55 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 09 Mar 2021 21:53:55 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:53:56 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Tue, 09 Mar 2021 21:53:56 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 09 Mar 2021 21:53:56 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 09 Mar 2021 21:54:16 GMT
RUN boot
# Tue, 09 Mar 2021 21:54:17 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7467d1831b6947c294d92ee957902c3cd448b17c5ac2103ca5e79d15afb317c3`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 7.8 MB (7830684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab2c490a3cea21cc051ff29c33cc9857418edfa1be9966124b18abe1d5ae16`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 10.0 MB (9996459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15a0f46f8c38f4ca7daecf160ba9cdb3ddeafda769e2741e179851cfaa14eec`  
		Last Modified: Tue, 09 Feb 2021 04:46:23 GMT  
		Size: 51.8 MB (51830963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415655c50d52018d0916c838b59d5ee0a87aea61c2464768eae0a629075c7263`  
		Last Modified: Tue, 09 Mar 2021 21:10:07 GMT  
		Size: 13.9 MB (13921302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfd6bc83dd557539e57f3ecfeec88e5af8ad45aedd020462975fd1f4f60eb38`  
		Last Modified: Tue, 09 Mar 2021 21:10:20 GMT  
		Size: 185.8 MB (185828422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83cd4fab091e7cb8e41ff8d1da6a949535cb5dbd5283c491931ad01654ccf5a`  
		Last Modified: Tue, 09 Mar 2021 22:09:47 GMT  
		Size: 6.9 KB (6924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1363d2a624d271ee9ecd790a7e1ed1d9b5571ac95598de8c7361a0f74705fd76`  
		Last Modified: Tue, 09 Mar 2021 22:09:50 GMT  
		Size: 58.8 MB (58820539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-boot-2.8.3-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:458b88d3b894d6b9b589c4a701360ca7df46e19c120fedfc185d18277dbdec52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.4 MB (374377350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d3aec2368a920e58402af52faa32c0c70cd3bb6ece223aed9f9b2df78a4bb5`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:40:45 GMT
ADD file:78412ee35e3dc6fb5fdfce41eb05dd273ba1d49328ab327465639bfa4821aa51 in / 
# Tue, 09 Feb 2021 02:40:50 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:43:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:43:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:44:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:10:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:10:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 09 Feb 2021 07:10:53 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 07:10:54 GMT
ENV LANG=C.UTF-8
# Thu, 04 Mar 2021 01:11:26 GMT
ENV JAVA_VERSION=17-ea+12
# Thu, 04 Mar 2021 01:12:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/12/GPL/openjdk-17-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='e281f7d1fd2aaa858b02d5be451c51a9ed836c78d002cb82b114e6c36041eebf'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/12/GPL/openjdk-17-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='e2ae713390655d0cfd8302cb2c840553404a3e366162ba5b9a2410ea7b6f1c27'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 04 Mar 2021 01:12:30 GMT
CMD ["jshell"]
# Thu, 04 Mar 2021 01:56:07 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 04 Mar 2021 01:56:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 04 Mar 2021 01:56:08 GMT
WORKDIR /tmp
# Thu, 04 Mar 2021 01:56:10 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Thu, 04 Mar 2021 01:56:11 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 04 Mar 2021 01:56:12 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 04 Mar 2021 01:56:34 GMT
RUN boot
# Thu, 04 Mar 2021 01:56:35 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:c78c297fb0d010ee085f95ae439636ecb167b050c1acb4273bd576998cf94a83`  
		Last Modified: Tue, 09 Feb 2021 02:47:03 GMT  
		Size: 49.2 MB (49183229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06af62193c25241eb123af8cf115c7a6298e834976fe148ac79ec11a7ca06ee5`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 7.7 MB (7694122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b846e1b73901174c506ae5e6219ac2f356ef71eaa5896dfbc238dc67ca4bf73`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb44d26a138a8d064a4ab8f9b472c64e7136c2482ec5af19bab8811b6d2c15b7`  
		Last Modified: Tue, 09 Feb 2021 04:57:46 GMT  
		Size: 52.2 MB (52165287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e26e0ab11a8be6b1e0ab54b0d53c323acda50b89d3549bd9c10527f3f79e07`  
		Last Modified: Tue, 09 Feb 2021 07:21:52 GMT  
		Size: 14.7 MB (14673596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79f8f427367d4bbf43d7c9f189258b5748a156e68c3f1c3110352e5314eea14`  
		Last Modified: Thu, 04 Mar 2021 01:18:20 GMT  
		Size: 181.8 MB (181849769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e96ffafee8137d14e6ef6af22cd7383fd75d6d2487dce21006d665c23262e97`  
		Last Modified: Thu, 04 Mar 2021 02:00:45 GMT  
		Size: 6.9 KB (6923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec65ebcf0b76c6206cd7b806335570a8465b76571e09e2e4ea3b22a3e0481685`  
		Last Modified: Thu, 04 Mar 2021 02:00:50 GMT  
		Size: 58.8 MB (58820143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
