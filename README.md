# CheckRedirectByUserAgent
Check Redirect by User Agents in txt file

## Usage

`node CheckRedirectByUserAgent.js [URL] [URL_ESPERADA_PARA_EL_REDIRECT FICHERO_CON_USER_AGENTS] [USAR_DELAY_ENTRE_LLAMADAS] [TIEMPO_ENTRE_LLAMADAS_EN_MILISEGUNDOS] [NUMERO_DE_URLS_EN_CADA_LLAMADA]`     

  
## Ejemplos  
1. Usar los valores por defecto dentro del fichero CheckRedirectByUserAgent.js:  
`node CheckRedirectByUserAgent.js`  

* URL =  https://www.duckduckgo.com/  
* URL_ESPERADA_PARA_EL_REDIRECT =  https://duckduckgo.com/    
* FICHERO_CON_USER_AGENTS USAR_DELAY_ENTRE_LLAMADAS = true  
* TIEMPO_ENTRE_LLAMADAS_EN_MILISEGUNDOS = 600  
* NUMERO_DE_URLS_EN_CADA_LLAMADA = 10  

2. Usar todos los valores por defecto menos las URLs:  
`node CheckRedirectByUserAgent.js https://www.duckduckgo.com/ https://duckduckgo.com/`   

3. Usar todos los valores por defecto menos las URLS y el fichero de UserAgents:
`node CheckRedirectByUserAgent.js https://www.duckduckgo.com/ https://duckduckgo.com/ UserAgentsListIPad.txt`   

4. Lanzar todas las peticiones de golpe:  
`node CheckRedirectByUserAgent.js https://www.duckduckgo.com/ https://duckduckgo.com/ UserAgentsListIPad.txt false` 

5. Lanzar 1 petición cada 5000ms:  
`node CheckRedirectByUserAgent.js https://www.duckduckgo.com/ https://duckduckgo.com/ UserAgentsListIPad.txt true 5000 1`
