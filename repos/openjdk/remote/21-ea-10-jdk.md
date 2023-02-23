## `openjdk:21-ea-10-jdk`

```console
$ docker pull openjdk@sha256:163ed09a4ce4b969a5fecf56b86a339d28bce3ea54248e4540d445789ccb8a7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `openjdk:21-ea-10-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:07f02c9be711e04f8ab59a4a40ab41d47abb5c2cdbd7b964540be886953c428b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256125648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7191613b0bb1eb14f9ae2f9356d1eece7daf36db5a3f526ea27ee17f4ff91223`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Feb 2023 19:37:08 GMT
ADD file:7c92981e2fed9bedfca663209480ce9006dce0edc6c44c25640255683952b929 in / 
# Thu, 23 Feb 2023 19:37:08 GMT
CMD ["/bin/bash"]
# Thu, 23 Feb 2023 19:56:18 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Feb 2023 19:56:18 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 23 Feb 2023 19:56:18 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Feb 2023 19:56:18 GMT
ENV LANG=C.UTF-8
# Thu, 23 Feb 2023 19:56:19 GMT
ENV JAVA_VERSION=21-ea+10
# Thu, 23 Feb 2023 19:56:29 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/10/GPL/openjdk-21-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='e60198534add038869d333ae9564ff8be298d712c5518b865952d66d07638b7b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/10/GPL/openjdk-21-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='eb5e840f2f81330fa3080312da34ce1daabb27138bbebdbb5ea409d79a970e6c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Feb 2023 19:56:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1319f85bbd2aad3767d41a6c767c94c23f7432642c7bda3df878c147ba384902`  
		Last Modified: Thu, 23 Feb 2023 19:38:02 GMT  
		Size: 44.6 MB (44552452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565fe2a72fd544bf059ba3dab17c20dd57232b65e41885f9004b841d0106f73b`  
		Last Modified: Thu, 23 Feb 2023 19:58:20 GMT  
		Size: 12.2 MB (12246468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cc176753cc1e165ecfba28a9a7c494cc15e2d19148b3529c58152e4125b66e`  
		Last Modified: Thu, 23 Feb 2023 19:58:32 GMT  
		Size: 199.3 MB (199326728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-10-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:9994bb788f77e985701b9845c29b5fc4ba82f8cb00e619fe23ab717dea1e664b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.3 MB (254347152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f72d04d0e491689a963c3401dbe0d00faea2d33ad19be53160ca99baf16f6f`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Feb 2023 19:52:36 GMT
ADD file:650f46a4a6a15a9b2d6f048bb51976942936d0c5daba7b0337bceacbc4efcf85 in / 
# Thu, 23 Feb 2023 19:52:37 GMT
CMD ["/bin/bash"]
# Thu, 23 Feb 2023 20:13:51 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Feb 2023 20:13:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 23 Feb 2023 20:13:51 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Feb 2023 20:13:51 GMT
ENV LANG=C.UTF-8
# Thu, 23 Feb 2023 20:13:51 GMT
ENV JAVA_VERSION=21-ea+10
# Thu, 23 Feb 2023 20:14:05 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/10/GPL/openjdk-21-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='e60198534add038869d333ae9564ff8be298d712c5518b865952d66d07638b7b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/10/GPL/openjdk-21-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='eb5e840f2f81330fa3080312da34ce1daabb27138bbebdbb5ea409d79a970e6c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Feb 2023 20:14:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7166504978b203e953381fdfe4d9e7656565d62a75183fcc5bf460e6135e033d`  
		Last Modified: Thu, 23 Feb 2023 19:53:23 GMT  
		Size: 43.5 MB (43459902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766ec681792700cac3beb59912bb93402833e5171c8ae979918ee6806da3d433`  
		Last Modified: Thu, 23 Feb 2023 20:16:05 GMT  
		Size: 13.1 MB (13073314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d49c44a5cd05f075b0bf6db6725e39ff3305ebc272377549029b9483847bbba`  
		Last Modified: Thu, 23 Feb 2023 20:16:16 GMT  
		Size: 197.8 MB (197813936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-10-jdk` - windows version 10.0.20348.1547; amd64

```console
$ docker pull openjdk@sha256:6deb1ac603d96bf4230dcf720b326a5cd8e2b4c5f83143a51763aec9dedb685b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875501602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17eddb27c35482389aba7f5ebe53f1020b9d7aa186ec4de16e826a7efc48714b`
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
# Sat, 18 Feb 2023 00:01:20 GMT
ENV JAVA_VERSION=21-ea+10
# Sat, 18 Feb 2023 00:01:21 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/10/GPL/openjdk-21-ea+10_windows-x64_bin.zip
# Sat, 18 Feb 2023 00:01:24 GMT
ENV JAVA_SHA256=68e0d0fd2ee261104468254cbb5c2087e757f7897c4b0ad7c462af5aef2df3c8
# Sat, 18 Feb 2023 00:04:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 18 Feb 2023 00:04:59 GMT
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
	-	`sha256:a241c5a5a1bd00c6eff8c509724fa450e588edac3b528386dc7596b0b653d430`  
		Last Modified: Sat, 18 Feb 2023 00:12:19 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81c7f2cef22e3f1fc7bc8942c91e22755903b336ed06ee52229e70605cb0378`  
		Last Modified: Sat, 18 Feb 2023 00:12:19 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b202b864c744668ad5a63d5f636911206b85c30acd3cb063bcd12dd30008b31`  
		Last Modified: Sat, 18 Feb 2023 00:12:18 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d712990be9dbd3968ae8ea18b96c20d86c8fbf343727f874c884e121d2cc9aea`  
		Last Modified: Sat, 18 Feb 2023 00:12:46 GMT  
		Size: 194.8 MB (194805593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa49df0d9277fc59ed4941456d9c8ae2641851ad9b81bf74966c8558712f90b3`  
		Last Modified: Sat, 18 Feb 2023 00:12:19 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-10-jdk` - windows version 10.0.17763.4010; amd64

```console
$ docker pull openjdk@sha256:503f42f1d79ff199219a1fd1bfc11ab40c8e25627937150453cd77e5052f14fd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2158388419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8fcef8a4d086af92b8493baa8bb1937e192d80d3fe27f344b7c16f981d6c93b`
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
# Sat, 18 Feb 2023 00:05:17 GMT
ENV JAVA_VERSION=21-ea+10
# Sat, 18 Feb 2023 00:05:20 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/10/GPL/openjdk-21-ea+10_windows-x64_bin.zip
# Sat, 18 Feb 2023 00:05:21 GMT
ENV JAVA_SHA256=68e0d0fd2ee261104468254cbb5c2087e757f7897c4b0ad7c462af5aef2df3c8
# Sat, 18 Feb 2023 00:09:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 18 Feb 2023 00:09:08 GMT
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
	-	`sha256:50c722efcf3b93a47fddf612846887ddf3096e3bdc38ee220f49ad8756d57682`  
		Last Modified: Sat, 18 Feb 2023 00:13:07 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87167ed9fce0f0e8c8cfd6a743274839304dae8e6d1b81c44d8ce2ffb229d7d9`  
		Last Modified: Sat, 18 Feb 2023 00:13:07 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f090a39409b1643a351a564f6d31e1258223845f57787f0e456923e7a03af`  
		Last Modified: Sat, 18 Feb 2023 00:13:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c193e6408f3e999b95e23c078f6164e3a743412ff1b3097b8aa45dc2e4b82ab3`  
		Last Modified: Sat, 18 Feb 2023 00:13:36 GMT  
		Size: 194.6 MB (194573344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce56f55779f93a4d50bf55792b74c7b4a4276500ce9952edc1c036b5d8a6bf9b`  
		Last Modified: Sat, 18 Feb 2023 00:13:07 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
