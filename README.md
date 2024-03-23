docker build -f Dockerfile_apache -t web100 . - zbudowanie obrazu o nazwie web100 na podstawie pliku Dockerfile_apache

docker run -d -p 80:8080 --name strona_apache web100 - uruchomienie kontenera o nazwie strona_apache na bazie obrazu web100 w trybie detach (w tle) z mapowaniem portu 80 hosta na port 8080 wewnątrz kontenera

Po uruchomieniu kontenera należy włączyć przeglądarkę i wpisać localhost.