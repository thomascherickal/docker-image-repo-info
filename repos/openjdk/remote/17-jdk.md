## `openjdk:17-jdk`

```console
$ docker pull openjdk@sha256:160c5e49408a84fb57ad7110eb6469df7d6480b682f03307d1ad70c91460aac3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `openjdk:17-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:d6f0c745adab26c02ae54304080a4ebab569475df927234f9b91a299718f3a04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.7 MB (242704481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eb3e3089b9e31c60a05f3ca44d37c32e50c57c49396d05be5a3ca659a69afcf`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jul 2021 20:20:57 GMT
ADD file:c830de449b9ecd90e02f56d99e8326701da17970fa314bd7b060fd9a7cf7ac77 in / 
# Mon, 12 Jul 2021 20:20:58 GMT
CMD ["/bin/bash"]
# Mon, 12 Jul 2021 23:33:03 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 12 Jul 2021 23:34:11 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Mon, 12 Jul 2021 23:34:11 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 12 Jul 2021 23:34:12 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jul 2021 23:34:12 GMT
ENV JAVA_VERSION=17-ea+30
# Mon, 12 Jul 2021 23:35:05 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/30/GPL/openjdk-17-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='527ba5657fb7d9814cdc22d860ab078bfa838e0d821a23a969e4cfd1ec616024'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/30/GPL/openjdk-17-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='a346c3043a0e636d0cfe0cc722e6e974871f96d777b96f9ec64960bd4dbd0fbd'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 12 Jul 2021 23:35:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c828c776e142cb23ad61c84403bb42deaa97efeda5e2b600df46f7dbd38ec681`  
		Last Modified: Mon, 12 Jul 2021 20:22:25 GMT  
		Size: 42.2 MB (42179737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8846dac42cae4499c0917b5bd5e81c0e6d6fcc5326d50972b3faed7ccdf688b8`  
		Last Modified: Mon, 12 Jul 2021 23:41:34 GMT  
		Size: 13.4 MB (13392657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e77521973d146549c5241e22b9cb5096e657369f92cbd4e0f4245b8ea61741`  
		Last Modified: Mon, 12 Jul 2021 23:44:42 GMT  
		Size: 187.1 MB (187132087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b8ea3f7642fa58ab8021175ebb70ea8dcb1871ec6b4977c101b7ceb09f770977
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.2 MB (242190317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36c32ff91cff84e199d9c272ac845b4922e2a9c69983cc7e1100fc414f5b211d`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jul 2021 20:40:32 GMT
ADD file:a184ed870dc7a85028f7ba3bd0cf3820d6f1b94ac4cea1ac94ca48c786901041 in / 
# Mon, 12 Jul 2021 20:40:33 GMT
CMD ["/bin/bash"]
# Mon, 12 Jul 2021 21:03:05 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 12 Jul 2021 21:04:07 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Mon, 12 Jul 2021 21:04:07 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 12 Jul 2021 21:04:07 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jul 2021 00:14:20 GMT
ENV JAVA_VERSION=17-ea+30
# Tue, 13 Jul 2021 00:14:29 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/30/GPL/openjdk-17-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='527ba5657fb7d9814cdc22d860ab078bfa838e0d821a23a969e4cfd1ec616024'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/30/GPL/openjdk-17-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='a346c3043a0e636d0cfe0cc722e6e974871f96d777b96f9ec64960bd4dbd0fbd'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Jul 2021 00:14:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6186b25cabd91cbdd2c6bf65b0c5ef261f52719e7c6c4d6252e7082b7a51b42e`  
		Last Modified: Mon, 12 Jul 2021 20:41:48 GMT  
		Size: 42.1 MB (42072715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8304774b066b61c2ae3dc6de204cb3d384a726b9376d301afc654577b50a9c0`  
		Last Modified: Mon, 12 Jul 2021 21:15:51 GMT  
		Size: 14.2 MB (14170180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a849297b0ab9e13b8758c79e109f0f1d440d94a2b0591bb3748c8d2a32f3539`  
		Last Modified: Tue, 13 Jul 2021 00:30:23 GMT  
		Size: 185.9 MB (185947422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-jdk` - windows version 10.0.17763.1999; amd64

```console
$ docker pull openjdk@sha256:72eec99728be65f79dbd6a55de18ff3c7889994a5163787b5b1e9b856a089c73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2824695226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acc4c67e8864ea4bf92ae44d522b46f8e1ef1306734aaa090cdf9b86d51e0dd9`
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
# Fri, 02 Jul 2021 19:32:26 GMT
ENV JAVA_VERSION=17-ea+29
# Fri, 02 Jul 2021 19:32:28 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/29/GPL/openjdk-17-ea+29_windows-x64_bin.zip
# Fri, 02 Jul 2021 19:32:31 GMT
ENV JAVA_SHA256=48240d2cb5b81a0cf2b85e8ddbc972daaefd1977c4336ca68fcbd3565a20d49a
# Fri, 02 Jul 2021 19:33:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 02 Jul 2021 19:34:01 GMT
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
	-	`sha256:20c0bcf92c506a1229487c91e74a2643d72a07e52e24ccbb22a6e31e7c548898`  
		Last Modified: Fri, 02 Jul 2021 19:43:27 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19444f4c7baa0d9a9d3dcc86692a676be6323b098e0b60646181bcd3ed48af1`  
		Last Modified: Fri, 02 Jul 2021 19:43:27 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0198f03bee56fa775d93109c901afba7de22e35e67c70cb2e3dd82445ae357`  
		Last Modified: Fri, 02 Jul 2021 19:43:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c820f037a08f349cde91eb472b1406d95f4c1dc715784a2d54aec2855929248`  
		Last Modified: Fri, 02 Jul 2021 19:43:46 GMT  
		Size: 182.4 MB (182439507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1332240a7899298b5b7da0687ef374dc5355a3a457bb8f644bd6af51a3f28c8`  
		Last Modified: Fri, 02 Jul 2021 19:43:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-jdk` - windows version 10.0.14393.4467; amd64

```console
$ docker pull openjdk@sha256:183a46ec99e35706715de77ee3b7302a3e8f85eb7a1fa2365f92aa84fadca8f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6448771401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ee1f9d4fb4953e0757b9ce141734ada617035091364d4d62a34eaaf480d261`
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
# Fri, 02 Jul 2021 19:34:11 GMT
ENV JAVA_VERSION=17-ea+29
# Fri, 02 Jul 2021 19:34:13 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/29/GPL/openjdk-17-ea+29_windows-x64_bin.zip
# Fri, 02 Jul 2021 19:34:16 GMT
ENV JAVA_SHA256=48240d2cb5b81a0cf2b85e8ddbc972daaefd1977c4336ca68fcbd3565a20d49a
# Fri, 02 Jul 2021 19:36:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 02 Jul 2021 19:36:16 GMT
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
	-	`sha256:a0101707cd931ce34c5142133a171a609e718b7536df60170ff6a028e17632cb`  
		Last Modified: Fri, 02 Jul 2021 19:44:07 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0993c8d7743626f9c1081084d1974a40e18e40c733acb56d7780041c30953a1`  
		Last Modified: Fri, 02 Jul 2021 19:44:07 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee15d7ca3bc4d4a0538a9916c44fd5eaa7a1b1946efaa7a055428b98044f355`  
		Last Modified: Fri, 02 Jul 2021 19:44:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919bd243b1224636c7736a90ee594a70423babf64ad830cd0f2bd629cef0ade4`  
		Last Modified: Fri, 02 Jul 2021 19:44:25 GMT  
		Size: 182.4 MB (182396218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb59d59bb406dd3809cd1406af42201c7b3d7ed0474edaf1ae51edeae9df821`  
		Last Modified: Fri, 02 Jul 2021 19:44:07 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
