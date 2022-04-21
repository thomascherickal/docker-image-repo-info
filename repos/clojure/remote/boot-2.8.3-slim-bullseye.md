## `clojure:boot-2.8.3-slim-bullseye`

```console
$ docker pull clojure@sha256:ab9d000a0a80724b0165443ef8dabf48939efe35d3d8e06a044569f1758cbaf0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:boot-2.8.3-slim-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:798a9e42e2cad4e4bff498b8c6ddc6c4071789bf84d13911b6fc81c96c07da08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.0 MB (279965570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd9cce3145def00dd5659cbe76a52b74101faa4455c43a88c70d79971de21a65`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:47:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:51:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 20 Apr 2022 10:51:06 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:51:06 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:51:06 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 20 Apr 2022 10:51:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 20 Apr 2022 10:51:22 GMT
CMD ["jshell"]
# Thu, 21 Apr 2022 00:22:48 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 21 Apr 2022 00:22:48 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 21 Apr 2022 00:22:48 GMT
WORKDIR /tmp
# Thu, 21 Apr 2022 00:22:52 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 21 Apr 2022 00:22:52 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 21 Apr 2022 00:22:52 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 21 Apr 2022 00:23:25 GMT
RUN boot
# Thu, 21 Apr 2022 00:38:54 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 21 Apr 2022 00:38:54 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 21 Apr 2022 00:38:54 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3aa8d076675d49d85180b0ced9daef210fe4fdff4bdbb422b9cf384e591d0`  
		Last Modified: Wed, 20 Apr 2022 11:01:25 GMT  
		Size: 1.6 MB (1582162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce99fdf16e86bd02f6ad66a0e1334878528b5a4b5487850a76e0c08a7a27d56`  
		Last Modified: Wed, 20 Apr 2022 11:06:39 GMT  
		Size: 187.9 MB (187900177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec046fdb16f9695ee3167a711e2ac086a657d9fe8ea70ab384e1035d49a58582`  
		Last Modified: Thu, 21 Apr 2022 00:47:39 GMT  
		Size: 283.1 KB (283079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ce7d3d7cb29684a7fe2c425daee63ab90474c7c1520513b3746eae83302458`  
		Last Modified: Thu, 21 Apr 2022 00:47:43 GMT  
		Size: 58.8 MB (58820766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e9c7bee879a10701af341792a4e79c96eaa1619df83834f91994931547b5f6`  
		Last Modified: Thu, 21 Apr 2022 00:58:30 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:boot-2.8.3-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b55ff3aca1e2794b89f474dd909c688d4769cbad09023d4fbd9339ff25418d74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.8 MB (276838071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8643d88b936cf26f45348e7d1c8b5521c50bbac4695f25034c0ce79d730464fd`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:24:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:28:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 20 Apr 2022 10:28:48 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:28:49 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:28:50 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 20 Apr 2022 10:29:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 20 Apr 2022 10:29:07 GMT
CMD ["jshell"]
# Thu, 21 Apr 2022 03:13:08 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 21 Apr 2022 03:13:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 21 Apr 2022 03:13:09 GMT
WORKDIR /tmp
# Thu, 21 Apr 2022 03:13:14 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 21 Apr 2022 03:13:15 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 21 Apr 2022 03:13:16 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 21 Apr 2022 03:13:50 GMT
RUN boot
# Thu, 21 Apr 2022 03:31:29 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 21 Apr 2022 03:31:29 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 21 Apr 2022 03:31:30 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59f13dc084e185af417a4c6d1be2534adaff0c4f35ac2166a539260f4e8e945`  
		Last Modified: Wed, 20 Apr 2022 10:46:08 GMT  
		Size: 1.4 MB (1361221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5035d2d5c6c24e610a9317c6907a7c58efd512757d559841e5d0851512ed9c`  
		Last Modified: Wed, 20 Apr 2022 10:51:56 GMT  
		Size: 186.5 MB (186526814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab74f33161361542e07d8239c99dc27d30798e93fc3c965825dd9e02f77e3768`  
		Last Modified: Thu, 21 Apr 2022 03:43:48 GMT  
		Size: 67.3 KB (67256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a0891ff96494a352eaadf0715906fb1415e5f07d03c3eba763576c9addddc2`  
		Last Modified: Thu, 21 Apr 2022 03:43:56 GMT  
		Size: 58.8 MB (58816572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2e9bf2b18716d6818ced610263461b48825bfdc2eae422c0484fdb3aac595c`  
		Last Modified: Thu, 21 Apr 2022 03:56:11 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
