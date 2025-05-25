# Snippets Angular Essenciais para TypeScript

![VS Code Marketplace](https://img.shields.io/visual-studio-marketplace/v/enrosales.cp-angular-unit-tests-snippets?label=VS%20Code%20Marketplace&color=blue)
![Downloads](https://img.shields.io/visual-studio-marketplace/dt/enrosales.cp-angular-unit-tests-snippets?label=Downloads&color=green)
![License](https://img.shields.io/badge/license-MIT-blue)

---

## 🚀 Visão Geral

Eleve sua produtividade no desenvolvimento Angular! Esta extensão oferece uma coleção de **snippets TypeScript** cuidadosamente elaborados para o Visual Studio Code, focados em agilizar a criação de estruturas de código comuns no ecossistema Angular.

Diga adeus à repetição e insira instantaneamente blocos de código complexos, como estruturas de testes para componentes e diretivas, importações essenciais e outros padrões comuns. **Ganhe velocidade e consistência** em seus projetos, permitindo que você se concentre na lógica principal da sua aplicação.

---

## ✨ Funcionalidades Principais

* **Snippets Otimizados:** Um conjunto crescente de atalhos para os padrões de código Angular mais utilizados em TypeScript.
* **Produtividade Acelerada:** Insira rapidamente estruturas complexas, economizando tempo e minimizando erros de digitação.
* **Foco em Testes:** Snippets dedicados para a criação de testes de unidades para componentes e diretivas (como `testDirective`, `testComponent`).
* **Compatibilidade:** Projetado para funcionar perfeitamente com projetos Angular em TypeScript.

---

## 💡 Como Usar

1.  Instale a extensão diretamente pelo [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName={{seu-publisher}}.my-angular-snippets).
2.  Em qualquer arquivo `.ts` (TypeScript) no seu projeto Angular, comece a digitar o prefixo do snippet desejado.
3.  Selecione o snippet na lista de sugestões de autocompletar e pressione `Enter` ou `Tab`.
4.  Utilize a tecla `Tab` para navegar entre os campos de preenchimento (`$1`, `$2`, etc.) do snippet.

### Snippets Atualmente Disponíveis:

* **`testDirective`**: Gera uma estrutura básica de teste para uma diretiva ou componente Angular.
    * **Prefixo:** `testDirective`
    * **Corpo do Snippet:**
        ```typescript
        import { Component } from '@angular/core';
        import { TestBed, ComponentFixture } from '@angular/core/testing';

        describe('${1:MyDirective}', () => {
          let fixture: ComponentFixture<${2:MyDirectiveComponent}>;
          let component: ${2:MyDirectiveComponent};

          beforeEach(async () => {
            await TestBed.configureTestingModule({
              declarations: [${2:MyDirectiveComponent}],
              // imports: [ ... ],
              // providers: [ ... ]
            }).compileComponents();
          });

          beforeEach(() => {
            fixture = TestBed.createComponent(${2:MyDirectiveComponent});
            component = fixture.componentInstance;
            fixture.detectChanges();
          });

          it('should create', () => {
            expect(component).toBeTruthy();
          });
        });
        ```

---

## 📋 Lista de Snippets Disponíveis

| Nº  | Prefixo                     | Descrição                                                        |
|-----|-----------------------------|------------------------------------------------------------------|
| 1   | `testComponent`             | Gera um teste básico para um componente Angular                  |
| 2   | `testService`               | Gera um teste básico para um serviço Angular                     |
| 3   | `testPipe`                  | Gera um teste básico para um pipe Angular                        |
| 4   | `testDirective`             | Gera um teste básico para uma diretiva Angular                   |
| 5   | `testGuard`                 | Gera um teste básico para um guard Angular                       |
| 6   | `testResolver`              | Gera um teste básico para um resolver Angular                    |
| 7   | `testModule`                | Gera um teste básico para um módulo Angular                      |
| 8   | `testInterface`             | Gera um teste básico para uma interface Angular                  |
| 9   | `testEnum`                  | Gera um teste básico para um enum Angular                        |
| 10  | `testComponentMockService`  | Teste de componente Angular com serviço mockado                  |
| 11  | `testServiceMockHttp`       | Teste de serviço Angular com HTTP mockado                        |
| 12  | `testComponentMockRouter`   | Teste de componente Angular com router mockado                   |
| 13  | `testReactiveForm`          | Teste para um componente com formulário reativo                  |
| 14  | `testTemplateDrivenForm`    | Teste para um componente com formulário template-driven          |
| 15  | `testComponentRouter`       | Teste de componente Angular com Router                           |
| 16  | `testStructuralDirective`   | Teste para uma diretiva estrutural Angular                       |
| 17  | `testAttributeDirective`    | Teste para uma diretiva de atributo Angular                      |

Cada snippet inclui placeholders para facilitar a edição rápida de nomes e estruturas.

---

## 🛠️ Instalação

1.  Abra o Visual Studio Code.
2.  Vá para a guia Extensões (`Ctrl+Shift+X` ou `Cmd+Shift+X`).
3.  Pesquise por "**cp-angular-unit-tests-snippets**".
4.  Clique em **Instalar**.

---

## 📄 Licença

Este projeto está licenciado sob a Licença MIT.

---

## 📧 Contato

Se tiver alguma dúvida ou sugestão, entre em contato através do meu GitHub: [enrosales](https://github.com/enrosales)

---