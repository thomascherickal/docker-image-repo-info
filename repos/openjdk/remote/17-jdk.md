## `openjdk:17-jdk`

```console
$ docker pull openjdk@sha256:baa4b31572ae18c8c63ba8b1a3879e8eeef697af33d78419e0a228b6be27a4f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `openjdk:17-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:b823292cb4065a96238ffa7ca5358bda019df30ed0c6dfe676d8af08222264d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.7 MB (242682194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:751cfcc067d2769aac9859d5203c176905f04989f573123e78375037d814d9b5`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 17:23:40 GMT
ADD file:d49890823c4e8287f936eec210400575f79c20f14f048017368faed0584841a6 in / 
# Wed, 30 Jun 2021 17:23:41 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:40:57 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:43:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 30 Jun 2021 17:43:12 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:43:12 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 17:43:13 GMT
ENV JAVA_VERSION=17-ea+28
# Wed, 30 Jun 2021 17:43:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/28/GPL/openjdk-17-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='29f489da387fdabce2ebfbb74f474c424ed9c92380783da511d8ab1ed5dee912'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/28/GPL/openjdk-17-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='60752f6f44e478db934f4dc4b9a7cb715387ae964fb353e469dd986a5aeaf92b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 30 Jun 2021 17:43:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9660ffb7976c51eb47b4425f6bb95173c170f4fcc442a2bb2b6ba7bf154f6fc8`  
		Last Modified: Wed, 30 Jun 2021 17:25:00 GMT  
		Size: 42.2 MB (42179226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f8b4ca74ea5f238671d4c7981ca7c99e6c70d3fcd8d4d0596ccdf6b8329dbe`  
		Last Modified: Wed, 30 Jun 2021 17:50:04 GMT  
		Size: 13.4 MB (13391447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da92b3bc8acc347b4c113e7f363ec20753cc078e7d01c51b81e9d89543008cc`  
		Last Modified: Wed, 30 Jun 2021 17:51:21 GMT  
		Size: 187.1 MB (187111521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:e8d87ffa883a55864a8b8c205b2ff28ee5b3e57fa10f4df1391cad8cc7d1abd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.1 MB (242138643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274d588d701f9305efe12256f22ac2a05c37273f8f509c43838c555e41f4f85d`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 16:40:33 GMT
ADD file:c33580f17660c9afa2637bda7e6cf34d631535b13ffc1535bb21cfb0ab7bdb5c in / 
# Wed, 30 Jun 2021 16:40:33 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:08:45 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:09:42 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 30 Jun 2021 17:09:42 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:09:43 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 17:09:43 GMT
ENV JAVA_VERSION=17-ea+28
# Wed, 30 Jun 2021 17:09:52 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/28/GPL/openjdk-17-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='29f489da387fdabce2ebfbb74f474c424ed9c92380783da511d8ab1ed5dee912'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/28/GPL/openjdk-17-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='60752f6f44e478db934f4dc4b9a7cb715387ae964fb353e469dd986a5aeaf92b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 30 Jun 2021 17:09:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e02c40d2e97c148eec83200018cd774bcf09562d984b2237577a0bebd5900481`  
		Last Modified: Wed, 30 Jun 2021 16:41:47 GMT  
		Size: 42.0 MB (42045297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c341a81c74999386f57f0e8e08448131a5297ce89816bbfe58e5d804b6e1384`  
		Last Modified: Wed, 30 Jun 2021 17:21:19 GMT  
		Size: 14.2 MB (14179251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeb872558aabedcdaa6adbd459087dad5be3d43f9e1f8644a88a49bf7d146c1`  
		Last Modified: Wed, 30 Jun 2021 17:22:58 GMT  
		Size: 185.9 MB (185914095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-jdk` - windows version 10.0.17763.1999; amd64

```console
$ docker pull openjdk@sha256:1653054844354edf69d1658584ac14a0814af096d7ec25901b94ddd87107a5c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2824680179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ebca9b9cb5370ad4966c6bf13f5690f95b6511ffbcb4efce7abf20c05c9fcd`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 16:45:14 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Jun 2021 16:45:17 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 09 Jun 2021 16:45:47 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 26 Jun 2021 01:30:05 GMT
ENV JAVA_VERSION=17-ea+28
# Sat, 26 Jun 2021 01:30:08 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/28/GPL/openjdk-17-ea+28_windows-x64_bin.zip
# Sat, 26 Jun 2021 01:30:10 GMT
ENV JAVA_SHA256=82fbbd1a079675fe31c09ac43f54c2d203d92272e6e0160cee6f719f1e7da1ae
# Sat, 26 Jun 2021 01:31:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 26 Jun 2021 01:31:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4f84ebe44976489de74231891a3bceaf046cdaf5d963f8d9785d418863bfd7`  
		Last Modified: Wed, 09 Jun 2021 17:24:02 GMT  
		Size: 352.1 KB (352057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580f726be9e9223f5fbe72ec77a450134c84e6501882795e77ae88e34b87949a`  
		Last Modified: Wed, 09 Jun 2021 17:24:01 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6098af536049b2e7b8c27707faac52e3ac75b37f3ba29e5543ea2f149e8ce501`  
		Last Modified: Wed, 09 Jun 2021 17:24:01 GMT  
		Size: 310.1 KB (310100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3b0e6f0a186ee8349669783497217e22003710ff3188546fc87586e190c72f`  
		Last Modified: Sat, 26 Jun 2021 01:41:44 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a653372907bce4ba5dd08cf27d3af90e510f6a444d75556bb633087a8753b1`  
		Last Modified: Sat, 26 Jun 2021 01:41:44 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8b4e611adfea4a4a67bf1feac30fd5ba2ea3a936ba59601b7ca99ecac07f86`  
		Last Modified: Sat, 26 Jun 2021 01:41:44 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794e62f26e5d17e2a56114eb986598f498271764cd8bba481725414fa55ad114`  
		Last Modified: Sat, 26 Jun 2021 01:42:04 GMT  
		Size: 182.4 MB (182424431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e864e446d24978165f95d6a2d9fbf11802f9af65a50c8928f6f713cdc843222`  
		Last Modified: Sat, 26 Jun 2021 01:41:44 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-jdk` - windows version 10.0.14393.4467; amd64

```console
$ docker pull openjdk@sha256:954b7b6bfa3fed2f5ff457c0d4276f2b19c092527190b757f85ca8e570e49ab5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6448750081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520849d9508be3efd09d81f43a12109b8718e8988e5048627990ce9fb972ecb5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 16:48:43 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Jun 2021 16:48:45 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 09 Jun 2021 16:50:13 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 26 Jun 2021 01:31:34 GMT
ENV JAVA_VERSION=17-ea+28
# Sat, 26 Jun 2021 01:31:37 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/28/GPL/openjdk-17-ea+28_windows-x64_bin.zip
# Sat, 26 Jun 2021 01:31:40 GMT
ENV JAVA_SHA256=82fbbd1a079675fe31c09ac43f54c2d203d92272e6e0160cee6f719f1e7da1ae
# Sat, 26 Jun 2021 01:33:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 26 Jun 2021 01:33:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030344af2a85aa48f4c1eb2866fe22830344ab5752d72cb3dec80e7234b68523`  
		Last Modified: Wed, 09 Jun 2021 17:24:45 GMT  
		Size: 343.9 KB (343868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41cbdbabbc3dc8df16e40d2439f3f57faa24b3d6cfde3f6407dd05c7dc09845`  
		Last Modified: Wed, 09 Jun 2021 17:24:44 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5c2af984d599f4fe5db096a3ad4bc6ea4d953344734d21db1d9a3a3b2ce0b2`  
		Last Modified: Wed, 09 Jun 2021 17:24:44 GMT  
		Size: 295.5 KB (295512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71c889c245c34ba6d6faf968c8044b2c24b7ad0a1a040421c8bc2e6f4d971b2`  
		Last Modified: Sat, 26 Jun 2021 01:42:25 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659d508af9a96c267c986b40de229ab55f86888e6f785fd25337ff024ce9f5c7`  
		Last Modified: Sat, 26 Jun 2021 01:42:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5834cd86e1d633191c8cf0061be05cf0f0bb716969f6dc258b0269ad7b018f78`  
		Last Modified: Sat, 26 Jun 2021 01:42:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c6a4efdd41bb94d396854d7cdc65c00d4d927561ff50dd9e32d223695ad04`  
		Last Modified: Sat, 26 Jun 2021 01:42:44 GMT  
		Size: 182.4 MB (182374890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbe13528f2e3b6457ab088dce967eeef53eac87277349ee89ebc26e370356a1`  
		Last Modified: Sat, 26 Jun 2021 01:42:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
