# Snippets Angular Essenciais para TypeScript

![VS Code Marketplace](https://img.shields.io/visual-studio-marketplace/v/{{seu-publisher}}.my-angular-snippets?label=VS%20Code%20Marketplace&color=blue)
![Downloads](https://img.shields.io/visual-studio-marketplace/dt/{{seu-publisher}}.my-angular-snippets?label=Downloads&color=green)
![License](https://img1.shields.io/badge/license-MIT-blue)

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

## 🛠️ Instalação

1.  Abra o Visual Studio Code.
2.  Vá para a guia Extensões (`Ctrl+Shift+X` ou `Cmd+Shift+X`).
3.  Pesquise por "**cp-angular-unit-tests-snippets**".
4.  Clique em **Instalar**.

---

---

## 📄 Licença

Este projeto está licenciado sob a Licença MIT.

---

## 📧 Contato

Se tiver alguma dúvida ou sugestão, entre em contato através do meu GitHub: [enrosales](https://github.com/enrosales)

---