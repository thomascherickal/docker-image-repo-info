## `eclipse-temurin:20-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:b122f2243056fae491fd6b1971c3e5478c4dd068d2e101283354c61ab0cb0177
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `eclipse-temurin:20-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull eclipse-temurin@sha256:dc94d384fec67480b9ce98db5a7f639da8a2646b6949c69e42734d299ce6ae24
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2144867056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0067726fd2be3fd0fc48ba7d6a01cb34fb744828379013d759a38c721262c343`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:04:02 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 10 May 2023 01:05:02 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jdk_x64_windows_hotspot_20.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jdk_x64_windows_hotspot_20.0.1_9.msi ;     Write-Host ('Verifying sha256 (8cd9abe9b188ef11f976c854e181c932c84aa15a44b94144e4b472990764229c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8cd9abe9b188ef11f976c854e181c932c84aa15a44b94144e4b472990764229c') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-20' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 May 2023 01:05:26 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 10 May 2023 01:05:27 GMT
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
	-	`sha256:6ea79297797be3714ba8d07431560ddff07237b2f971b0b44db0c144814ec2b5`  
		Last Modified: Wed, 10 May 2023 07:01:27 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5844ffefab15d7215e2afcaf42d811b55a871da736e4306e2d68b6ad2e55470b`  
		Last Modified: Wed, 10 May 2023 07:01:53 GMT  
		Size: 369.6 MB (369603433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc96ae3f72b261085e3160293d4bccfa7ed165aafd5c0b6f6ec2961409747d`  
		Last Modified: Wed, 10 May 2023 07:01:27 GMT  
		Size: 277.9 KB (277882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd02f0d7c6984360e6e27814b06975dbcae0cecbb5cde6147f950cdb3fffc9c`  
		Last Modified: Wed, 10 May 2023 07:01:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
