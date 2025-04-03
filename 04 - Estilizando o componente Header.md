Importe o material toolbar dentro do arquivo header.component.ts

```
import { Component } from '@angular/core';
import {MatToolbarModule} from '@angular/material/toolbar';

@Component({
  selector: 'app-header',
  standalone: true,
  // Importando toolbar do material
  imports: [MatToolbarModule],
  templateUrl: './header.component.html',
  styleUrl: './header.component.scss'
})
```

Agora no arquivo header.component.html chame o componente mat-toolbar

<mat-toolbar>
  <p>header works!</p>
</mat-toolbar>
