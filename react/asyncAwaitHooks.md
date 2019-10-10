# Fetching API data in React and es6

```js

const [pets, setPets] = useState([])

async function requestPets() {
    const {animals} = await pet.animals({
        location, 
        breed, 
        type: animal
    })
}

setPets(animals || [])

// say if you had a form with a submit button you would then do the following 

<form onSubmit={(e)=> {
    e.preventDefault();
    requestPets()
}}>


```

the async function means that it will return a promise. Once await promise is fulfilled we can setPets 
to the results now stored in the variable that we destructured with the animals. 