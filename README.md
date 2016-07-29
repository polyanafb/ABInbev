# abiServicesTest
Repositório usado para ABI - tese de conhecimento

# Services ABI

This project accesses external apis to recover informations like variation of the European currency, artists or tracks and movies.

### Prerequisities

Mulesoft Anypoint studio  6.0.1 instaled - Available to download at https://www.mulesoft.com/platform/studio
API access and valid keys - Movies DB, Last FM and ApiLayer - You need make the register in each API using the links below. 
https://www.themoviedb.org/
http://www.last.fm/
https://apilayer.com/

## Running the tests

To call the integrations you need to send some parameters.
ApiLayer: startdate and enddate parameters. Format: yyyy-mm-ss
LastFM: artist and track parameters
MovieDB: no parameters is necessary
Examples (If you are testing already in the cloudhub, you need to use the cloudhub url. No more localhost.):
ApiLayer:http://localhost:8080/getcurrency?startdate=2016-04-01&enddate=2016-04-04
LastFM: http://localhost:8080/getlastfminfo?artist=cher&track=believe
MovieDB: http://localhost:8080/getmovie

## Deployment

1.Download the zip file here "app_servicesabi.zip".
2.Sign in the cloudhub. https://anypoint.mulesoft.com/login/#/signin
3.Create a new application
4.Upload zip file.
5.Fill all settings.
6. Fill the properties with the same properties you have into mule-app.properties - Available in 
7.Apply.
8. After it's uploaded, start the service.

## Built With

*Anypoint Studio 6.0.1 

## Versioning

For the versions available, see the GitHub. Test-knowledge-Products branch.

## Authors

* **Polyana Fernandes**

## Acknowledgments

* Integration
* REST and HTTP
* Mulesoft and MEL
