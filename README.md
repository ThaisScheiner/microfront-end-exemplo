# Angular - Microfrontends com Module Federation do Webpack

Os **microfrontends** aplicam os princípios dos **microservices** ao frontend.  
Em vez de ter um único projeto monolítico, a interface da aplicação é dividida em partes menores (**módulos remotos**), carregados dinamicamente em um **host** (shell principal).

O **Module Federation**, introduzido no **Webpack 5**, permite que diferentes aplicações compartilhem código e carreguem módulos remotamente em tempo de execução, sem necessidade de recompilação total.  

Assim, cada parte do frontend pode ser:  
- Desenvolvida e implantada separadamente  
- Compartilhada sem redundâncias  
- Carregada dinamicamente conforme necessário  

## Exemplo prático  

Neste exemplo:  
- A **página Home** atua como o **host**  
- Os links **Dashboard Barra** e **Dashboard Pizza** são aplicações independentes  

### URLs das aplicações  
- **Host:** [http://localhost:4200/](http://localhost:4200/)  
- **Dashboard Barra:** [http://localhost:4201](http://localhost:4201)  
- **Dashboard Pizza:** [http://localhost:4202](http://localhost:4202)  

### Como inicializar  
Para rodar cada aplicação, utilize o comando:  
```sh
ng start


