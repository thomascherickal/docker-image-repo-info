## `openjdk:21-jdk`

```console
$ docker pull openjdk@sha256:f13014cd20d53b4c1dcd5873226bdadf9e35d210f08e9f85ce942cc85d942346
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `openjdk:21-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:f2c33bb04d4126ec8d1eab7f86226b68e9f25058ee510eb25cf72bb5cf97a07e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263022860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a737415ec531faa9f3590c2ffe39a3299fe87acd82cc4c2ea132d2b43afb8e2`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 May 2023 21:20:28 GMT
ADD file:e15c235506d8dd134e69d458a7c0afefef1522e9d0cfb28e3538760ddf032785 in / 
# Wed, 24 May 2023 21:20:29 GMT
CMD ["/bin/bash"]
# Wed, 24 May 2023 21:44:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 24 May 2023 21:44:56 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 24 May 2023 21:44:56 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 May 2023 21:44:56 GMT
ENV LANG=C.UTF-8
# Fri, 26 May 2023 23:05:09 GMT
ENV JAVA_VERSION=21-ea+24
# Fri, 26 May 2023 23:05:20 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='437e740a3ee795a3cf08d6cf5006d03668023151200d5e09ada16d94ef30db22'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='ecabd8a50340461d04d06b8f587bf06c614aed9cb441ee3ff9577e1b10e53035'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 May 2023 23:05:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:90e2fb2facff1c5093f0ebfa9d08fde487930822d9ac278bb2df0195610f1d13`  
		Last Modified: Wed, 24 May 2023 21:21:24 GMT  
		Size: 44.9 MB (44873648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0845850e9baa985b97efc76bed4795ff90eb1249ecf4531667da84d4be1fcdf`  
		Last Modified: Wed, 24 May 2023 21:45:40 GMT  
		Size: 15.0 MB (15010668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee812e754920b3231666f1d458d8aef25c9e75562b5b05c314dd1d9778d52ca`  
		Last Modified: Fri, 26 May 2023 23:07:29 GMT  
		Size: 203.1 MB (203138544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:27f52854c43307c0f923e67f26a1d9f661ac20831b6c724e4de0a6a60eafe279
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261121088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2089cc4b709fb37808e9d16785253780275e1058d570026a03b68e0529e945`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 May 2023 21:44:09 GMT
ADD file:8c6f57a98019c407c59b2adbf7da54536eff3a7ca62c46883bbc60975b39ad04 in / 
# Wed, 24 May 2023 21:44:09 GMT
CMD ["/bin/bash"]
# Wed, 24 May 2023 22:03:14 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 24 May 2023 22:03:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 24 May 2023 22:03:14 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 May 2023 22:03:14 GMT
ENV LANG=C.UTF-8
# Thu, 25 May 2023 23:39:43 GMT
ENV JAVA_VERSION=21-ea+24
# Thu, 25 May 2023 23:39:56 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='437e740a3ee795a3cf08d6cf5006d03668023151200d5e09ada16d94ef30db22'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='ecabd8a50340461d04d06b8f587bf06c614aed9cb441ee3ff9577e1b10e53035'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 25 May 2023 23:39:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0bb308beee4aa3eb768d546b1ee61303d6f190f63bed75dc7f88ecc26018a944`  
		Last Modified: Wed, 24 May 2023 21:44:58 GMT  
		Size: 43.8 MB (43791991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da95086478e81c9f4c37c04e50d244968af554844dd950bcb04b5f0171653f64`  
		Last Modified: Wed, 24 May 2023 22:03:55 GMT  
		Size: 15.9 MB (15852529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c427e1a7c7546fe45ab6f18696b7bf1e8173249c96d70f910136d2f0663221`  
		Last Modified: Thu, 25 May 2023 23:42:01 GMT  
		Size: 201.5 MB (201476568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk` - windows version 10.0.20348.1726; amd64

```console
$ docker pull openjdk@sha256:287367fbe875baefa760ee4e1c39358faf875d594ba7d66995b6bf3806379e70
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1973332703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d69e1271131032e07867d7b1c528255a1ca58dbd8fe264156db8cc0e2d77c59`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 02:50:46 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 May 2023 02:50:50 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 10 May 2023 02:51:20 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 26 May 2023 00:15:18 GMT
ENV JAVA_VERSION=21-ea+24
# Fri, 26 May 2023 00:15:19 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_windows-x64_bin.zip
# Fri, 26 May 2023 00:15:20 GMT
ENV JAVA_SHA256=94a6c75c97d125c5c258fce73749b367c9ee4791ce77d625585e5ac2acdae6e8
# Fri, 26 May 2023 00:16:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 26 May 2023 00:16:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6500851308f2a80744cfa1cca578e46041bad797f47ea2d8c83f894349fac438`  
		Last Modified: Wed, 10 May 2023 03:00:03 GMT  
		Size: 448.7 KB (448735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d15d3ceb58f655a9b9e1310abf5e4a03194602c97d6cbdfa450b22ffbc6d0f`  
		Last Modified: Wed, 10 May 2023 03:00:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74b424d7445673b30f720a5569aad1a4050cf8a0ad3c7ac1abe1f0576007898`  
		Last Modified: Wed, 10 May 2023 03:00:02 GMT  
		Size: 262.6 KB (262606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce04de762bfcdb3a0c0050cd5b3d2c3e2244338aa5b052c52a12944697ff18e`  
		Last Modified: Fri, 26 May 2023 00:19:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e9b690083212b12cc0c3ec504653a1ae94e7ca0887a7cc306920ad38c0fc44`  
		Last Modified: Fri, 26 May 2023 00:19:33 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b553a237a1e4bed24be9454257bc59ced397cc4c74536def0515a70f66c3f4cc`  
		Last Modified: Fri, 26 May 2023 00:19:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019cf3b876d046a7c30ceebf43537679c0c904138b5e8fa0c7c3d9db99decac2`  
		Last Modified: Fri, 26 May 2023 00:19:52 GMT  
		Size: 197.6 MB (197631390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e9f0b0f74cc56c16f332e74446af69811e603d096cb74c4a76b4d35f4b2f72`  
		Last Modified: Fri, 26 May 2023 00:19:33 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk` - windows version 10.0.17763.4377; amd64

```console
$ docker pull openjdk@sha256:897b875e1ee62dbfb736482e07d489cb93a57928516f7e1b50ed6539745e6892
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2270378646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fad5bc3f998f8ae2723c9b794cd828cd2b2015f2da7021bbd3ceb0961f03f39b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 02:54:18 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 May 2023 02:54:19 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 10 May 2023 02:55:54 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 26 May 2023 00:16:20 GMT
ENV JAVA_VERSION=21-ea+24
# Fri, 26 May 2023 00:16:21 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_windows-x64_bin.zip
# Fri, 26 May 2023 00:16:22 GMT
ENV JAVA_SHA256=94a6c75c97d125c5c258fce73749b367c9ee4791ce77d625585e5ac2acdae6e8
# Fri, 26 May 2023 00:17:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 26 May 2023 00:18:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8712378a27a3538d7991a50dcb72abb565959575008a538c012500547b6acf3a`  
		Last Modified: Wed, 10 May 2023 03:00:47 GMT  
		Size: 441.2 KB (441178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34b75cb4c34981b4a471f423e801ccecb0e509ef934ebed87377603d134a0b0`  
		Last Modified: Wed, 10 May 2023 03:00:46 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0267ca94f1356d921f0a3b30e5336c9c1c0604b0f3cb81963ab715ba48ff81`  
		Last Modified: Wed, 10 May 2023 03:00:47 GMT  
		Size: 259.9 KB (259927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c9a824d0f58905ef61ad7aaa689ea71fba4274b547d627861d6f8317b62b93`  
		Last Modified: Fri, 26 May 2023 00:20:14 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e5e6363fa5c53fc642e857d92949afc11ccd0d9898fd5ebf135ac62dbcfe4c`  
		Last Modified: Fri, 26 May 2023 00:20:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a34edc4ee0405aaa415ff2a0029a833bfc167f51000c9fa972591a6125442d`  
		Last Modified: Fri, 26 May 2023 00:20:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945b85bf68e6a983e9ab05789af2406814864d3005b7eb146d6f2b4cae8f8d6f`  
		Last Modified: Fri, 26 May 2023 00:20:33 GMT  
		Size: 197.6 MB (197633818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad29b8a849de15efff218d4e7fb64e2edf48a85b9e67886f0593b24bc438cdf`  
		Last Modified: Fri, 26 May 2023 00:20:14 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
