## `openjdk:20-ea-20-jdk`

```console
$ docker pull openjdk@sha256:d16496e020f94f1424ab9d31748a8d339c5050e2761a03abf179c76a3c17ba88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1129; amd64
	-	windows version 10.0.17763.3532; amd64

### `openjdk:20-ea-20-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:088aab8034380f0d9d3e042e97f9a0130fe1faeb04e8c278eccd5c73b68b7eb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.9 MB (249937308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc57e4e66e694f144b16cedb3df7f6f38b7a6c8aa490a487ac06b07a1ee616e8`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:51:29 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:51:29 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Fri, 21 Oct 2022 19:51:29 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2022 19:51:29 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2022 19:51:29 GMT
ENV JAVA_VERSION=20-ea+20
# Fri, 21 Oct 2022 19:51:40 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='0cb0f79bee2e61134a86049952a1e572bb3e2dad49aa200a20f18c697715a402'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='4db7319dfbfb4a3561e9707c0178d0ba8d6413bc94f13d8c9ce406fd7445e000'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Oct 2022 19:51:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f15da7b20d89dec72e0bff2c38edc4d7119a8f5049343764ac32b207f7bd7b9`  
		Last Modified: Fri, 21 Oct 2022 19:55:16 GMT  
		Size: 12.2 MB (12231175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260cbb1d34a59f50f2fdfaac9c65eb84b3c19441a52f658f2063cff4c8ceccc5`  
		Last Modified: Fri, 21 Oct 2022 19:55:30 GMT  
		Size: 197.1 MB (197117386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-20-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:97d84a34c87b192034ebe3021280374a34dd151bbb6d8cd9d7768a9f1e81b976
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.1 MB (248136747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d654752fc77c1dfe2e17fbebabbb4f9fbf227f321488fc44eec7ef5b8952127`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:05:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 21 Oct 2022 20:05:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Fri, 21 Oct 2022 20:05:55 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2022 20:05:56 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2022 20:05:57 GMT
ENV JAVA_VERSION=20-ea+20
# Fri, 21 Oct 2022 20:06:09 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='0cb0f79bee2e61134a86049952a1e572bb3e2dad49aa200a20f18c697715a402'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='4db7319dfbfb4a3561e9707c0178d0ba8d6413bc94f13d8c9ce406fd7445e000'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Oct 2022 20:06:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f680af7f923e4833016ec0913265a98759f537be7682214cfab283f2577edc78`  
		Last Modified: Fri, 21 Oct 2022 20:13:32 GMT  
		Size: 13.1 MB (13054886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd55ea58fb31963ffd5a44c705b990fe642fd26b93be26b6bec2c727528f9b00`  
		Last Modified: Fri, 21 Oct 2022 20:13:47 GMT  
		Size: 195.7 MB (195673710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-20-jdk` - windows version 10.0.20348.1129; amd64

```console
$ docker pull openjdk@sha256:c29a07fa3fb29525879b6a52ac4fd1f0e3d238b73b0652fc441cc6aa565c45fa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2609991609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:728fbe5d8feb6d32ea033b10fc9bdfdabc1d36fe27e4bf65c366649dbcd3ab97`
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
# Thu, 20 Oct 2022 20:17:19 GMT
ENV JAVA_VERSION=20-ea+20
# Thu, 20 Oct 2022 20:17:19 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_windows-x64_bin.zip
# Thu, 20 Oct 2022 20:17:20 GMT
ENV JAVA_SHA256=9435f4c1b174163806adf97e70e974aef9becfe0394a343831509ca56d05f01e
# Thu, 20 Oct 2022 20:18:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 20 Oct 2022 20:18:33 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
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
	-	`sha256:b3551e507e13ca80b940f09c8e912a14eda0ce7895bb844c9d10374f196f8e56`  
		Last Modified: Thu, 20 Oct 2022 20:23:04 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc9cf42286623c2d14deadc3991e784ba341ba93ff0f3d7234013970a97b5c9`  
		Last Modified: Thu, 20 Oct 2022 20:23:04 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238736766c8aed82402341d79fea69e7240229a0c5d3d4776fccf7c8eaffaf75`  
		Last Modified: Thu, 20 Oct 2022 20:23:04 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac16f971b9271079296a8776488a9850937698510af0ef401abd473366902153`  
		Last Modified: Thu, 20 Oct 2022 20:23:27 GMT  
		Size: 192.6 MB (192625257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3ba4e89f2bc381ae30a910d3cd1dc2a89aa1c5ef37222181f3659d751bdc8d`  
		Last Modified: Thu, 20 Oct 2022 20:23:04 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-20-jdk` - windows version 10.0.17763.3532; amd64

```console
$ docker pull openjdk@sha256:635a0b9516f19ef6742ed401715901dbf61a566f9acaa821ede6852d223a8e6d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2904264700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e06c335d38b879e3744e140ecedc9d4353ca2e0b150cd04350a2ed2438c2180`
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
# Thu, 20 Oct 2022 20:18:44 GMT
ENV JAVA_VERSION=20-ea+20
# Thu, 20 Oct 2022 20:18:45 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_windows-x64_bin.zip
# Thu, 20 Oct 2022 20:18:46 GMT
ENV JAVA_SHA256=9435f4c1b174163806adf97e70e974aef9becfe0394a343831509ca56d05f01e
# Thu, 20 Oct 2022 20:20:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 20 Oct 2022 20:20:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
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
	-	`sha256:9d21b72d9d9dcbf4da52d9e24645ad75a7d3930ac86b1e036276669ac24651f9`  
		Last Modified: Thu, 20 Oct 2022 20:23:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0d7ed0a70410b2d8af8583c259071ea31e7895a01617c5a64386f349d275f4`  
		Last Modified: Thu, 20 Oct 2022 20:23:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4ee27c1e77fb08e8b9eafaacbe611057e15381f5a05c5dec84e8e53d0a0579`  
		Last Modified: Thu, 20 Oct 2022 20:23:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b65b1a7ed74dd8b340ec1203415d8dee32c078a6b3f45a179cbbf81cce4f58`  
		Last Modified: Thu, 20 Oct 2022 20:24:09 GMT  
		Size: 192.4 MB (192433506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42c0e17c09ace7eda452b18453b5049b07855b9e8394eebc2a6928966bdb7d`  
		Last Modified: Thu, 20 Oct 2022 20:23:49 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
