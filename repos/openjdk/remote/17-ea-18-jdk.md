## `openjdk:17-ea-18-jdk`

```console
$ docker pull openjdk@sha256:9c74bd3ffd86f192c461dae30d34f98f3f0867786122d1d88a15b597cb9804f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `openjdk:17-ea-18-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:dd7c4ef0efae41fbcbb8ca197884df5d935895aca7f3c83d1b7240947664995a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241332950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76b2f7b3691641b2b382bcacca26bc29446c927222b9dbe8c91408d667dce9fd`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Mar 2021 21:01:16 GMT
ADD file:6a8b1c26fdbf2beb390286575735d9efcd8cd6c3d135c9d7d25b3fe4c641a7ee in / 
# Tue, 30 Mar 2021 21:01:16 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:36:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Mar 2021 21:36:55 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Tue, 30 Mar 2021 21:36:55 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Mar 2021 21:36:55 GMT
ENV LANG=C.UTF-8
# Fri, 16 Apr 2021 22:21:13 GMT
ENV JAVA_VERSION=17-ea+18
# Fri, 16 Apr 2021 22:21:23 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='272350ce50f4f6f5ff111060a05bafa14f1adfe9ea9f0df06ea1cb242760ed29'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='0b65ebc5bcb5e14028c6459bc32158ac530bb41418ca2be95de4da4e64d90df7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Apr 2021 22:21:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:50c2d151af498a24eabbdd1f14042e94106189e17f7858fa9c9e6537816bfa34`  
		Last Modified: Tue, 30 Mar 2021 21:02:23 GMT  
		Size: 42.1 MB (42065616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26bc0351d047f744512b1f8920863854334f02e11637445a710596e8d9aaa7d`  
		Last Modified: Tue, 30 Mar 2021 21:43:00 GMT  
		Size: 13.3 MB (13265630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cf9228d5dee5e22802266b967dbbb03d58c9f57ab7098649a6337168c4a6fd`  
		Last Modified: Fri, 16 Apr 2021 22:26:43 GMT  
		Size: 186.0 MB (186001704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-18-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:89430da7017b85b981ee37f4a547f8f33f120535dcd812d6a9218d0fcb13d5c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.1 MB (238117919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2112e8e2f59e84b3fad9fbf4d2988bb3e20eb710bae394089cf55d0229eb2af0`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Mar 2021 20:50:28 GMT
ADD file:a59a6e0ab925ce07b112d2a2ec9d3f239ea833dc65666a0d1d898d3b048c96ef in / 
# Tue, 30 Mar 2021 20:50:31 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:34:57 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Mar 2021 21:34:58 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Tue, 30 Mar 2021 21:34:59 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Mar 2021 21:35:00 GMT
ENV LANG=C.UTF-8
# Fri, 16 Apr 2021 22:40:26 GMT
ENV JAVA_VERSION=17-ea+18
# Fri, 16 Apr 2021 22:41:20 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='272350ce50f4f6f5ff111060a05bafa14f1adfe9ea9f0df06ea1cb242760ed29'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='0b65ebc5bcb5e14028c6459bc32158ac530bb41418ca2be95de4da4e64d90df7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Apr 2021 22:41:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7da3223bdf8ee9e05ea4db775be9cb26ab65169aba0ba04ec2c3e0fa7331f0a2`  
		Last Modified: Tue, 30 Mar 2021 20:51:50 GMT  
		Size: 42.0 MB (41995846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e536b6ea357fbefc427ef10b23569012130790959e996d73efed97a345522cf`  
		Last Modified: Tue, 30 Mar 2021 21:41:18 GMT  
		Size: 14.0 MB (14033795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47121d1c52478ab7e2bbddc6e65c19ed7cdc087cbe5c585f49dc922ee2d0edf`  
		Last Modified: Fri, 16 Apr 2021 22:47:11 GMT  
		Size: 182.1 MB (182088278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-18-jdk` - windows version 10.0.17763.1879; amd64

```console
$ docker pull openjdk@sha256:fd1b84b205616f988ec6fbed96dda7c3cc2dc2d56dc878f06d59b0865c898ccf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2656584532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294d5d708383a56bd2bd5a639ef2b1e9f8900b5980d2000cc7dafb71333486ba`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 16:45:00 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Apr 2021 16:45:01 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Apr 2021 16:45:32 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 16 Apr 2021 22:15:19 GMT
ENV JAVA_VERSION=17-ea+18
# Fri, 16 Apr 2021 22:15:20 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_windows-x64_bin.zip
# Fri, 16 Apr 2021 22:15:21 GMT
ENV JAVA_SHA256=68e2ae787b12780848818c1b8d16b3e18003b25f04efb989ed3c137acbb0321b
# Fri, 16 Apr 2021 22:16:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 16 Apr 2021 22:16:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3d005d273e9763b53b5f1034b1284bcce913f8dbd1855d70f561efc09be849`  
		Last Modified: Wed, 14 Apr 2021 17:36:21 GMT  
		Size: 5.1 MB (5074608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ab40deb7e8f2f68f8ddebdcf9a4ccf7112615246fd6c75d400cd491cdac535`  
		Last Modified: Wed, 14 Apr 2021 17:36:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3fa76ecf2e81ab47fe24f1aeab9427a58be444cc60cf90038197c769d046a0`  
		Last Modified: Wed, 14 Apr 2021 17:36:21 GMT  
		Size: 319.5 KB (319514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d30133686100b41cb4b6e8727fbfa4975b872a87d1399ebd4acea12757b46e4`  
		Last Modified: Fri, 16 Apr 2021 23:22:01 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbc2925de72f24193036c25117d1c6c4b90497f37ce20191ece06f39ced5e5a`  
		Last Modified: Fri, 16 Apr 2021 23:22:02 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00fa4b7610ecb65b18b4100f640351da780d5aa1a50b7df244012487c00c8d8`  
		Last Modified: Fri, 16 Apr 2021 23:22:01 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8be0182fc89d090ebcbfa3e6b3a6c72330a957e9c5b85d0603438845ea0095b`  
		Last Modified: Fri, 16 Apr 2021 23:22:20 GMT  
		Size: 181.4 MB (181428101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fc7d133dc7a2b64e0d318092e8eac5bf76ec36c66fa0ea76e2420233cb7eb5`  
		Last Modified: Fri, 16 Apr 2021 23:22:02 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-18-jdk` - windows version 10.0.14393.4350; amd64

```console
$ docker pull openjdk@sha256:86cf7300bb90bee0dbc479d906cac05001136ddd1340d8c71d687c22b71ea1b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5992822539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fa01d4e9b9436271d8cd2ac5da5f6f6708433dde932a9ab7cc89d5f3732432d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 16:48:32 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Apr 2021 16:48:33 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Apr 2021 16:50:24 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 16 Apr 2021 22:16:47 GMT
ENV JAVA_VERSION=17-ea+18
# Fri, 16 Apr 2021 22:16:48 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_windows-x64_bin.zip
# Fri, 16 Apr 2021 22:16:49 GMT
ENV JAVA_SHA256=68e2ae787b12780848818c1b8d16b3e18003b25f04efb989ed3c137acbb0321b
# Fri, 16 Apr 2021 22:19:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 16 Apr 2021 22:19:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e39566a6e39d3a16eac2642132dd97b58680502417c33529cb3b20734e62ffd`  
		Last Modified: Wed, 14 Apr 2021 17:37:12 GMT  
		Size: 5.6 MB (5648642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501b89977f05abcd65cccdbfec96af4495b33ee4acc7932a4bf2a77874b2d40`  
		Last Modified: Wed, 14 Apr 2021 17:37:09 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79ef171c9bf6c1503c79940d0393f3121096ad7a3a91bc2d65c511c78175e8`  
		Last Modified: Wed, 14 Apr 2021 17:37:11 GMT  
		Size: 5.6 MB (5595448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce517039ea0a499c5e6a7366c50c9aa0cec53cb6797365dbf353b263ddb3e2ea`  
		Last Modified: Fri, 16 Apr 2021 23:22:42 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c15c544da8b84b3b6c4d9a59d99f51a1b94b889d4c9b75e1b4c478c233036`  
		Last Modified: Fri, 16 Apr 2021 23:22:42 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4baea0205ddc34fe91a72da5407b39833bfb44321928ae445a9564b923fdbd4`  
		Last Modified: Fri, 16 Apr 2021 23:22:43 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4747b84bd66393fd04f8bc1dda8bd688cabaa91940ebfa9a0aa2e0354a971e`  
		Last Modified: Fri, 16 Apr 2021 23:23:11 GMT  
		Size: 186.7 MB (186686020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189ee5d904e76b22900c45f23f3fb76aa1897d1d79be67f1b4700db1442ace20`  
		Last Modified: Fri, 16 Apr 2021 23:22:42 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
