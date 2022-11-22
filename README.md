# spring-boot-jwt-JPA

Esimerkki on kopioitu sivulta https://www.javainuse.com/spring/boot-jwt-mysql#google_vignette

Tein siihen pieniä muutoksia saadakseni sen toimimaan Mavenilla.

## Esimerkin kokeilu

<ol>
<li>Anna projektin juuressa komento mvnw clean spring-boot:run</li>
<li>Kokeile Postmanilla Get requestia http://localhost:8080/hello</li>
<li>Kokeile Postmanilla Post requestia http://localhost:8080/register ja kirjoita body-osaan (raw/json) 
<pre>
{
    "username":"user01",
    "password":"pass01"
}
</pre>
</li>
<li>Kokeile Postmanilla Post requestia http://localhost:8080/authenticate ja kirjoita body-osaan (raw/json) 
<pre>
{
    "username":"user01",
    "password":"pass01"
}
</pre>
</li>
<li>Kokeile Postmanilla uudestaan Get requestia http://localhost:8080/hello, mutta laita edellä saamasi webtoken requestin Authenticate osioon (Bearer)</li>
</ol>