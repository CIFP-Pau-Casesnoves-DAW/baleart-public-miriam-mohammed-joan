Ruta de la API (Conté la taula amb l'ajuda):
http://baleart.projectebaleart.com/public/

Exemple de consulta: http://baleart.projectebaleart.com/public/api/municipis

Per a crear un usuari i fer login no fa falta emprar token, però per a la resta de peticions serà necessari emprar el token que retorna el login.
Format del token -> Bearer token
![imagen](https://user-images.githubusercontent.com/55986837/153614400-78034440-c406-4b25-bb9d-d34c3e1cd462.png)

(El token es valid durant 30min, en passar aquest temps s'haurà de fer el login de nou)
