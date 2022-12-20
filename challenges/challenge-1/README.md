<p align="center"> 
  <img width=60% src=../../images/challenge-1.png/>
</p>

<h1 align="center">🎁 Reto #1: <em>¡Automatizando envolver regalos de navidad!</em> 🎅🏻</h1>

<p style="background:LimeGreen; border-radius:20px; width:60px; text-align:center; font-weight:600; margin: 0 auto; padding:0 5px; font-size:14px">Fácil</p>

## Instrucciones

Este año los elfos han comprado una máquina que envuelve regalos. Pero... ¡no viene programada! Necesitamos crear un algoritmo que le ayude en la tarea.

A la máquina se le pasa un array con los regalos. Cada regalo es un string. Necesitamos que la máquina envuelva cada regalo en papel de regalo y lo coloque en un array de regalos envueltos.

El papel de regalo es el símbolo `*` y para envolver un regalo se coloca el símbolo `*` de forma que rodee totalmente al string por todos los lados. Por ejemplo:

```
const gifts = ['book', 'game', 'socks']
const wrapped = wrapping(gifts)

console.log(wrapped)

/*
  [
    "******\n*book*\n******",
    "******\n*game*\n******",
    "*******\n*socks*\n*******"
  ]
*/
```

Como ves, el papel de regalo envuelve el string. Por arriba y por abajo, para no dejar ningún hueco, las esquinas también están cubiertas por el papel de regalo.

**Nota:** El carácter `\n` representa un salto de línea.

**¡Ojo!** Asegúrate que pones el número correcto de `*` para envolver completamente el string.

Ah, y **no modifiques (mutes) el array original.**