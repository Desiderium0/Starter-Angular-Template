# Starter Template

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 20.1.3.

To install project dependencies, run the npm i command
```
npm i
```
Then to run the project you will need the command
```
npm run start
```
# Unit testing with Jest

Then run your tests with
```
npm test
```

**Example**
```ts
import { ComponentFixture, TestBed } from '@angular/core/testing';
import { MyComponent } from './my.component';

describe('MyComponent', () => {
  let component: MyComponent;
  let fixture: ComponentFixture<MyComponent>;

  beforeEach(async () => {
    await TestBed.configureTestingModule({
      declarations: [MyComponent],
    }).compileComponents();

    fixture = TestBed.createComponent(MyComponent);
    component = fixture.componentInstance;
    fixture.detectChanges();
  });

  it('should create', () => {
    expect(component).toBeTruthy();
  });

  it('should display title', () => {
    component.title = 'Test Title';
    fixture.detectChanges();
    const element = fixture.nativeElement.querySelector('h1');
    expect(element.textContent).toContain('Test Title');
  });
});
```

# Architecture

```
angular-starter/
├── public/
├── src/
│   ├── app/
│   │   ├── _pages/          # Main application pages
│   │   │   └── ...          # Sub-sections/components (recursive)
│   │   ├── shared/          # Shared modules for app
│   │   │   └── ...          # Structure mirrors root /shared
│   │   └── ...              # Other app folders
│   ├── shared/              # Global shared modules
│   │   ├── api/             # API clients and configurations
│   │   ├── components/      # Shared components
│   │   ├── constants/       # Application constants
│   │   ├── directives/      # Directives
│   │   ├── enums/           # Enumerations
│   │   ├── guards/          # Route guards
│   │   ├── interceptors/    # HTTP interceptors
│   │   ├── layouts/         # Page layouts
│   │   ├── pipes/           # Pipes
│   │   ├── providers/       # Providers
│   │   ├── services/        # Services
│   │   ├── storages/        # Storage management
│   │   ├── styles/          # Global styles
│   │   ├── types/           # Types and interfaces
│   │   ├── utils/           # Utility functions
│   │   └── validators/      # Form validators
│   ├── assets/              # Static assets
│   └── environments/        # Environment configurations
└── ...                     # Other project root folders
```

# Dependencies
The project has installed:
- **Taiga UI**
<img width="250" height="400" alt="Taiga UI" src="https://github.com/user-attachments/assets/c24c1c84-9253-4569-ad6d-28f269eb399e" />

<br>

- **Jest (Unit Testing)**
<img width="250" height="400" alt="Jest" src="https://github.com/user-attachments/assets/0a2138c5-1b2a-472c-8c32-196923dca2d1" />


