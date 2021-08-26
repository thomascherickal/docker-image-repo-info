## `eclipse-temurin:11-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:78b88acd81f3ed5926bd7a2369a812a98ef2856b042d6777158209153b05eb42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `eclipse-temurin:11-jdk-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull eclipse-temurin@sha256:bb3ef34d859d4dfb57cce63d4f8c21a581b6de70a5cfdbbe65051b12bbc98807
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3051935246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df05e2c0bfd85814e2201c788a14fcd49194d065c48291f788be7b55bf4e688`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 16:39:51 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Wed, 25 Aug 2021 16:41:24 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.12_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.12_7.msi ;     Write-Host ('Verifying sha256 (80546d8a36ad0cdf69305f72f42465093b9d0388f45819b05cc640ecd1310b32) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '80546d8a36ad0cdf69305f72f42465093b9d0388f45819b05cc640ecd1310b32') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 25 Aug 2021 16:42:21 GMT
RUN Write-Host 'Verifying install ...';     Write-Host '  javac --version'; javac --version;     Write-Host '  java --version'; java --version;         Write-Host 'Complete.'
# Wed, 25 Aug 2021 16:42:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70b5ef22de7973c9cc52b8012a28cea074c31c106e0ae83baeffc793404cdeb`  
		Last Modified: Wed, 25 Aug 2021 23:25:01 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f681114403bc0c429f3cd5a771e9d7611c3b48fcf08209d49bb43190a67349`  
		Last Modified: Wed, 25 Aug 2021 23:31:28 GMT  
		Size: 365.6 MB (365589366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd41c04673ab6b13501bf6146d91a09fb089d09d2e55aa335f65014fcd31803a`  
		Last Modified: Wed, 25 Aug 2021 23:25:01 GMT  
		Size: 343.8 KB (343821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0468f06b88789bb4d899597d70ce75d47dbd913b92a974ddd9e9cc7ed722c`  
		Last Modified: Wed, 25 Aug 2021 23:25:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
