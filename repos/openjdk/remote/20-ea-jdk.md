## `openjdk:20-ea-jdk`

```console
$ docker pull openjdk@sha256:7f36bffee7c2a2efd67d9cb4f79c87b597ac5bf2071fb2490a09af3310094eaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1249; amd64
	-	windows version 10.0.17763.3650; amd64

### `openjdk:20-ea-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:b4ee01ca5c7925026250fb6971709a16f311b49e3717029b230f2da591897a1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.0 MB (251042264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bab8184f21de35719e60326e04a9acee05af4b203e6c1f94d7d40be566b1f75`
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
# Fri, 11 Nov 2022 00:55:46 GMT
ENV JAVA_VERSION=20-ea+23
# Fri, 11 Nov 2022 00:55:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Nov 2022 00:56:00 GMT
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
	-	`sha256:aaf6385da395568951fb61497c938edf2fd6a188ddde7d7db5494360a2511b5e`  
		Last Modified: Fri, 11 Nov 2022 01:00:08 GMT  
		Size: 198.2 MB (198231563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:9d7f15521d7f7db2ea9638d20e3777aabca3f3600d7dfc59fae3b64d59aff39d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249243808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7a66440227e5c03e2cd4b6f21004555d62c856096992422f43ec601bc655e66`
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
# Fri, 11 Nov 2022 11:33:30 GMT
ENV JAVA_VERSION=20-ea+23
# Fri, 11 Nov 2022 11:33:38 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Nov 2022 11:33:40 GMT
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
	-	`sha256:42a80be26959592a5861c6f1306a65cf2b59f4b8127eaaa22c99a4e74ed04281`  
		Last Modified: Fri, 11 Nov 2022 11:37:55 GMT  
		Size: 196.8 MB (196792404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk` - windows version 10.0.20348.1249; amd64

```console
$ docker pull openjdk@sha256:cafd59cc3f41283071329bee3e39b660f70989aef15060da222c8aac3f5bf1bb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2676665743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:418117389a8645125cb95e4f646018e5fb0a8ad65762d0c101737b8ce476e01d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 17:20:09 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Nov 2022 17:20:10 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 09 Nov 2022 17:20:37 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 10 Nov 2022 22:16:21 GMT
ENV JAVA_VERSION=20-ea+23
# Thu, 10 Nov 2022 22:16:23 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_windows-x64_bin.zip
# Thu, 10 Nov 2022 22:16:24 GMT
ENV JAVA_SHA256=ccb9c93fb62e650814b144e6097463b00e166366469ddcd2e87f3a2ae5d05771
# Thu, 10 Nov 2022 22:17:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 10 Nov 2022 22:17:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f5ce72a05e01b629001eb0ff2b493ddf6cd8e3c7a836607dc83cfbbec299b3`  
		Last Modified: Wed, 09 Nov 2022 17:35:31 GMT  
		Size: 614.7 KB (614677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766f89a2f9cf276bf435dc9be37e180dfcfc54b750ca8cca41b1e0673eb95abe`  
		Last Modified: Wed, 09 Nov 2022 17:35:30 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3329d7d902a4cde0c4f3848690267bd771e713ccee926c04fc723e62ad0105e8`  
		Last Modified: Wed, 09 Nov 2022 17:35:31 GMT  
		Size: 546.1 KB (546089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3279e0a6f145b97aef1d3469c9d4bdb14c25442ee1d6b3d91cac5be6348cec09`  
		Last Modified: Fri, 11 Nov 2022 01:17:24 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3995c0e83432eabb60a374c2970359ba0f5e8f3c28eb741a26abd7594e41da5`  
		Last Modified: Fri, 11 Nov 2022 01:17:24 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a816493b452fd9278b665061424edeede7d4faed86827c2019b5c06d12c53c97`  
		Last Modified: Fri, 11 Nov 2022 01:17:24 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176c4a524ba640a7264a6214b12e7578bd5f003f8433ac946598b749c510d89c`  
		Last Modified: Fri, 11 Nov 2022 01:17:47 GMT  
		Size: 193.7 MB (193727860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb7d24283be46bdbfea9eadaa371fa1391c1dc049ee4216906b094c5c1f94f4`  
		Last Modified: Fri, 11 Nov 2022 01:17:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk` - windows version 10.0.17763.3650; amd64

```console
$ docker pull openjdk@sha256:6840bd66264d835d84352d9c0c9122735d635590f80f3c091998d3e31031e679
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2972786653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dfb9c3bf4c16a37a21df34e967a0b32077ef590d16f926a015b4e30d7294aae`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 17:23:18 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Nov 2022 17:23:19 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 09 Nov 2022 17:24:31 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 10 Nov 2022 22:17:40 GMT
ENV JAVA_VERSION=20-ea+23
# Thu, 10 Nov 2022 22:17:41 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_windows-x64_bin.zip
# Thu, 10 Nov 2022 22:17:42 GMT
ENV JAVA_SHA256=ccb9c93fb62e650814b144e6097463b00e166366469ddcd2e87f3a2ae5d05771
# Thu, 10 Nov 2022 22:19:48 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 10 Nov 2022 22:19:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c85372c7985a34aa1619da07364507356666af5e2f073a7a04b171c25354b4a`  
		Last Modified: Wed, 09 Nov 2022 17:36:18 GMT  
		Size: 364.8 KB (364807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2c5944c42080bba06b7004a16754ffff768c5ce0b7b3c895891f0f4efe6ef6`  
		Last Modified: Wed, 09 Nov 2022 17:36:17 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e29b6097f3b07473eb77be3c0d8c63285a498161914a045d403afd73a63e73`  
		Last Modified: Wed, 09 Nov 2022 17:36:18 GMT  
		Size: 321.6 KB (321605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd5f18b85739b128a4b65ee89e92b997c2ae174d4623323f84d6807f73ef336`  
		Last Modified: Fri, 11 Nov 2022 01:18:10 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6280f675a3fdbefc9f2e2307cf0c3dc5a447dc1898c57c0e2784cbfb79e00`  
		Last Modified: Fri, 11 Nov 2022 01:18:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9136dcfca1c699ce89c89c290a0ab60a0e32983b4131730b9ae30797eca27dcc`  
		Last Modified: Fri, 11 Nov 2022 01:18:11 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993ffc733ad33179ea9ed64c12ce310d5543768573ceeb7e9850ee63151aedc4`  
		Last Modified: Fri, 11 Nov 2022 01:18:32 GMT  
		Size: 193.5 MB (193504975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679293b5fa6848ef356921e5c2fbfda5f9960802ddbab3237bf275cfafe4ccd2`  
		Last Modified: Fri, 11 Nov 2022 01:18:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
