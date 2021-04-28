## `python:windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:d1a4a5d631963a8c6236392f04a4fb0be4629fec32129ad8308739852bb3ffa4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `python:windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull python@sha256:cb8201be9ce382a9cd78d7d8c5bb507418dd91b230005d805bfc6a3a9eaa9dc4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5865637171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:824ea4effe6ed1e4c47728cb193629b442c45dedf5a3b4e1ed886f5a9b48a4a9`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 16:15:18 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 14 Apr 2021 16:24:02 GMT
ENV PYTHON_VERSION=3.9.4
# Wed, 14 Apr 2021 16:24:03 GMT
ENV PYTHON_RELEASE=3.9.4
# Wed, 14 Apr 2021 16:26:37 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 27 Apr 2021 22:18:40 GMT
ENV PYTHON_PIP_VERSION=21.1
# Tue, 27 Apr 2021 22:18:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ab9dde151f662745c13461f00c453dcf32a51ea9/public/get-pip.py
# Tue, 27 Apr 2021 22:18:42 GMT
ENV PYTHON_GET_PIP_SHA256=0ed17e859b835ad5bf00851f4dc8bbc3520c13dfff6c131d410cdb3a92ff0af9
# Tue, 27 Apr 2021 22:20:22 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 27 Apr 2021 22:20:23 GMT
CMD ["python"]
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
	-	`sha256:32b4598ab88dab64b25b4257872564af9825cc6cd41fc8cc1ad11c32958d0da9`  
		Last Modified: Wed, 14 Apr 2021 16:39:38 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3902851ebd791590e71166e85429e5b052b7772ac7ff02c5b24d9ccdbcb4a932`  
		Last Modified: Wed, 14 Apr 2021 16:41:32 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6a84a844f2697f99daf89fbb5fb464dcc3fb6077890a4199e32b912969ef87`  
		Last Modified: Wed, 14 Apr 2021 16:41:32 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6114df8d320bdd1859f3b1d082e3498e5cca294b92388d492fc78efb6306f082`  
		Last Modified: Wed, 14 Apr 2021 16:41:45 GMT  
		Size: 59.3 MB (59260692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35c53aa45d445aa920f9160e68fb4349609c97c08d5852276bb754fc1d99c97`  
		Last Modified: Tue, 27 Apr 2021 22:25:37 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fdfa979f77efcdf6d15c58d6c161d9db5d846b82085325f3f0b110b9e0bd0e`  
		Last Modified: Tue, 27 Apr 2021 22:25:36 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771ad1c50f028de06a3625dbe83acfa31f77b04b3199c67acd86cc07b38682a0`  
		Last Modified: Tue, 27 Apr 2021 22:25:36 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204577b7a89806d9822c6a778e5692d02089d8eb8c433137c09c42836c1c3cf4`  
		Last Modified: Tue, 27 Apr 2021 22:25:50 GMT  
		Size: 11.5 MB (11481535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b5a86d9a21cd97bc74b9b7ae42c4c29c3f48303936f65157589e6e5ddef401`  
		Last Modified: Tue, 27 Apr 2021 22:25:36 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
