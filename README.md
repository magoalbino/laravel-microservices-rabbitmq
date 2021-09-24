
## Pode ser útil:

Laravel
- php artisan make:controller nomeController --api (cria a controller já com todos os métodos de apiResourse)
- php artisan make:resource nomeResource 
- - Nesse resource podemos sobrescrever a função toArray() para definir como os dados devem ser retornados, substituindo o retorno dos métodos das controllers pela classe. Ex: "return new UserResource($user)" ou "return new UserResource::collection($user)" para retornar array de vários usuários.
