Pokémon API Documentation

This API allows users to manage Pokémon and their owners. The following endpoints are available:

Get All Pokémon

- Method: GET
- Endpoint: /pokemon
- Description: Returns a list of all Pokémon

Add Pokémon

- Method: POST
- Endpoint: /pokemon
- Description: Creates a new Pokémon
- Request Body:
    - ownerId (string)
    - pokemonName (string)
    - pokemonAbility (string)
    - noOfPokemon (number)

Add Pokémon to User

- Method: POST
- Endpoint: /pokemon/:ownerName/add
- Description: Adds a Pokémon to a user's collection
- Request Body:
    - pokemonName (string)
    - pokemonAbility (string)
    - noOfPokemon (number)

Delete Pokémon

- Method: DELETE
- Endpoint: /pokemon/:ownerName
- Description: Deletes a Pokémon from a user's collection

Delete All Pokémon

- Method: DELETE
- Endpoint: /pokemon
- Description: Deletes all Pokémon

Get All Pokémon Owners

- Method: GET
- Endpoint: /pokemon-owners
- Description: Returns a list of all Pokémon owners

Get Pokémon by Owner

- Method: GET
- Endpoint: /pokemon/:ownerName
- Description: Returns a list of Pokémon owned by a specific user

Update Pokémon

- Method: PUT
- Endpoint: /pokemon/:pokemonOwnerName
- Description: Updates a Pokémon's details
- Request Body:
    - pokemonName (string)
    - pokemonAbility (string)
    - noOfPokemon (number)

To use this API, send HTTP requests to the corresponding endpoints with the required request bodies. For example, to add a new Pokémon, send a POST request to /pokemon with the required details in the request body.

Note: Replace /:ownerName and /:pokemonOwnerName with the actual owner name and Pokémon owner name, respectively.

This API is built using Node.js and Express.js. To run the API locally, clone the repository, install dependencies using npm install, and start the server using npm start.