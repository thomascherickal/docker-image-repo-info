## `julia:rc-windowsservercore`

```console
$ docker pull julia@sha256:2d3fd1f3f185de3ea00e03a47a5c3bd6eb27c17d50b1d0bbd2c551388589d868
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.825; amd64
	-	windows version 10.0.17763.3165; amd64

### `julia:rc-windowsservercore` - windows version 10.0.20348.825; amd64

```console
$ docker pull julia@sha256:b40295221fc02297b80d996ed971fcbe248b86f0cd3234cb709c9a82cc97089f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2460280279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb0d7d3adfa6552f04b37f492dd27ab917a892dbea1eec5ce87acac518da5e70`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 14:22:17 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Wed, 13 Jul 2022 14:22:18 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-rc1-win64.exe
# Wed, 13 Jul 2022 14:22:19 GMT
ENV JULIA_SHA256=f739f4fb46030df00cbaea513afd427b436fc91b6fc6d7f4e437498cd16cc2aa
# Wed, 13 Jul 2022 14:23:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Jul 2022 14:23:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e841b978414a36a669d161db72407037658758664e96942f0843f37cd89d2`  
		Last Modified: Wed, 13 Jul 2022 14:35:40 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddcf37bffb7c9ca5fede56a416f2785eca09076704fb58deae2e6663c008177`  
		Last Modified: Wed, 13 Jul 2022 14:35:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762b73a954d41deec3c60e087fce4e035db4616f68674c88385585b926bd9739`  
		Last Modified: Wed, 13 Jul 2022 14:35:40 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f40b218d3d931ba1aef64895cd5313332e770731bace75fc774db836291dad5`  
		Last Modified: Wed, 13 Jul 2022 14:36:14 GMT  
		Size: 160.0 MB (160041633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8420b4ad6759eed24c0711db18b5d91973d64a887c1bc483ebf5b49f5c60cfbe`  
		Last Modified: Wed, 13 Jul 2022 14:35:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-windowsservercore` - windows version 10.0.17763.3165; amd64

```console
$ docker pull julia@sha256:6e7c4546d5ed03e097e252d95e3157558ee3de47881a1306981b681b1ddd70d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2831796109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2af323cfe0e01f04d78531f5296c8116a12d89bb1c672528540ef341c38ecfa2`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 14:23:44 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Wed, 13 Jul 2022 14:23:45 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.8/julia-1.8.0-rc1-win64.exe
# Wed, 13 Jul 2022 14:23:46 GMT
ENV JULIA_SHA256=f739f4fb46030df00cbaea513afd427b436fc91b6fc6d7f4e437498cd16cc2aa
# Wed, 13 Jul 2022 14:25:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Jul 2022 14:25:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5df57bea7009e59c77679b58ea65203d33c96188efca2b2b00aa2aaa11055d`  
		Last Modified: Wed, 13 Jul 2022 14:36:26 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168e82b3fea3e36cf41027fd7e173c5bf64687ae78ac0c06dd6e2e4d1f18d54a`  
		Last Modified: Wed, 13 Jul 2022 14:36:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecf6981f98315f649c93892b1fc2adee252f31d927a7cb2bca5c5be70a0a04c`  
		Last Modified: Wed, 13 Jul 2022 14:36:26 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fa14e223503e51548cde52d3caffcd1a48bea0cc81a5f7739c2fc2612b8f7`  
		Last Modified: Wed, 13 Jul 2022 14:37:02 GMT  
		Size: 159.7 MB (159745321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226e74c9f9c3d727e5d705cfc09b45a353d5ce1aa4b864b5fd6a456075593e65`  
		Last Modified: Wed, 13 Jul 2022 14:36:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
