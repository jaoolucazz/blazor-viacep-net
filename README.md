# blazor-viacep-net

Aplicação **Blazor WebAssembly (Standalone)** que consulta endereços pela API pública [ViaCEP](https://viacep.com.br).

## Funcionalidades

- Campo para digitar o CEP (aceita com ou sem hífen)
- Validação: CEP vazio e CEP com quantidade de dígitos diferente de 8
- Consulta `https://viacep.com.br/ws/{cep}/json/` via `HttpClient`
- Exibe CEP, logradouro, complemento, bairro, localidade, UF e DDD
- Mensagens de erro para CEP não encontrado e falha de conexão

## Como rodar

```powershell
cd BlazorViaCep
dotnet run
```

Depois acesse a URL exibida no terminal (ex.: `http://localhost:5172`).

## Estrutura

- `BlazorViaCep/Models/Endereco.cs` — modelo que representa o JSON do ViaCEP
- `BlazorViaCep/Pages/Home.razor` — tela e lógica de consulta

## Licença

MIT
