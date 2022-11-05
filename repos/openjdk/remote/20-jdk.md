## `openjdk:20-jdk`

```console
$ docker pull openjdk@sha256:64e82566379844668b89f15e9cf607771a04cec46d78f60c2d2787fac9faf3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1129; amd64
	-	windows version 10.0.17763.3532; amd64

### `openjdk:20-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:c9f96746587ab2b5e04b63d44802a77d9b09b45f7a6ecaeff0d08b5a7de11f96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.1 MB (251080465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1af5be66eba2d5f0cbce0c70c69e214a35e93c14d55418b72b461aa65ae00138`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:19:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:19:44 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Sat, 05 Nov 2022 02:19:44 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 02:19:44 GMT
ENV LANG=C.UTF-8
# Sat, 05 Nov 2022 02:19:44 GMT
ENV JAVA_VERSION=20-ea+21
# Sat, 05 Nov 2022 02:19:55 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/21/GPL/openjdk-20-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='7cb7563541c5a384bcdac868744a5faeea2fa8bd68f5e0f2ee03ffa27d1f9d56'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/21/GPL/openjdk-20-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='f63aac8e75f05ed5212a7365be1007c6995c7f10d6f9308f8894634455d9a0f4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Nov 2022 02:19:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab968c9bcaf076780e21bb249a61cd5dfda4716508c17678f3082057a3c9b8f8`  
		Last Modified: Sat, 05 Nov 2022 02:23:30 GMT  
		Size: 12.2 MB (12229784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cda77a5c28cd28b3120fe1b005e8d2f751900832268b97cbd4fe44c30c69f5`  
		Last Modified: Sat, 05 Nov 2022 02:23:44 GMT  
		Size: 198.3 MB (198269764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:6a3f5cd14a732c5126edd8281c561dd0ba89e65c81b020ec412536cc42f9dae4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.3 MB (249294363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd05d8a5608bce52cf940e6fa15739abbf77e40bb9d3dc77a651dcdc939e9945`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Nov 2022 22:50:08 GMT
ADD file:efa6454225ba5be177493364c69d425968d42231b708b5d492a41f9ab14d64f4 in / 
# Fri, 04 Nov 2022 22:50:08 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 00:48:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 05 Nov 2022 00:48:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Sat, 05 Nov 2022 00:48:43 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 00:48:43 GMT
ENV LANG=C.UTF-8
# Sat, 05 Nov 2022 00:48:44 GMT
ENV JAVA_VERSION=20-ea+21
# Sat, 05 Nov 2022 00:48:51 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/21/GPL/openjdk-20-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='7cb7563541c5a384bcdac868744a5faeea2fa8bd68f5e0f2ee03ffa27d1f9d56'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/21/GPL/openjdk-20-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='f63aac8e75f05ed5212a7365be1007c6995c7f10d6f9308f8894634455d9a0f4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Nov 2022 00:48:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a13cd8cb50ab4c8c5cb15a9929fa5faf1b7833f87c827551a9a54e84789b1e0b`  
		Last Modified: Fri, 04 Nov 2022 22:51:35 GMT  
		Size: 39.4 MB (39401738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2b575a486b4b7df2602a19466f69783be33126ccdea7a939dbef7ecc85a7c7`  
		Last Modified: Sat, 05 Nov 2022 00:53:50 GMT  
		Size: 13.0 MB (13049666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3b46aefd64f29e78c2332b28f4315f522f7504164fa5a049f73e1e93974b52`  
		Last Modified: Sat, 05 Nov 2022 00:54:01 GMT  
		Size: 196.8 MB (196842959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk` - windows version 10.0.20348.1129; amd64

```console
$ docker pull openjdk@sha256:5db70746105e48172a1bb521e9f22d191033d80b8e983e2cad6ae7f0426b9bef
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668938661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712913cdccce41e0d75b9f3b4b837b43aeed5f195daac23c8c079e31840ddc09`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:39:02 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:39:03 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 12 Oct 2022 16:39:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 27 Oct 2022 21:15:05 GMT
ENV JAVA_VERSION=20-ea+21
# Thu, 27 Oct 2022 21:15:09 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/21/GPL/openjdk-20-ea+21_windows-x64_bin.zip
# Thu, 27 Oct 2022 21:15:10 GMT
ENV JAVA_SHA256=30b32b392a540133857358ce96a76184de53add58ce72fea92a8ba623bb80835
# Thu, 27 Oct 2022 21:16:19 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 27 Oct 2022 21:16:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cbc434576dbff410ee0aa4228c6f0fa038ee64fba58d8b81df98ab5bd3e8e5`  
		Last Modified: Wed, 12 Oct 2022 16:51:49 GMT  
		Size: 609.6 KB (609572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d05c1a9fc44de33350221b30e908eaeae6d05eba0fe481490fe562a59dc8fc`  
		Last Modified: Wed, 12 Oct 2022 16:51:49 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71e1244e1a09ac39ec09321d2cf652a948c02d0366d860e30695700811edad3`  
		Last Modified: Wed, 12 Oct 2022 16:51:49 GMT  
		Size: 524.9 KB (524924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75db809d83b7fdb14f27f2ca9c42a3e68baf518c73e335fae92aa8e622f7a68e`  
		Last Modified: Thu, 27 Oct 2022 21:21:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8214597138a714f72a361340b307e2ab5e92d89ba4ae93e3893e160ad9930348`  
		Last Modified: Thu, 27 Oct 2022 21:21:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5451b7bc47721968dc4e919211f2cda9a44ff0552bec06fe6d6575ee54719d79`  
		Last Modified: Thu, 27 Oct 2022 21:21:29 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41a1ab692e085a1732e6b10521a8b9deb448cebbfcff126fde7b9dac912d755`  
		Last Modified: Thu, 27 Oct 2022 21:21:49 GMT  
		Size: 193.8 MB (193769315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c723466059fa0232fb887fff6ee8118ed6c6a0eafb4fbf12947c4d017dfb9e`  
		Last Modified: Thu, 27 Oct 2022 21:21:29 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk` - windows version 10.0.17763.3532; amd64

```console
$ docker pull openjdk@sha256:927ecc0cc2a443b55bc03b1f611da1cdf211d80d89a72347dc06435cc0445f23
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2967743835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0cc5ca2758b4d880ceec1684302a26868be42f9084536c553a983f6995a63f1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:41:21 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:41:22 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 12 Oct 2022 16:42:14 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 27 Oct 2022 21:16:33 GMT
ENV JAVA_VERSION=20-ea+21
# Thu, 27 Oct 2022 21:16:34 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/21/GPL/openjdk-20-ea+21_windows-x64_bin.zip
# Thu, 27 Oct 2022 21:16:35 GMT
ENV JAVA_SHA256=30b32b392a540133857358ce96a76184de53add58ce72fea92a8ba623bb80835
# Thu, 27 Oct 2022 21:18:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 27 Oct 2022 21:18:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891dd6ec2fa598da717e21a05ad77857caf95e46fc5861ed7e79aab507e9fd11`  
		Last Modified: Wed, 12 Oct 2022 16:52:29 GMT  
		Size: 347.9 KB (347943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e673f50a0247a96d4f10904fad919663c061d29e5445b3531a1eb3a227b99657`  
		Last Modified: Wed, 12 Oct 2022 16:52:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f4cce28740d1d55be90dac59ca06df221cfd3100dd82e1eedd5a929a54b2cf`  
		Last Modified: Wed, 12 Oct 2022 16:52:29 GMT  
		Size: 310.8 KB (310762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5008a4a848866c7b61beabdffe4458a85bcf4ca78790036bf38043cea4e81adf`  
		Last Modified: Thu, 27 Oct 2022 21:22:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9724704f9d8b9533488991d56365be7e4bb0401440a00afcaff8bd2e28a85ef4`  
		Last Modified: Thu, 27 Oct 2022 21:22:12 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69db01cb096dc1b53d04a38914ba93f887a759d04265fffe86f311a2721fba9`  
		Last Modified: Thu, 27 Oct 2022 21:22:12 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd18020b59c9e1da04eaf4337aea39a255e3c531b5e56db97555b035de7f8d5`  
		Last Modified: Thu, 27 Oct 2022 21:22:33 GMT  
		Size: 193.6 MB (193578268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc41ee66fab9b6f79bc7a20b10327425385035ec2772912db41404b6ca2fee3`  
		Last Modified: Thu, 27 Oct 2022 21:22:12 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
