# nomenclaturaMAC
'''
Se necesitaba cambiar la seguridad NAC de todos los puertos de la TORRE BBVA REFORMA con el servicio de CCTV (puesto que estos equipos no soportan la carga de certificados
para la autenticación por 802.1X) y posterior a ello, dar de alta en Cisco Identity Services Engine todas las MAC-Address, evidentemente se trataban de muchos equipos y 
por ende demasiadas MAC-Address, mediante PuTTY se observa que la sintaxis de el SO de los Switches muestra las direcciones de la manera "abcdef-123456" y otros modelos
con distinto SO de la manera "abcd-ef12-3456", sin embargo para que los equipos logren autenticar a nivel TACACS, se deben de dar de alta en 
Cisco Identity Services Engine para que su servidor RADIUS los conozca y logre autenticarlos por medio de la MAC-Address . dicha herramienta solo acepta las
direcciones de la forma tradicional "ab:cd:ef:12:34:56" derivado de todo esto propuse darme un pequeño lapse de tiempo, para crear un programa que nos ahorrase 
el interminable trabajo y tiempo de ir cambiando el formato de las más de 300 direcciones MAC mano a mano...
'''
