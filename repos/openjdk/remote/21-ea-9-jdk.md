## `openjdk:21-ea-9-jdk`

```console
$ docker pull openjdk@sha256:68fccc9031d3ddc9ff65a6575d1bb799a8e9eb32afbf58e483b35cf715c0b568
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `openjdk:21-ea-9-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:b9fcb015201a82b07acd54605cc07b65cba4873234fd86fba7e81ed390912043
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256069022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66537da09d724b26b70c154a47a9d100c546ab457106ea117018f37e2115d834`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Feb 2023 19:27:31 GMT
ADD file:6a3fb962576ab4237e9335cfcf419249f08417e28cfbb633d7cc6f26f1f85287 in / 
# Wed, 08 Feb 2023 19:27:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Feb 2023 19:44:53 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 08 Feb 2023 19:44:53 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 08 Feb 2023 19:44:54 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Feb 2023 19:44:54 GMT
ENV LANG=C.UTF-8
# Fri, 10 Feb 2023 18:37:14 GMT
ENV JAVA_VERSION=21-ea+9
# Fri, 10 Feb 2023 18:37:28 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='50ce8bd2e9b710726e7117ba3a302287a0be51cb187721a422ee63cadbf717a2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='86f137227e32994689e70b0a2f426adb45a16807bc84398926e841452cfe83d0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Feb 2023 18:37:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:197c1adcd755131915cd019bdd58658d44445b3638f65449932c18ee39b6047c`  
		Last Modified: Wed, 08 Feb 2023 19:29:00 GMT  
		Size: 44.6 MB (44555906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b698b7af4b18900b53c768746b1dfb603dfb9aec1eea328fdac86d37001e2a`  
		Last Modified: Wed, 08 Feb 2023 19:48:51 GMT  
		Size: 12.3 MB (12256034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2a81cf7215cb2e3a50bb44e0839cdf2cb7101db2da6f655d951277d73678b8`  
		Last Modified: Fri, 10 Feb 2023 18:44:03 GMT  
		Size: 199.3 MB (199257082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-9-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:64e1dbd93af081fa9f0b80568ccdcb5723fd8fe0a208cabb53b3736c89ffd986
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.2 MB (254248577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53c8b5086e1fb4bd01f63988d9532fc2a3b38d10788ffeae551240400d607a8a`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Feb 2023 19:44:57 GMT
ADD file:b0d30d32b82572c00d83e2fd97813f8b9ff4c6a92efcd3696df1120df4c1065f in / 
# Wed, 08 Feb 2023 19:44:58 GMT
CMD ["/bin/bash"]
# Wed, 08 Feb 2023 20:04:19 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 08 Feb 2023 20:04:19 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 08 Feb 2023 20:04:19 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Feb 2023 20:04:19 GMT
ENV LANG=C.UTF-8
# Fri, 10 Feb 2023 01:56:32 GMT
ENV JAVA_VERSION=21-ea+9
# Fri, 10 Feb 2023 01:56:42 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='50ce8bd2e9b710726e7117ba3a302287a0be51cb187721a422ee63cadbf717a2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='86f137227e32994689e70b0a2f426adb45a16807bc84398926e841452cfe83d0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Feb 2023 01:56:44 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7d4ed4ca78bc8f807025d2f2a491ee60099ed37ad040ce330257955d319a347f`  
		Last Modified: Wed, 08 Feb 2023 19:46:11 GMT  
		Size: 43.5 MB (43456591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb69dde29350e5a2369237cbe74bc3c8c50699d796a4fd09120ea4a5b1f26be9`  
		Last Modified: Wed, 08 Feb 2023 20:08:29 GMT  
		Size: 13.1 MB (13073762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb85c5ae53bd4df853acf7bec01dd58501f1af7ae0ff7c5f6557c838e1ac0f5`  
		Last Modified: Fri, 10 Feb 2023 02:02:57 GMT  
		Size: 197.7 MB (197718224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-9-jdk` - windows version 10.0.20348.1547; amd64

```console
$ docker pull openjdk@sha256:916c1ccb32c5f8ad0c70280df8730704ad62ff72881056e05b8a4307910b0719
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875414271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27fb2043f176c73120d5624e3e4af575a06c737dd062c3284e928ed8d6efd15c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:14:39 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:14:40 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 16 Feb 2023 02:15:04 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:15:05 GMT
ENV JAVA_VERSION=21-ea+9
# Thu, 16 Feb 2023 02:15:06 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_windows-x64_bin.zip
# Thu, 16 Feb 2023 02:15:06 GMT
ENV JAVA_SHA256=012fada2a58fa64ab3708ede97876c32050dc6c4dd4c77d29740af88954bda8d
# Thu, 16 Feb 2023 02:16:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:16:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8108d16cd884206ec4969828d09af6c32cb29b30d6f5ac0628fbaa03f5acbfc3`  
		Last Modified: Thu, 16 Feb 2023 02:27:56 GMT  
		Size: 770.5 KB (770457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c865bc76fec4cadb1aba9ec04e94e30b1ae91b8396e43f048cac5d9e9751fb`  
		Last Modified: Thu, 16 Feb 2023 02:27:55 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f5b31252c305eec6ed404696a45a13faa4edf1d630169d6b56eb13e25229c`  
		Last Modified: Thu, 16 Feb 2023 02:27:55 GMT  
		Size: 570.8 KB (570829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5308fc3f77ca9348e28d33121478a39592f8693093f9537aa56e6bd002fb75d`  
		Last Modified: Thu, 16 Feb 2023 02:27:52 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fc6fbdd8b38a41cc02ff30637c44fe8663b8ada70dce00ad1818243c079255`  
		Last Modified: Thu, 16 Feb 2023 02:27:52 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d137ced33dfd0fadd0652e297ecbfb586d262527bc12faa25bf2990a01e9c3a2`  
		Last Modified: Thu, 16 Feb 2023 02:27:53 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d01680b0bcb1b4af46c72f6526af6ae70d697a08b11ae95f96353f06848e997`  
		Last Modified: Thu, 16 Feb 2023 02:28:14 GMT  
		Size: 194.7 MB (194718137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12042ede1b9fadbb34038830abb0ee1ca370d1427eadeab4795214adedf3e22`  
		Last Modified: Thu, 16 Feb 2023 02:27:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-9-jdk` - windows version 10.0.17763.4010; amd64

```console
$ docker pull openjdk@sha256:9ca6e38289520a4317079cda276cdcc955cd01fa1241ecd7f938287df08ba04b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2158303108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17d172d305f9864ee69e5756aa7c6564d54ab1809383f7ee7195845d49294999`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:17:23 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:17:24 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 16 Feb 2023 02:18:29 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:18:30 GMT
ENV JAVA_VERSION=21-ea+9
# Thu, 16 Feb 2023 02:18:31 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_windows-x64_bin.zip
# Thu, 16 Feb 2023 02:18:32 GMT
ENV JAVA_SHA256=012fada2a58fa64ab3708ede97876c32050dc6c4dd4c77d29740af88954bda8d
# Thu, 16 Feb 2023 02:20:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:20:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98437cec399b6656d20521928c292ca8c2e4c0c737b7cb970de037167fc8db6f`  
		Last Modified: Thu, 16 Feb 2023 02:28:35 GMT  
		Size: 515.3 KB (515330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0fdacfc64d4626f9464e954281e2675812980cad460d5989807088ab5d22d6`  
		Last Modified: Thu, 16 Feb 2023 02:28:35 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63aceb75603170d702778c30ea615042a578e11438c4f8e572720a1a81963ec`  
		Last Modified: Thu, 16 Feb 2023 02:28:35 GMT  
		Size: 333.4 KB (333385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a632c96df365bd1475c1f4e881a34f90112435f9e3d5aed355aa6d61d5f9f8b8`  
		Last Modified: Thu, 16 Feb 2023 02:28:33 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20c098de9ee331a2b164134cfe5ce950ea4bba048a3711e39de24b5a860ad6`  
		Last Modified: Thu, 16 Feb 2023 02:28:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fdd93b432a5883e2797fbe338090248951b3f09dd5ee3ab959159c1e44d7d4`  
		Last Modified: Thu, 16 Feb 2023 02:28:33 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c16acb0407b3048a5a87ea468ccee40948819781e7ae8eaa01e19ca84aa75e`  
		Last Modified: Thu, 16 Feb 2023 02:28:54 GMT  
		Size: 194.5 MB (194487983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28c0ceb99a84ce69de6895d51a1c0b49864854046a6316cd7637a203432c6dc`  
		Last Modified: Thu, 16 Feb 2023 02:28:33 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
