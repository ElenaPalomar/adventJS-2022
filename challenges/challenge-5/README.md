</br>
<p align="center"> 
  <img width=40% src=../../images/challenge-5.png/>
</p>

<h1 align="center">🎁 Reto #5: <em>Optimizando viajes de Santa</em> 🌆</h1>

## Instrucciones - [![](https://img.shields.io/badge/-Difícil-C0392B?style=plastic)]()

Para no cansar a los renos, Papá Noel quiere dejar el máximo número de regalos haciendo el menor número posible de viajes.

Tiene un array de ciudades donde cada elemento es el número de regalos que puede dejar allí. `[12, 3, 11, 5, 7]`. Por otro lado, el límite de regalos que caben en su saco. Y, finalmente, el número de ciudades máximo que sus renos pueden visitar.

Como no quiere dejar una ciudad a medias, **si no puede dejar todos los regalos que son de esa ciudad, no deja ninguno allí.**

Crea un programa que le diga **la suma más alta de regalos** que podría repartir teniendo en cuenta el máximo de regalos que puede transportar y el número máximo de ciudades que puede visitar:

```
const giftsCities = [12, 3, 11, 5, 7]
const maxGifts = 20
const maxCities = 3

// la suma más alta de regalos a repartir
// visitando un máximo de 3 ciudades
// es de 20: [12, 3, 5]

// la suma más alta sería [12, 7, 11]
// pero excede el límite de 20 regalos y tendría
// que dejar alguna ciudad a medias.

getMaxGifts(giftsCities, maxGifts, maxCities) // 20
```

Si no se puede realizar ningún viaje que satisface los requerimientos, el resultado debe ser `0`. Más ejemplos:

```
getMaxGifts([12, 3, 11, 5, 7], 20, 3) // 20
getMaxGifts([50], 15, 1) // 0
getMaxGifts([50], 100, 1) // 50
getMaxGifts([50, 70], 100, 1) // 70
getMaxGifts([50, 70, 30], 100, 2) // 100
getMaxGifts([50, 70, 30], 100, 3) // 100
getMaxGifts([50, 70, 30], 100, 4) // 100
```

Cosas a tener en cuenta y consejos:

- `maxGifts >= 1`
- `giftsCities.length >= 1`
- `maxCities >= 1`
- El número de `maxCities` puede ser mayor a `giftsCities.length`