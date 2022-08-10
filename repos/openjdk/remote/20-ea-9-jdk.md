## `openjdk:20-ea-9-jdk`

```console
$ docker pull openjdk@sha256:4b6342643d5cc0c0e7c99e33b0a25aef5ba14fdd89aaee8f4f5f9af8b972f2a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `openjdk:20-ea-9-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:1a9409a7f753b1c36c1303bf396f582966423456512e7b38764922ddc7abede2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (249958254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201fb337745338ee4afdffed1c2400711cb4a7c47668f34ef822612b961f19e3`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:35:27 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:35:27 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 04 Aug 2022 01:35:27 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:35:27 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 22:51:01 GMT
ENV JAVA_VERSION=20-ea+9
# Mon, 08 Aug 2022 22:51:28 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='0d07c62c8d17ef034b26568ed71d3025cf9dcbc6b4294987e53d54cab10f549f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='13fc41a17f015ca801975625021a320b5112883194fc5dde964529894907fd83'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 22:51:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d72ac1fb23a36f89addf60367990f28d5c0882e4b8f569c77b51c51eb271261`  
		Last Modified: Thu, 04 Aug 2022 01:42:41 GMT  
		Size: 13.5 MB (13506500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42cf7a320801f642ab774ae90a06dd631bbdaff1a1d624c4bc5698bda715459a`  
		Last Modified: Mon, 08 Aug 2022 23:00:16 GMT  
		Size: 197.2 MB (197227802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-9-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f45b3e8a7b391cd5019777539ad14f56cb0007656e2c2920a9434219b9b39efa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.2 MB (248224453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7002618414e88d3c639308366042ab127ff361e2a7b05a8490cc5367c878bd`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:01:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:01:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 04 Aug 2022 01:01:13 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:01:14 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 23:29:46 GMT
ENV JAVA_VERSION=20-ea+9
# Mon, 08 Aug 2022 23:29:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='0d07c62c8d17ef034b26568ed71d3025cf9dcbc6b4294987e53d54cab10f549f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='13fc41a17f015ca801975625021a320b5112883194fc5dde964529894907fd83'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 23:29:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e225b6ab834ff85ee0d347a2859ecb14fc169f362360408133589ab8a37d8333`  
		Last Modified: Thu, 04 Aug 2022 01:14:59 GMT  
		Size: 14.3 MB (14278746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44516f349abc34c211463e2b6a990c2b2f5cfc954046603018baaa29061031a9`  
		Last Modified: Mon, 08 Aug 2022 23:45:45 GMT  
		Size: 195.9 MB (195922661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-9-jdk` - windows version 10.0.20348.887; amd64

```console
$ docker pull openjdk@sha256:91681c96537d044a6d2f545f2f4071d9ccb4bd8cc3ff9163c36e3253a4ff23c4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2510977592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f52184a22b801135b4183c991485492094d2d25d43f15232d4bcac96f09bb6a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 16:55:00 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 16:55:00 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 10 Aug 2022 16:55:20 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 16:55:20 GMT
ENV JAVA_VERSION=20-ea+9
# Wed, 10 Aug 2022 16:55:21 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_windows-x64_bin.zip
# Wed, 10 Aug 2022 16:55:22 GMT
ENV JAVA_SHA256=69540c9291f1d68616035ff98d95ec4b0bc9fe19d1bddbc4fe091a8c70fcf4f0
# Wed, 10 Aug 2022 16:56:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 16:56:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0cc935c154780815cf1fb6065aa1c262b52a7648b984b06133beb4e95833c0`  
		Last Modified: Wed, 10 Aug 2022 17:27:08 GMT  
		Size: 624.7 KB (624700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43525a703370320083aa7f64beeb4176b2090f555b73f9be7f9cb9fbda9f5736`  
		Last Modified: Wed, 10 Aug 2022 17:27:07 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf27aca426cd52616bfeb5296c1b75f2095211cf6c91d27a306c654522f65a32`  
		Last Modified: Wed, 10 Aug 2022 17:27:08 GMT  
		Size: 557.0 KB (557029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cd315ff6aac4a8596895322c5c74ed94937b941347fb4ff7f9447d6a3d7702`  
		Last Modified: Wed, 10 Aug 2022 17:27:05 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce3197a99489de7ea1a020b08b6d9da9bea3e25a4afac0864dcbd0dd2c6deab`  
		Last Modified: Wed, 10 Aug 2022 17:27:05 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48c85562a3d553b33a92263f110f2c9959e15f1e475cea04700c740f3bed484`  
		Last Modified: Wed, 10 Aug 2022 17:27:05 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0958535bb3500b7c90ff0cc2bd50eb8c31ef4bf01c24040b9a8d9b161e3db273`  
		Last Modified: Wed, 10 Aug 2022 17:27:28 GMT  
		Size: 192.9 MB (192898181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1121ba060e78cc69becff9a11ecc76964c9a34cec7280b2fada5a8a7289a7efd`  
		Last Modified: Wed, 10 Aug 2022 17:27:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-9-jdk` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:7f7370550c4b20544b78dc53b8899b06b69ae2b37154af76cd5aba794b3889bd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2871041196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69483bf086f33103dc57d3b9ddabdd9076b0b6df7272bd180cb2dfa59393a67c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 16:57:20 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 16:57:21 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 10 Aug 2022 16:58:18 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 16:58:19 GMT
ENV JAVA_VERSION=20-ea+9
# Wed, 10 Aug 2022 16:58:20 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_windows-x64_bin.zip
# Wed, 10 Aug 2022 16:58:21 GMT
ENV JAVA_SHA256=69540c9291f1d68616035ff98d95ec4b0bc9fe19d1bddbc4fe091a8c70fcf4f0
# Wed, 10 Aug 2022 16:59:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 16:59:51 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9df80b59d75310c5b623001e9a6fefa8c2f0255dfbb8c58e60daa3aba0f9c6`  
		Last Modified: Wed, 10 Aug 2022 17:27:52 GMT  
		Size: 347.3 KB (347323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a313f85e8b9975fcba0bc4920f5caf6d1aca17b778349b49c87d1633e7ae60eb`  
		Last Modified: Wed, 10 Aug 2022 17:27:51 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448a04775e0e1c17f4166d28a03de82719ce659ec910523df8a06c97c94a7d3b`  
		Last Modified: Wed, 10 Aug 2022 17:27:51 GMT  
		Size: 309.6 KB (309626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c5d5d021af3361c719e242ebdfa094043dce5aae8902ea93eecd536db91000`  
		Last Modified: Wed, 10 Aug 2022 17:27:49 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d3573078e4d5ab892bfc029f2123ea933564488aaee13251823acfec339891`  
		Last Modified: Wed, 10 Aug 2022 17:27:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc056ffdcc0ca61badec1af19eaf4e1b2ecceb755e03083bbf567f69bdff2896`  
		Last Modified: Wed, 10 Aug 2022 17:27:49 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a4754568b3f0299b6cd15738d87dd2af6a1d6ea15c556da9f22a6fefab5315`  
		Last Modified: Wed, 10 Aug 2022 17:28:11 GMT  
		Size: 192.7 MB (192663056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa80f2a836e03d76f4c0ab7369a7ca16280644977765322452e7c30441a720ee`  
		Last Modified: Wed, 10 Aug 2022 17:27:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
