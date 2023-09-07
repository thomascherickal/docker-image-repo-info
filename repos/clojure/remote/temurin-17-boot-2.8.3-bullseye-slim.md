## `clojure:temurin-17-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:e1fee8a049d3241305f698137e11b427808481f6480fd08548f86fc1253ed7a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:487f07fae61b71afc12d6ec7727c01917d3ebbad92bafab18d0eb41909cb588d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236091753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b3db47bf2a0969944b82779dd6b6d6992dedc94ae326914c055f9f3591cc899`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:03:47 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 07 Sep 2023 03:24:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:24:14 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 07 Sep 2023 03:24:14 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 07 Sep 2023 03:24:14 GMT
WORKDIR /tmp
# Thu, 07 Sep 2023 03:24:19 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 07 Sep 2023 03:24:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 07 Sep 2023 03:24:19 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 07 Sep 2023 03:24:38 GMT
RUN boot
# Thu, 07 Sep 2023 03:24:38 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 07 Sep 2023 03:24:38 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 07 Sep 2023 03:24:38 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732d09690feda2ec5aced0543a2cf8ee1aadf1e05dd333f551cc4b11eaa287a0`  
		Last Modified: Thu, 07 Sep 2023 02:06:03 GMT  
		Size: 144.8 MB (144775798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0cfeaf959e4e0d89cea5495403e174ff58b9951b4a7051ab33dfa0c9d82185`  
		Last Modified: Thu, 07 Sep 2023 03:33:17 GMT  
		Size: 1.1 MB (1077552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd29084fdc212089aba6195cbbc4ca89c335fd0c4cd1c135be65970957500cd`  
		Last Modified: Thu, 07 Sep 2023 03:33:20 GMT  
		Size: 58.8 MB (58820502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf4e8d8445e38b694a0728acd12a67edb9f6ea6e160234eee7ce7f25eda02a2`  
		Last Modified: Thu, 07 Sep 2023 03:33:17 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:73f986b49fe0f1a73db22fd972c8a9c0aa38c788a4ad842af1fbfac6c221740a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.5 MB (233491962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88104b988afd7753245a0d8b96959f4df8841ecf1f6a5d1a136cc6a6916f50f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:46:35 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 07 Sep 2023 09:09:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 09:09:46 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 07 Sep 2023 09:09:46 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 07 Sep 2023 09:09:46 GMT
WORKDIR /tmp
# Thu, 07 Sep 2023 09:09:51 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 07 Sep 2023 09:09:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 07 Sep 2023 09:09:51 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 07 Sep 2023 09:10:08 GMT
RUN boot
# Thu, 07 Sep 2023 09:10:08 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 07 Sep 2023 09:10:08 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 07 Sep 2023 09:10:09 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0067a4775f017792de5f753490d0b5645640bc00f5c264295100a66ea689ec96`  
		Last Modified: Thu, 07 Sep 2023 06:48:31 GMT  
		Size: 143.5 MB (143543493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7431cdebb714dca289c54cad5e769b95466db8459a203840468ac78b6ce765`  
		Last Modified: Thu, 07 Sep 2023 09:17:42 GMT  
		Size: 1.1 MB (1064800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afe617e30ae4f2eae6d83874b104e309baf51a13ab1cdcb4e0f4b2ff1fdb2e2`  
		Last Modified: Thu, 07 Sep 2023 09:17:45 GMT  
		Size: 58.8 MB (58820367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4a6ad8813cd8d68061045262559bfcb7c32943f714eb926ea624957df25298`  
		Last Modified: Thu, 07 Sep 2023 09:17:42 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
