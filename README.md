# delitos-chile-data
Rest Api de delitos para el repositorio: https://github.com/alexbgh1/delitos-chile/

## Preview

[Ejemplo .json](https://alexbgh1.github.io/delitos-chile-data/data/Delitos%20de%20mayor%20connotaci%C3%B3n%20social.json)

![Ejemplo .json](https://i.imgur.com/3CTHq88.png)

## Ejemplo fetching data

```javascript

const endpoint = "https://alexbgh1.github.io/delitos-chile-data/data"

const fetchData = async () =>{
try {
// group_crime corresponde al grupo delictual del delito (puedes revisarlos en el mismo repositorio en la carpeta /data/)
  const response = await fetch(`${endpoint}/${group_crime}.json);
  const data = await response.json();
  // Filtrar o utilizar data aquí ...

  } catch(error){
    console.log(error)
  }
}
```
