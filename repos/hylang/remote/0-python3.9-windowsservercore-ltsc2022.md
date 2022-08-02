## `hylang:0-python3.9-windowsservercore-ltsc2022`

```console
$ docker pull hylang@sha256:7114c0f638217b16a0b71a43c53043a6f10e696566b63b7f8877295eed69cc27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `hylang:0-python3.9-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull hylang@sha256:450b9c8f7361add4dd638b80d1eedf6903629aed0b83199724eecc4b2fd9429c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2360620236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7407b92cca94836760ffb8d3f7e7e00d92ead200021465cb103721cb43f800e6`
-	Default Command: `["hy"]`
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
# Tue, 12 Jul 2022 20:50:00 GMT
ENV PYTHON_VERSION=3.9.13
# Tue, 12 Jul 2022 20:51:18 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 12 Jul 2022 20:51:19 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 12 Jul 2022 20:51:20 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 02 Aug 2022 20:24:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Tue, 02 Aug 2022 20:24:45 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Tue, 02 Aug 2022 20:25:28 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 02 Aug 2022 20:25:29 GMT
CMD ["python"]
# Tue, 02 Aug 2022 20:46:56 GMT
ENV HY_VERSION=0.24.0
# Tue, 02 Aug 2022 20:46:57 GMT
ENV HYRULE_VERSION=0.2
# Tue, 02 Aug 2022 20:48:04 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Tue, 02 Aug 2022 20:48:05 GMT
CMD ["hy"]
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
	-	`sha256:090ce0c092147a617936f3f964fb55f8bd2930749dc550642dbc5d65f33b8f6d`  
		Last Modified: Tue, 12 Jul 2022 20:57:58 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fca5498c8a0c78b9b210db675489ce5e7a2a843930d82da78dd23cda2dabea9`  
		Last Modified: Tue, 12 Jul 2022 20:58:05 GMT  
		Size: 52.0 MB (51982748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29619e5e28282b5438d24f3da90273aafb5b1e5630c96f3eaafe80a26ea770aa`  
		Last Modified: Tue, 12 Jul 2022 20:57:58 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc454d63f220b0999f197261db2a80c712afc3d327d9a6d80eb8f2a68e4da259`  
		Last Modified: Tue, 12 Jul 2022 20:57:56 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be0660894606aeb6d09c3ce5408c43cf6e9cfd3ef232cdef57a23ec4e7b11c9`  
		Last Modified: Tue, 02 Aug 2022 20:29:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27320b1a71a36aad331aac1af68d8b642fe2de4a9a7a8ea492b3c32236e7fb7e`  
		Last Modified: Tue, 02 Aug 2022 20:29:20 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb475264f0149cf016a22771d06c38eee49ad9dff0ea01500a24f3d6e3b65d9`  
		Last Modified: Tue, 02 Aug 2022 20:29:21 GMT  
		Size: 3.7 MB (3747390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28d128a05805df395e10e1af284529bd62f7bccf2a1c1b1db3d0d44b4416ffd`  
		Last Modified: Tue, 02 Aug 2022 20:29:20 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce30e0be91cd23ea9178be2d425690cfed3960e7a4f9203ae50f5fe35bb86bb`  
		Last Modified: Tue, 02 Aug 2022 20:51:57 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b0f459c0952954369a5e2a8ee71f9e9781c74f036dc4b6e16bf25e4a4bd11b`  
		Last Modified: Tue, 02 Aug 2022 20:51:56 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87da2742cfd0adbb0df91c4e10e567fb7bad7e580599b25a688c1c913d8241aa`  
		Last Modified: Tue, 02 Aug 2022 20:51:58 GMT  
		Size: 4.6 MB (4643027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1baa8c7dd73a0b2a6b45e5757200e6eade0824076443a1c8d2e914fa7eb60da`  
		Last Modified: Tue, 02 Aug 2022 20:51:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
