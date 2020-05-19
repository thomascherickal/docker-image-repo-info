## `hylang:python3.7-windowsservercore-1809`

```console
$ docker pull hylang@sha256:6475d36ea2fc8183f2d68718a225cf3aed62bf1013a12ee9e966b7568b318e3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `hylang:python3.7-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull hylang@sha256:2e45718ee3e9d7c27acab28c673d483f8999af276ecbbb6305d57fca28b2cf21
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1771547805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa1c231d949db3ddf6a7c97ed42b30b7bdc7a1fea3157dd1c0055bbf221cd0b`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 15:14:25 GMT
ENV PYTHON_VERSION=3.7.7
# Wed, 13 May 2020 15:14:26 GMT
ENV PYTHON_RELEASE=3.7.7
# Wed, 13 May 2020 15:15:53 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Tue, 19 May 2020 19:27:44 GMT
ENV PYTHON_PIP_VERSION=20.1.1
# Tue, 19 May 2020 19:27:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/eff16c878c7fd6b688b9b4c4267695cf1a0bf01b/get-pip.py
# Tue, 19 May 2020 19:27:46 GMT
ENV PYTHON_GET_PIP_SHA256=b3153ec0cf7b7bbf9556932aa37e4981c35dc2a2c501d70d91d2795aa532be79
# Tue, 19 May 2020 19:28:32 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 19 May 2020 19:28:33 GMT
CMD ["python"]
# Tue, 19 May 2020 19:50:40 GMT
ENV HY_VERSION=0.18.0
# Tue, 19 May 2020 19:51:13 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 19 May 2020 19:51:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e42db83b6fde9999f234181023877fdb59d6d366b1c7ba41e0dfb0ab0d7dc32`  
		Last Modified: Wed, 13 May 2020 15:20:36 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40d2b795a52909a8b19edf315eb664544da9576997b51c723a594349e9ec91e`  
		Last Modified: Wed, 13 May 2020 15:20:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cb649ec9351b1fe28f150bf68c6f9aef9abc480c2f2b297bcb339ada65b8cb`  
		Last Modified: Wed, 13 May 2020 15:21:24 GMT  
		Size: 46.6 MB (46571649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f2206e6002192aa1fd64baf1067c75e4ce73aff97a93dc90be110c40919863`  
		Last Modified: Tue, 19 May 2020 19:31:07 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9771818a9e4122d21cc51e7c87afdd7b91934bc09153b7ce68871faa8b9e25`  
		Last Modified: Tue, 19 May 2020 19:31:07 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b16f50e4fe28fa70d9b078bc2bb676a50e915218abd2b9dfb782abd3f4eefc7`  
		Last Modified: Tue, 19 May 2020 19:31:07 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5915f8087cd9a4fc31827024356e20b892953e51c09f651188868573e7513f5`  
		Last Modified: Tue, 19 May 2020 19:31:14 GMT  
		Size: 5.5 MB (5480128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d785033661339fe0e2ecbef3378249788f1bc7187c53123753e59bbf69fd89`  
		Last Modified: Tue, 19 May 2020 19:31:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101e9acdc3225e8d7b70cb2e97e744c5229ebb5d07b56d2fe1ccf37d3e31ea96`  
		Last Modified: Tue, 19 May 2020 19:54:29 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f1b7ebb34526400e2491f6e6ca65fe18e0b6446917b3a2568bdaebf60a491f`  
		Last Modified: Tue, 19 May 2020 19:54:30 GMT  
		Size: 1.2 MB (1152856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f27aa1bd9feac914325b76910ded6f7decddc71588afce45f5f9941cd2bc32c`  
		Last Modified: Tue, 19 May 2020 19:54:29 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
