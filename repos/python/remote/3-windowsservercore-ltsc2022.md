## `python:3-windowsservercore-ltsc2022`

```console
$ docker pull python@sha256:cf357e769124547c6f1a44e291d98c5b55528bf9aaac62909135840e6e220869
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `python:3-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull python@sha256:8ee7f3e5e8e5f0130d779c4ca5b433abba64a81c4a5f650ed25dd70f143acded
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2352686007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c65fad9ad00a572d68c9de5de587ba0372674f82f10b886c12ee29279969b3f`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 20:35:01 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 12 Jul 2022 20:43:45 GMT
ENV PYTHON_VERSION=3.10.5
# Tue, 12 Jul 2022 20:45:01 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 12 Jul 2022 20:45:02 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 12 Jul 2022 20:45:04 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 26 Jul 2022 23:21:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/49ca29908cfd49683da12f2d5a4fa5689539f9d9/public/get-pip.py
# Tue, 26 Jul 2022 23:21:39 GMT
ENV PYTHON_GET_PIP_SHA256=d077d469ce4c0beaf9cc97b73f8164ad20e68e0519f14dd886ce35d053721501
# Tue, 26 Jul 2022 23:22:27 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 26 Jul 2022 23:22:28 GMT
CMD ["python"]
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
	-	`sha256:9ef330eb8cab3834d9737ff92915047264f01ac2d39da71a4aa5e63eddef3204`  
		Last Modified: Tue, 12 Jul 2022 20:56:31 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3ed561c4f8056db1802084150986eb17bed901b15f45470d6e430e32c9fa95`  
		Last Modified: Tue, 12 Jul 2022 20:57:10 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458a04bb6d463880fdf62e44cd4df0f44ece479d179c59c64d66b14ea3a21544`  
		Last Modified: Tue, 12 Jul 2022 20:57:17 GMT  
		Size: 48.7 MB (48695923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d136e826624e9948136a52e5d0896c139d90099647b07d064a801e134a00d2`  
		Last Modified: Tue, 12 Jul 2022 20:57:10 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1223df38d594adb8331acc96dadc02186ea6ca9869af4025c8ec9c3920001072`  
		Last Modified: Tue, 12 Jul 2022 20:57:08 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28563015dd682cee139bf7d6e6af48662b03c42e6a7e68f0f4408c3862fb4f4`  
		Last Modified: Tue, 26 Jul 2022 23:28:25 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dbe8a80b9c4175417b0e2db2bd50eec1d203e494e1a76973ca2b104e3b25f8`  
		Last Modified: Tue, 26 Jul 2022 23:28:25 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b189d036a1054467dfdc5030422c7fbc21dcaab8e1f94ecd041f6615777c3034`  
		Last Modified: Tue, 26 Jul 2022 23:28:27 GMT  
		Size: 3.7 MB (3747349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340ee2af64e45496bd0148fa89d279e7f037cd6b2ce1b4a1347ded7877927f47`  
		Last Modified: Tue, 26 Jul 2022 23:28:25 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
