## `openjdk:17-ea-31-jdk`

```console
$ docker pull openjdk@sha256:08dccb53cbb657600408aa483ff714523d007473ea965b4a0a27553fe624eede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `openjdk:17-ea-31-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:586d13dfa993cfbe57643b1934cf738b6d2a6eca830f14a339a26f4273f3dfd4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.7 MB (242695166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40ad801e33e11b66720e215426fa59469cdb99316a5daf537c7413316f3f9c1`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 23 Jul 2021 01:13:10 GMT
ADD file:c047ac1784a3670f52d12ad67cf238654237149dc2c9d7b921cd005c7ec42105 in / 
# Fri, 23 Jul 2021 01:13:11 GMT
CMD ["/bin/bash"]
# Fri, 23 Jul 2021 06:40:31 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 23 Jul 2021 06:41:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 23 Jul 2021 06:41:12 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:41:13 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 06:41:13 GMT
ENV JAVA_VERSION=17-ea+31
# Fri, 23 Jul 2021 06:42:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/31/GPL/openjdk-17-ea+31_linux-x64_bin.tar.gz'; 			downloadSha256='b66b6d200604e1bfa5d5642162626601d262756a6f313d1b8532dec41c870ab0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/31/GPL/openjdk-17-ea+31_linux-aarch64_bin.tar.gz'; 			downloadSha256='6879cd8978ad5b00cbf56ee2c1b297142ff0a6017df29a66ffa80b8aa864037f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jul 2021 06:42:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1da50e1664e1b58d93182fe5af093c642668ec93f67fcd8215b9c1979930b84d`  
		Last Modified: Fri, 23 Jul 2021 01:14:27 GMT  
		Size: 42.2 MB (42178827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c8e5a84542212d0126ce88facd146befb1c731fb4faafb50a7b96ad0568cd9`  
		Last Modified: Fri, 23 Jul 2021 06:49:18 GMT  
		Size: 13.4 MB (13390485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdffc1c6598d11b0c9b93cbabad3a7d89bd1d3515eef9e8d2af6758065b955bc`  
		Last Modified: Fri, 23 Jul 2021 06:50:42 GMT  
		Size: 187.1 MB (187125854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-31-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:44aada012fa8b78987151d215a1ecfea03c3e08c61648a940c037e23172d2811
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.1 MB (242141799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8133a7bd6c5cbd58397877306ced813dccc9f66d8867aab90c66260c1f984302`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 23 Jul 2021 00:50:01 GMT
ADD file:2b2b9653730f3bb9d3a6327d4b9a6b425279decd90b84755c033b95536ebe027 in / 
# Fri, 23 Jul 2021 00:50:02 GMT
CMD ["/bin/bash"]
# Fri, 23 Jul 2021 04:34:01 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 23 Jul 2021 04:34:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 23 Jul 2021 04:34:49 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:34:49 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 04:34:49 GMT
ENV JAVA_VERSION=17-ea+31
# Fri, 23 Jul 2021 04:34:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/31/GPL/openjdk-17-ea+31_linux-x64_bin.tar.gz'; 			downloadSha256='b66b6d200604e1bfa5d5642162626601d262756a6f313d1b8532dec41c870ab0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/31/GPL/openjdk-17-ea+31_linux-aarch64_bin.tar.gz'; 			downloadSha256='6879cd8978ad5b00cbf56ee2c1b297142ff0a6017df29a66ffa80b8aa864037f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jul 2021 04:34:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a21bf021f71862240d392ffdd7f376294fa46f2729f1771f269c1a888d0aab25`  
		Last Modified: Fri, 23 Jul 2021 00:51:19 GMT  
		Size: 42.0 MB (42040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20d17a0583d5448fece8a45dc16fcd83266885f5eabbeaa44c9bcc8738ed0fa`  
		Last Modified: Fri, 23 Jul 2021 04:45:32 GMT  
		Size: 14.2 MB (14170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ebdeccb237bdbc57b85eb83d1fab19b1a89c6ec6126b7a1d3b4f9fd5503f35`  
		Last Modified: Fri, 23 Jul 2021 04:47:11 GMT  
		Size: 185.9 MB (185930129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-31-jdk` - windows version 10.0.17763.2061; amd64

```console
$ docker pull openjdk@sha256:b9982a8855ac04e9ca96430fc2ba33afc865ce88e4b7f020e755631c1f84adcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2868574620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:defcd2409b7a69eb676dc83c124439c5abebe403fd1adc25b81393f87ee54617`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 02:43:11 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Jul 2021 02:55:40 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Jul 2021 02:56:53 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 15 Jul 2021 22:20:06 GMT
ENV JAVA_VERSION=17-ea+31
# Thu, 15 Jul 2021 22:20:08 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/31/GPL/openjdk-17-ea+31_windows-x64_bin.zip
# Thu, 15 Jul 2021 22:20:10 GMT
ENV JAVA_SHA256=b46f818241d7d1a01192b061500a905e0ee1ccc2b0e41baa0c85ffd5c557002a
# Thu, 15 Jul 2021 22:21:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 15 Jul 2021 22:21:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60588ed228454a5b9a3ebf90d5ae7109392676a95ebab716cf7bd486f4e257ae`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 365.3 KB (365286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1803aa8cded0dbe983dc584b95721731baff32adc0a819e4331756bd0a7a9b38`  
		Last Modified: Wed, 14 Jul 2021 03:46:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e8b66d878091e45d7ce5b9c5fa1033aabd86bc416035f11a6852c31fb4ff1c`  
		Last Modified: Wed, 14 Jul 2021 03:46:11 GMT  
		Size: 323.7 KB (323703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6de6405871bc39966da2d5d80b5e4bbd1eb7035a2b211b9ebe17d472fd5db2`  
		Last Modified: Thu, 15 Jul 2021 22:37:37 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4815db0be0fa875ae32293c8ef8b8d4bd76fef63f9d0acd1cc914c3ff819831`  
		Last Modified: Thu, 15 Jul 2021 22:37:37 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc8c1ced3644381271bb33c08c8011f7e69a95388dfa5c4e6f176a1bd89069f`  
		Last Modified: Thu, 15 Jul 2021 22:37:37 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec8fcd11bd677bbae2786c93406bc75a1fbe89fbf85f2f422df49d0c7cd916f`  
		Last Modified: Thu, 15 Jul 2021 22:37:58 GMT  
		Size: 182.4 MB (182430320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6b5d870816277974641e49c36b67502e2fd1be2de9494bd9ea882fdcd4286a`  
		Last Modified: Thu, 15 Jul 2021 22:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-31-jdk` - windows version 10.0.14393.4530; amd64

```console
$ docker pull openjdk@sha256:ccbb87cb3adbf119cc4142669fee86f4f7846520254cc14da71514d41747a680
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6452763951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c0016972ea8c8bd84a914eec36a424a245513667e3b7abb41d92a05ae44e59c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 02:47:31 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Jul 2021 02:59:29 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Jul 2021 03:00:47 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 15 Jul 2021 22:22:03 GMT
ENV JAVA_VERSION=17-ea+31
# Thu, 15 Jul 2021 22:22:05 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/31/GPL/openjdk-17-ea+31_windows-x64_bin.zip
# Thu, 15 Jul 2021 22:22:08 GMT
ENV JAVA_SHA256=b46f818241d7d1a01192b061500a905e0ee1ccc2b0e41baa0c85ffd5c557002a
# Thu, 15 Jul 2021 22:24:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 15 Jul 2021 22:24:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4efeafa471485cac56b3d111ef85272828cab146a6a1ada3aeff81bcb4dda8`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 328.5 KB (328523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b9d5fc77f9415b1d2edd80e47bb01755c2f5c19a823bc39db43e4916171dde`  
		Last Modified: Wed, 14 Jul 2021 03:46:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02ce0ecdf569be2c6b0f4004fb93d010966b94dab71a4bd9c6ea67ae3ede4fb`  
		Last Modified: Wed, 14 Jul 2021 03:46:53 GMT  
		Size: 364.3 KB (364267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8889c88d8b5359beb238a185c4ba2f358d28c6b854c2669743c35a6771fd83a7`  
		Last Modified: Thu, 15 Jul 2021 22:38:20 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c6caaf86d21b0059f9f4a38840dfd756fb5608078314f5c5b58715315fcae8`  
		Last Modified: Thu, 15 Jul 2021 22:38:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1419fcc2365e34398955b7b887c0c72439d230ae71962b11dcd53afeb38e6bdd`  
		Last Modified: Thu, 15 Jul 2021 22:38:20 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ad6f3d86fcf88b52c3b55bbcfd6c05ce52e98261604bdc335e60cabab3b628`  
		Last Modified: Thu, 15 Jul 2021 22:38:39 GMT  
		Size: 182.4 MB (182430726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80c5405cb8c911dbe3cea13d45551e98d6c406d785493c0c7c3d0e029cbc180`  
		Last Modified: Thu, 15 Jul 2021 22:38:20 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
