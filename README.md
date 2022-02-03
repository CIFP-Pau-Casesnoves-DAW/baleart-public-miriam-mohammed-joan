Ruta de la API:
http://baleart.projectebaleart.com/public/

Exemple de consulta: http://baleart.projectebaleart.com/public/api/municipis

municipis	GET		/municipis		    Retorna tots els municipis	
municipis	GET		/municipis/{id}	    Retorna un municipi en concret	
municipis	POST	/municipis		    Crea un nou municipi	                        nom_municipi, illa
municipis	PUT		/municipis/{id}	    Modifica algun atribut de municipis	            nom_municipi, illa
municipis	DELETE	/municipis/{id}	    Esborra un municipi	
    
tipus		GET		/tipus			    Retorna tots els tipus	
tipus		GET		/tipus/{id}		    Retorna un tipus en concret	
tipus		POST	/tipus			    Crea un nou tipus	                            nom_tipus, descripcio_tipus_es, descripcio_tipus_ca, descripcio_tipus_en
tipus		PUT		/tipus/{id}		    Modifica algun atribut de tipus	                nom_tipus, descripcio_tipus_es, descripcio_tipus_ca, descripcio_tipus_en
tipus		DELETE	/tipus/{id}		    Esborra un tipus	
    
serveis		GET		/serveis		    Retorna tots els serveis	
serveis		GET		/serveis/{id}	    Retorna un servei en concret	
serveis		POST	/serveis		    Crea un nou servei	                            nom_servei, descripcio_servei_es, descripcio_servei_ca, descripcio_servei_en
serveis		PUT		/serveis/{id}	    Modifica algun atribut de serveis	            nom_servei, descripcio_servei_es, descripcio_servei_ca, descripcio_servei_en    
serveis		DELETE	/serveis/{id}	    Esborra un servei	
    
espais		GET		/espais			    Retorna tots els espais	
espais		GET		/espais/{id}	    Retorna un espai en concret	
espais		POST	/espais			    Crea un nou espai	                            id_usuari, id_tipus, id_municipi, id_servei, id_obra, nom_espai, direccio, email, telefon, web, descripcio_espai_es, descripcio_espai_ca, descripcio_espai_en, imatge
espais		PUT		/espais/{id}	    Modifica algun atribut de espais	            id_usuari, id_tipus, id_municipi, id_servei, id_obra, nom_espai, direccio, email, telefon, web, descripcio_espai_es, descripcio_espai_ca, descripcio_espai_en, imatge
espais		DELETE	/espais/{id}	    Esborra un espai	

autors		GET		/autors			    Llistat de tots els autors de la base de dades	
autors		GET		/autors/{id}	    Retorna un autor donat el seu ID	
autors		POST	/autors			    Crea un nou autor a la base de dades	        nom_autor, llinatges, nacionalitat, biografia
autors		PUT		/autors/{id}	    Modifica un autor donat el seu ID	            nom_autor, llinatges, nacionalitat, biografia
autors		DELETE	/autors/{id}	    Borra un autor donat el seu ID	
				
exposicions	GET		/exposicions	    Llistat de totes les exposicions de la base de dades	
exposicions	GET		/exposicions/{id}	Retorna una exposició donat el seu ID	
exposicions	POST	/exposicions	    Crea una nova exposició a la base de dades	    id_espai, titol_expo, data_inici, data_fi, descripcio_expo_es, descripcio_expo_ca, descripcio_expo_en
exposicions	PUT		/exposicions/{id}	Modifica una exposició donat el seu ID      	id_espai, titol_expo, data_inici, data_fi, descripcio_expo_es, descripcio_expo_ca, descripcio_expo_en
exposicions	DELETE	/exposicions/{id}	Borra una exposició donat el seu ID	
				
modalitats	GET		/modalitats	        Llistat de totes les modalitats de la base de dades	
modalitats	GET		/modalitats/{id}	Retorna una modalitat donat el seu ID	
modalitats	POST	/modalitats	        Crea una nova modalitat a la base de dades	    nom_modalitat, descripcio_modalitat_es, descripcio_modalitat_ca, descripcio_modalitat_es
modalitats	PUT		/modalitats/{id}	Modifica una modalitat donat el seu ID	        nom_modalitat, descripcio_modalitat_es, descripcio_modalitat_ca, descripcio_modalitat_es
modalitats	DELETE	/modalitats/{id}	Borra una modalitat donat el seu ID	
				
obres	    GET	    /obres  	        Llistat de totes les obres de la base de dades	
obres	    GET	    /obres/{id}	        Retorna una obra donat el seu ID	
obres	    POST	/obres	            Crea una nova obra a la base de dades	        id_autor, id_exposicio, id_modalitat, titol, any_data, fotografia, descripcio_obra_es, descripcio_obra_ca, descripcio_obra_en
obres	    PUT 	/obres/{id}	        Modifica una obra donat el seu ID	            id_autor, id_exposicio, id_modalitat, titol, any_data, fotografia, descripcio_obra_es, descripcio_obra_ca, descripcio_obra_en
obres	    DELETE	/obres/{id}	        Borra una obra donat el seu ID	        

usuaris	    GET	    /usuaris	        Retorna tots els usuaris	
usuaris	    GET	    /usuaris/{id}	    Retorna un tipu de usuari	
usuaris	    GET	    /usuaris	        Crea un usuari nou	                            nom_usuari , cognoms ,email_usuari ,telefon_usuari , password , registrat_desde 
usuaris	    POST	/usuaris/{id}	    Modifica un usuari	                            nom_usuari , cognoms ,email_usuari ,telefon_usuari , password , registrat_desde 
usuaris	    POST	/usuaris/{id}	    borrar usuaris	
    
comentaris	GET	    /comentaris	        Retorna tots els comentaris	
comentaris	GET	    /comentaris/{id}	Retorna un comentari de un espai	
comentaris	GET	    /comentaris	        Crea un comentari	                            id_usuari,id_espai,comentari ,data 
comentaris	POST	/comentaris/{id}	Modifica un comentari	                        id_usuari,id_espai,comentari ,data 
comentaris	POST	/comentaris/{id}	borra comentaris	
				
valoracions	GET 	/valoracions	    Retorna totes les valoracions	
valoracions	GET 	/valoracions/{id}	Retorna una valoracio de un espai	
valoracions	GET 	/valoracions	    Crea una valoracio	                            id_usuari,id_espai ,puntuacio 
valoracions	POST	/valoracions{id}	Modifica una valoracio                      	id_usuari,id_espai ,puntuacio 
valoracions	POST	/valoracions/{id}	borra valoracions	