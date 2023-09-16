## `openjdk:22-ea-15-jdk`

```console
$ docker pull openjdk@sha256:91dc62334874af5d37dd312776763d32fa72c6b6ed3d2cabcab19d647c1b0308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1970; amd64
	-	windows version 10.0.17763.4851; amd64

### `openjdk:22-ea-15-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:c6f0b3a2a975af975495028a2243949ee877f57c3f55879bd4729441569e114c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.0 MB (264991966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc216b769f1faa6c9fef71de64826c86138c2db673424537f93a588483b3bbb0`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 16 Sep 2023 02:40:54 GMT
ADD file:1632d5b9918ff63c9e38191b65ad8e6f1e0eb5c2ef274cce4f50534bba2f7493 in / 
# Sat, 16 Sep 2023 02:40:55 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:53:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 16 Sep 2023 02:53:11 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Sat, 16 Sep 2023 02:53:11 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Sep 2023 02:53:11 GMT
ENV LANG=C.UTF-8
# Sat, 16 Sep 2023 02:53:11 GMT
ENV JAVA_VERSION=22-ea+15
# Sat, 16 Sep 2023 02:53:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/15/GPL/openjdk-22-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='86b3ab4e12d302e039dc65fc4700ffd572d072d6d822c983a6d74b569b9186ef'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/15/GPL/openjdk-22-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='6c680f4dc89b64fbe5cfcf7b12f232e31737112a8801ac594416c21e4b04c892'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Sep 2023 02:53:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bc377bce3181aab0e51009b13b6a6890e49c64e7bf6ab7fa12dce86a95c88bd4`  
		Last Modified: Sat, 16 Sep 2023 02:42:29 GMT  
		Size: 44.9 MB (44911063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fe7d94225755f280f5249e52cf0633729ae0585805f1912428007f164e1d7e`  
		Last Modified: Sat, 16 Sep 2023 02:54:54 GMT  
		Size: 15.0 MB (15001921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4a746de42f6c684ace484cf55415b8c197bc4e7ea2c033a58f67a0600ce0c9`  
		Last Modified: Sat, 16 Sep 2023 02:55:07 GMT  
		Size: 205.1 MB (205078982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-15-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:36238665f9adf15a79a7c1101e2fc49395a5dddf399f31cce4c0bc6f4bea4009
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262697640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888e8f842cf46d61278010f96579727931e7333771949470fdf7b098258b82ee`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 16 Sep 2023 02:21:42 GMT
ADD file:c1b7bfaf11bf64b9c1b24345749a98cbd3f593162ea942e12b15c6f2110c1e94 in / 
# Sat, 16 Sep 2023 02:21:43 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:49:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 16 Sep 2023 02:49:47 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Sat, 16 Sep 2023 02:49:47 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Sep 2023 02:49:47 GMT
ENV LANG=C.UTF-8
# Sat, 16 Sep 2023 02:49:47 GMT
ENV JAVA_VERSION=22-ea+15
# Sat, 16 Sep 2023 02:49:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/15/GPL/openjdk-22-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='86b3ab4e12d302e039dc65fc4700ffd572d072d6d822c983a6d74b569b9186ef'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/15/GPL/openjdk-22-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='6c680f4dc89b64fbe5cfcf7b12f232e31737112a8801ac594416c21e4b04c892'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Sep 2023 02:50:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d095360c6402749d9f7a3d7b7cdd417f27e41419f8027f4704ab00d0dd8ae7ee`  
		Last Modified: Sat, 16 Sep 2023 02:22:42 GMT  
		Size: 43.6 MB (43630964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7548ed69b34282ed3935dd421a868025a61827eb4d197bcee64f8ae913c858ad`  
		Last Modified: Sat, 16 Sep 2023 02:51:22 GMT  
		Size: 15.7 MB (15675185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1fef6e96a1b52fba3ce172e634ed96d0a9a630966a5bf6d7ba3cc07ea78c46`  
		Last Modified: Sat, 16 Sep 2023 02:51:33 GMT  
		Size: 203.4 MB (203391491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-15-jdk` - windows version 10.0.20348.1970; amd64

```console
$ docker pull openjdk@sha256:7ee9d7dc953abd3765e3566267120706d5f2fa0e3c8af592f6839f9596b29486
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037432064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96565ad68623668290c29b9f872363ca12737c6ac90c185a9a2a66229947b203`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:14:15 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Sep 2023 05:14:16 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 13 Sep 2023 05:14:36 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 14 Sep 2023 22:30:22 GMT
ENV JAVA_VERSION=22-ea+15
# Thu, 14 Sep 2023 22:30:23 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/15/GPL/openjdk-22-ea+15_windows-x64_bin.zip
# Thu, 14 Sep 2023 22:30:24 GMT
ENV JAVA_SHA256=9adc0c416a6856e721ca26724a9a16efca073f67520c59ff43508bc3eb6deabd
# Thu, 14 Sep 2023 22:31:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 14 Sep 2023 22:31:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b411249ef1c74d6763984f0b9b085ac311c6e49aba35a7dbbc1d42264a11ba`  
		Last Modified: Wed, 13 Sep 2023 05:25:31 GMT  
		Size: 462.9 KB (462878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d5d90c5ae40ed0401706ba6915059213a0cc520cc862f8fdbff4e582cbc835`  
		Last Modified: Wed, 13 Sep 2023 05:25:31 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b84e7bb658094bff788d92f8ca930570e83805ce31d072d4c675acbef78b62b`  
		Last Modified: Wed, 13 Sep 2023 05:25:31 GMT  
		Size: 274.9 KB (274889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b547342e3406ab181e2fdd2e8aaac0ed1fc98d4e072e9de8e86d3ad3fa73c7f`  
		Last Modified: Thu, 14 Sep 2023 22:35:15 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50be428010acb12e1c8535826de0c25e898652d67b96a0e14538bf3276761b6`  
		Last Modified: Thu, 14 Sep 2023 22:35:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3f8a93bb81f41a6e7216560a405ef5898b2fdfcbd0ef403ac51518ffebdc4a`  
		Last Modified: Thu, 14 Sep 2023 22:35:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681b01dd013c8eafa17ad2c175258dde049c16829f0f350714e091bd7a7f40f7`  
		Last Modified: Thu, 14 Sep 2023 22:35:35 GMT  
		Size: 199.4 MB (199411732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce495c3faee01a0c248535e4e607f529d18d279802dfe6109108513a23f1650`  
		Last Modified: Thu, 14 Sep 2023 22:35:15 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-15-jdk` - windows version 10.0.17763.4851; amd64

```console
$ docker pull openjdk@sha256:b6803e47ecc74084dde6ae4289ef8e683d0a15e8345e853813760a2f50d1c702
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2216347787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f43313cb15250f36171b76f602e0084d86fe97f6783a3a2946ae2e1cf6a9e10`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:16:37 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Sep 2023 05:16:38 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 13 Sep 2023 05:17:33 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 14 Sep 2023 22:31:36 GMT
ENV JAVA_VERSION=22-ea+15
# Thu, 14 Sep 2023 22:31:37 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/15/GPL/openjdk-22-ea+15_windows-x64_bin.zip
# Thu, 14 Sep 2023 22:31:37 GMT
ENV JAVA_SHA256=9adc0c416a6856e721ca26724a9a16efca073f67520c59ff43508bc3eb6deabd
# Thu, 14 Sep 2023 22:33:12 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 14 Sep 2023 22:33:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da151b70a7f82a6d6963a3317229ba06177114b9d44cd362e90207d42aa4d828`  
		Last Modified: Wed, 13 Sep 2023 05:26:10 GMT  
		Size: 255.5 KB (255460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f8ba7984984551020a40f5b8881b3c1fb035e9785ba3bdbae07f7c770a4f6d`  
		Last Modified: Wed, 13 Sep 2023 05:26:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0c6f3841f682fcfe5bcc0fb248fac7844337b14dd92db7132434ac8133685`  
		Last Modified: Wed, 13 Sep 2023 05:26:09 GMT  
		Size: 216.8 KB (216765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ec3b598e4b70a2304c7138bd42ebfc00f7e1aa2e808dfc86f84365f2ae7c85`  
		Last Modified: Thu, 14 Sep 2023 22:36:00 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1974849b7e141d4a22eb298608352c8fad1787ca6aebc9bb154bee8de3c8030`  
		Last Modified: Thu, 14 Sep 2023 22:36:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd98b8780af47ea6af12db2ef434965ee4a710fa5f07d447ce5a956dd5d700a`  
		Last Modified: Thu, 14 Sep 2023 22:36:00 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9c6e44d27f54b7689e2423db78556fc71d67983f5b8cdeea958abe90c30d61`  
		Last Modified: Thu, 14 Sep 2023 22:36:20 GMT  
		Size: 199.5 MB (199537286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9500e885b8eff524d4481f853b1619a06c38bff6832910e77d009b1dfe18fd`  
		Last Modified: Thu, 14 Sep 2023 22:36:00 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
