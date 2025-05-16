---
theme: ./theme/style.json
author: Roberto Alvarado
paging: Slide %d / %d
---

                     _                                  _       __     ___           
                    | |    ___ _ __   __ _ _   _  __ _ (_) ___  \ \   / (_)_ __ ___  
                    | |   / _ \ '_ \ / _` | | | |/ _` || |/ _ \  \ \ / /| | '_ ` _ \ 
                    | |__|  __/ | | | (_| | |_| | (_| || |  __/   \ V / | | | | | | |
                    |_____\___|_| |_|\__, |\__,_|\__,_|/ |\___|    \_/  |_|_| |_| |_|
                                     |___/           |__/                            
                          
                          



                  Entendiendo como hablar a Vim


---

# Comandos generales

### Como cambiar de un estado a otro

Modo command o normal es el primer estado que se encuentra el editor

                        ------->
                                      <Esc>                       v
                        |Insert|-----------------|Normal| -------------------|Visual|
                                        i                         <Esc>
                                                                            <--------

¡No son la unica forma de cambiar entre estados!
---
# Comandos generales

### Guardar los cambios
                      :w <file-name>
### Salir de Vim
                      :q
### Abrir un nuevo archivo en Vim
                      :e <file-name>

---
## Como movernos en vim 

Primer Paso: DEJAR A UN LADO LAS FLECHAS

¿Por qué? __Buscamos la máxima eficiencia__

```
~~~graph-easy --as=boxart
[ Fleclas ] --> [ hjkl ]
~~~
```
                                              ﰵ
                                   ---       ---       ---        ---
                                 | h |     | j |     | k |      | l | 
                                   ---       ---       ---        ---
                                                        
---

# El lengsuaje de Vim


Imaginemos que queremos hacer una acción en vim, por ejemplo, queremos borrar una palabra.

En el lenguaje de Vim vamos a hacer uso de una estructura de verb + adjective + noun

```
~~~graph-easy --as=boxart
[ Acción ] -- [ Contador ] -- [ Objeto ]
[ Verb ] -- [ Adjetive ] -- [ Noun ]
~~~
```
Es similar a la estructura que utilizamos al hablar de sujeto y predicado


                                Delete 3 words -> d3w
                                Change 4 letters -> c4l
                                Yank 2 words -> y2s

---

# Acciones (Verbs)


                          d   -> Delete
                          c   -> Change
                          >|< -> Indent
                          v   -> Visual select
                          y   -> Yank (Copy)

# Objetos (Text objects)
                          w ->  word
                          t ->  tag
                          " ->  quotes
                          p ->  paragraph

---




