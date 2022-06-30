## `openjdk:20-jdk`

```console
$ docker pull openjdk@sha256:3a1dc196fbb30b56a7e02d41c8f2a229e7312660623177328a6696d022fea458
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.768; amd64
	-	windows version 10.0.17763.3046; amd64

### `openjdk:20-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:a145b5191c96b982398ded1d0fdc27a0d6031792572b8f5e5ab89f90ce5ddd0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.9 MB (249879997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49cafc33e9fad9b5dd876263b5390233b999d0a52c008f8217d8d6979827e8fe`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Jun 2022 17:20:45 GMT
ADD file:03d0377f5864198b250372de990ebf0ef7597cfdcc2e18421e8e0025394a7572 in / 
# Thu, 30 Jun 2022 17:20:46 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 17:37:33 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 30 Jun 2022 17:37:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 30 Jun 2022 17:37:33 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jun 2022 17:37:34 GMT
ENV LANG=C.UTF-8
# Thu, 30 Jun 2022 17:37:34 GMT
ENV JAVA_VERSION=20-ea+3
# Thu, 30 Jun 2022 17:37:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/3/GPL/openjdk-20-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='8f930cbbf2c85c0cfe87eef8646d1e038fe51d19132613e868e96118b1e0f8d0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/3/GPL/openjdk-20-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='d7b270b059fe08487492d38760e0e821b3a7be20864205d7ab0b5e5206109bda'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 30 Jun 2022 17:37:44 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:337897a5aaf7b54e691e2ed305fbf00e0e8933d5a8a3c07d6fbb95f10b15c644`  
		Last Modified: Thu, 30 Jun 2022 17:21:37 GMT  
		Size: 39.2 MB (39221672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1e7c755c4cccc19ca62372088ce86de7711ff0e0e2e7e18f65711eb2299602`  
		Last Modified: Thu, 30 Jun 2022 17:45:09 GMT  
		Size: 13.5 MB (13509384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63012b5e715f55e4ffdc7118eab9c8304685e8554f82b7e884b9afc9f7bd4ced`  
		Last Modified: Thu, 30 Jun 2022 17:45:22 GMT  
		Size: 197.1 MB (197148941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:1acf50078f758ec39001e19292d8ca88743539db9bc361251f2139b983f899e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.3 MB (248319901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cad3a37cf3c5df11dc99487dfb30bf0111e13276d800b4ee9d30ef9e35db057`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Jun 2022 17:40:34 GMT
ADD file:deb746f3cc547a36a34f3bfe68510bbd6f8a3b2da72bcca3cce36dfe0e519e77 in / 
# Thu, 30 Jun 2022 17:40:35 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 18:00:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 30 Jun 2022 18:00:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 30 Jun 2022 18:00:55 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jun 2022 18:00:56 GMT
ENV LANG=C.UTF-8
# Thu, 30 Jun 2022 18:00:57 GMT
ENV JAVA_VERSION=20-ea+3
# Thu, 30 Jun 2022 18:01:18 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/3/GPL/openjdk-20-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='8f930cbbf2c85c0cfe87eef8646d1e038fe51d19132613e868e96118b1e0f8d0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/3/GPL/openjdk-20-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='d7b270b059fe08487492d38760e0e821b3a7be20864205d7ab0b5e5206109bda'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 30 Jun 2022 18:01:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c7107c973a1b04b1f048e43f460fd4f030df5f2e53fce3dfb8a13dc7fefdb4b0`  
		Last Modified: Thu, 30 Jun 2022 17:41:32 GMT  
		Size: 38.0 MB (38023864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a33b6e144a0eee25610c802e234489b8afda2108ce38e5f76ee4d79e5e45ff`  
		Last Modified: Thu, 30 Jun 2022 18:15:30 GMT  
		Size: 14.3 MB (14303308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a15aa1dc5096392961caa44354931a26b8fd9919dab56c9f6846f06efeb9403`  
		Last Modified: Thu, 30 Jun 2022 18:15:47 GMT  
		Size: 196.0 MB (195992729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk` - windows version 10.0.20348.768; amd64

```console
$ docker pull openjdk@sha256:49130bb9f65c6e942150b51a19439fab8410398285b3fd829fe4a5a8449d6e06
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2472446705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38253345dbfb810bab0db3516958a2ab8713252a27334bee8b47750800ae76f2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 19:30:14 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Jun 2022 01:14:39 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 16 Jun 2022 01:15:08 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Tue, 28 Jun 2022 00:14:58 GMT
ENV JAVA_VERSION=20-ea+3
# Tue, 28 Jun 2022 00:15:00 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/3/GPL/openjdk-20-ea+3_windows-x64_bin.zip
# Tue, 28 Jun 2022 00:15:01 GMT
ENV JAVA_SHA256=d6bd89dafc55e34638d75e312e32bea22f8b2132baf19c2749e8dbe5fda7c5bb
# Tue, 28 Jun 2022 00:15:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 28 Jun 2022 00:15:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b6e059d50cccbff94037bf242f1b94acf1cc939d701dff58c07f4fcfdc9767`  
		Last Modified: Wed, 15 Jun 2022 20:02:04 GMT  
		Size: 632.3 KB (632288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e4ff554b66055922423d154f7282c8144066ebe31d1393200cf475fb56555f`  
		Last Modified: Thu, 16 Jun 2022 01:26:02 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a207dedd7fa079f899254dd9a6ea4b20cbb4e77f9880ed19716901e210c1e42f`  
		Last Modified: Thu, 16 Jun 2022 01:26:02 GMT  
		Size: 564.2 KB (564202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2af4ee24347f154b1cf7fcb4aa2f97a75e82031c6e7f85474281553e37f2a5`  
		Last Modified: Tue, 28 Jun 2022 02:20:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d334f11f87fa4f9130548a41ce4eaf125c5cf80ac1c80b7e48888a1e0ce9ffe`  
		Last Modified: Tue, 28 Jun 2022 02:20:28 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dfb423ee6f29077b4623f20b91fbed731edc97e08ab19d70afcc519b43239e`  
		Last Modified: Tue, 28 Jun 2022 02:20:28 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aef8f8682b9dc25941354dc8cc65d34f5865d601f3b416feed15610359b95cf`  
		Last Modified: Tue, 28 Jun 2022 02:20:49 GMT  
		Size: 192.8 MB (192777648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8f8b91950493bcc4bc5c0754cbfd0331d3bbf2df4cffc3b6c5f047a6165a36`  
		Last Modified: Tue, 28 Jun 2022 02:20:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk` - windows version 10.0.17763.3046; amd64

```console
$ docker pull openjdk@sha256:4c0d526ac504b2ee59294ec77e3c25fac97d210d4a04bcaeef1ce60e3355fec7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2856498954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a7c2de60de4e79328f1e4f99611e1a74fb4692efef3dfbb0fcdfc94ee9bb6c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 19:33:08 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Jun 2022 01:16:22 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 16 Jun 2022 01:17:35 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Tue, 28 Jun 2022 00:16:12 GMT
ENV JAVA_VERSION=20-ea+3
# Tue, 28 Jun 2022 00:16:13 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/3/GPL/openjdk-20-ea+3_windows-x64_bin.zip
# Tue, 28 Jun 2022 00:16:14 GMT
ENV JAVA_SHA256=d6bd89dafc55e34638d75e312e32bea22f8b2132baf19c2749e8dbe5fda7c5bb
# Tue, 28 Jun 2022 00:18:01 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 28 Jun 2022 00:18:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75415e053743ebceabbf30d0a8101d97dd712c88fc012c45f1df824cbac48e21`  
		Last Modified: Wed, 15 Jun 2022 20:05:58 GMT  
		Size: 354.4 KB (354400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52024d1a50366ffd4635321735cd38ce0ecab43a1ba938284d4286b6020140ef`  
		Last Modified: Thu, 16 Jun 2022 01:29:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4732abfe811150ac2b9a2ccb0f838bf2f402b7f56952056d2f28ba681fc8b120`  
		Last Modified: Thu, 16 Jun 2022 01:29:40 GMT  
		Size: 312.4 KB (312396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b7b8658fe630fd1e79b96d180d48965e653cb345bd5899d32541786dbd423b`  
		Last Modified: Tue, 28 Jun 2022 02:21:10 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f2b963ab8ad3cbc071cfe1753c78d4b1e2ef9a9eab8cf1766a7727a3ed2dab`  
		Last Modified: Tue, 28 Jun 2022 02:21:10 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094ed4c67eeeb3811d26496a1e1a3f909578c579cf9d7f329a2325d8c7e1fa5a`  
		Last Modified: Tue, 28 Jun 2022 02:21:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6a38fb91102d540ebd3e59833990e11d454772d95d6b9f53a5dffe23e7d74d`  
		Last Modified: Tue, 28 Jun 2022 02:21:31 GMT  
		Size: 192.5 MB (192543959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade2ae5756d19ea567e31e5255a49995c7d1c66f841dc12b95518d531b5a0446`  
		Last Modified: Tue, 28 Jun 2022 02:21:10 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
