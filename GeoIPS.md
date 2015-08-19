# Introducción #

Geo IPS es un software que permite definir reglas de acceso a puertos TCP/UDP en base a la procedencia geográfica de las conexiones.

Ejemplos típicos de uso puede ser filtrar el acceso al servicio SSH a conexiones cuyo origen sea un Pais o Ciudad.


# Plataforma #

Geo IPS debería funcionar en cualquier Linux con una versión de Perl moderna y teóricamente en sistemas **BSD**

# Instalación #

Pasos de instalación hechos en una Fedora Core 11

**1) Instalación de los módulos Perl necesarios**

 Cormo root

#perl -MCPAN -e shell

(una vez dentro de la shell CPAN)

cpan> install YAML

cpan> install DBI

`cpan> install DBD::SQLite`

`cpan> install Net::PcapUtils`

`cpan> install NetPacket::Ethernet`

`cpan> install XML::Simple`

**2) Instalación de Geo::IP**

De aquí http://geolite.maxmind.com/download/geoip/api/c/ descargamos las librerías en C

# wget http://geolite.maxmind.com/download/geoip/api/c/GeoIP-1.4.6.tar.gz

# tar -xvzf GeoIP-1.4.6.tar.gz

# cd GeoIP-1.4.6

(En este punto, tal vez debas instalar las librerias Zlib)

# yum install zlib-devel

# ./configure

# make

# make install

Ahora, descargamos el modulo Perl desde aquí http://geolite.maxmind.com/download/geoip/api/perl/

# wget http://geolite.maxmind.com/download/geoip/api/perl/Geo-IP-1.38.tar.gz

# tar -xvzf Geo-IP-1.38.tar.gz

# cd Geo-IP-1.38

# perl Makefile.PL

# make

# make test

# make install

**3) Instalación de GeoIPS**

Descargamos el software

# wget http://sbdtools.googlecode.com/files/GeoIPS1.0.tgz

# tar -xvzf GeoIPS1.0.tgz

# cd GeoIPS/

Descargamos la base de datos de Geolocalización de Max Mind

wget http://geolite.maxmind.com/download/geoip/database/GeoLiteCity.dat.gz

`# gzip -d GeoLiteCity.dat.gz`

Y con esto, estaría completado el proceso de instalación







