## Biblioteca para fornecer componentes (botões, toolbar, etc)

1. Instale o Angular Material no terminal do vscode:
   npx ng add @angular/material

### Criação de componente

Em seguida crie um componente header usando o comando:

- npx ng g c shared/components/header

g = global
c = component
shared/components/header = caminho das pastas e arquivo.

### Importando o componente

Dentro do @component, na propriedade imports do arquivo app.component.ts vincule o header que foi criado.

```
@Component({
  selector: 'app-root',
  standalone: true,
  // importando HeaderComponent
  imports: [RouterOutlet, HeaderComponent],
  templateUrl: './app.component.html',
  styleUrl: './app.component.scss'
})
```

No app.component.html chame o header (igual a um componente em React).

<app-header></app-header>

### Dica de extensão

Para uma experiência melhor com o Angular, instale a extensão "Angular Language Service"
