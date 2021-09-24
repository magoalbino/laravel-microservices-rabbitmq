
## Pode ser útil:

Laravel
- php artisan make:controller nomeController --api (cria a controller já com todos os métodos de apiResourse)
- php artisan make:resource nomeResource 
- - Nesse resource podemos sobrescrever a função toArray() para definir como os dados devem ser retornados, substituindo o retorno dos métodos das controllers pela classe. Ex: "return new UserResource($user)" ou "return new UserResource::collection($user)" para retornar array de vários usuários.
- app/Exceptions/Handler.php -> método Render() (para deixar a resposta da api apenas com o código do erro e a mensagem em json, sem html)
- - return response(['error' => $exception->getMessage()], $exception->getCode() ?: 400);
