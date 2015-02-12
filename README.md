#Csforge Public Maven repository

##Usage

- **pom.xml**:

		<repositories>
		    <repository>
		        <id>csforge-snapshots</id>
		        <url>https://github.com/csforge/public-mvn-repo/raw/master/snapshots</url>
		    </repository>
	 	</repositories> 

##Delopy and Install Repo

- Type **mvn** command in opensource root directory:

		mvn install -DcreateChecksum=true

- Generate sources.jar:

		mvn source:jar install -DcreateChecksum=true

- Copy all mvn generate files with directories from local **.m2** directory to your  ***public-mvn-repo*** clone directory, bellow *snapshots* or *releases* subdirectory.

- **Git** push in ***public-mvn-repo*** clone directory:

		git push origin master
	  