# 🎨 Guia de Uso dos Diagramas DevRel

Este guia explica como usar e personalizar os diagramas visuais do roadmap DevRel.

## 🛠️ Ferramentas Compatíveis com Mermaid

### Plataformas que Renderizam Automaticamente
- ✅ **GitHub** - Renderiza diagramas automaticamente
- ✅ **GitLab** - Suporte nativo ao Mermaid
- ✅ **VS Code** - Com extensão Mermaid Preview
- ✅ **Notion** - Suporte nativo
- ✅ **Obsidian** - Plugin Mermaid

### Ferramentas de Apresentação
- **Marp** - Markdown para slides com Mermaid
- **Reveal.js** - Apresentações web com diagramas
- **GitPitch** - Slides direto do GitHub

### Editores Online
- [Mermaid Live Editor](https://mermaid.live/) - Editor oficial
- [Draw.io](https://app.diagrams.net/) - Importa Mermaid
- [Lucidchart** - Suporte a Mermaid

## 📝 Como Personalizar os Diagramas

### 1. Modificar Cores e Estilos

```mermaid
graph TD
    A[Exemplo] --> B[Personalizado]
    
    %% Definir classes de estilo
    classDef destaque fill:#ff6b6b,stroke:#d63031,stroke-width:3px,color:#fff
    classDef importante fill:#74b9ff,stroke:#0984e3,stroke-width:2px
    classDef opcional fill:#a29bfe,stroke:#6c5ce7,stroke-width:1px
    
    %% Aplicar estilos
    class A destaque
    class B importante
```

### 2. Adaptar para Sua Empresa

```mermaid
graph LR
    DevRel[DevRel Team] --> Product[Product Team]
    DevRel --> Engineering[Engineering]
    DevRel --> Marketing[Marketing]
    
    %% Cores da sua empresa
    classDef empresa fill:#your-primary-color,stroke:#your-secondary-color
    class DevRel empresa
```

### 3. Focar em Roles Específicos

```mermaid
graph TD
    Start[Interesse em DevRel] --> Choice{Qual área mais interessa?}
    
    Choice -->|Gosto de falar| DevAdvocate[🎤 Developer Advocate]
    Choice -->|Gosto de comunidade| Community[👥 Community Manager]
    Choice -->|Gosto de escrever| Writer[📝 Technical Writer]
    
    DevAdvocate --> AdvSkills[Apresentações<br/>Conteúdo técnico<br/>Evangelismo]
    Community --> CommSkills[Engajamento<br/>Eventos<br/>Moderação]
    Writer --> WriteSkills[Documentação<br/>Tutoriais<br/>UX Writing]
```

## 🎯 Templates para Diferentes Usos

### Para Workshops/Treinamentos
```mermaid
journey
    title Workshop DevRel - 4 horas
    section Manhã (2h)
      Apresentação conceitos: 5: Instrutor
      Discussão em grupo: 4: Participantes
      Break: 3: Todos
    section Tarde (2h)
      Hands-on atividade: 5: Participantes
      Apresentação resultados: 4: Participantes
      Q&A e networking: 5: Todos
```

### Para Onboarding
```mermaid
graph TD
    NewHire[🆕 Novo DevRel] --> Week1{Semana 1}
    Week1 --> Shadow[👥 Acompanhar veteranos]
    Week1 --> Learn[📚 Estudar roadmap]
    Week1 --> Meet[🤝 Conhecer teams]
    
    Shadow --> Week2{Semana 2}
    Learn --> Week2
    Meet --> Week2
    
    Week2 --> FirstContent[📝 Primeiro conteúdo]
    Week2 --> FirstEvent[🎪 Primeiro evento]
    
    FirstContent --> Month1[🎯 Avaliação 30 dias]
    FirstEvent --> Month1
```

### Para Métricas
```mermaid
graph LR
    subgraph "📊 Métricas DevRel"
        Awareness[👀 Awareness<br/>Views, Reach]
        Engagement[🤝 Engagement<br/>Comments, Shares]
        Adoption[📈 Adoption<br/>Sign-ups, Usage]
        Retention[🔄 Retention<br/>Return users]
    end
    
    Awareness --> Engagement
    Engagement --> Adoption
    Adoption --> Retention
    Retention -.->|Feedback| Awareness
```

## 🎨 Dicas de Design

### Cores Recomendadas
- **Fundamentos**: Verde claro (`#e8f5e8`)
- **Habilidades**: Azul claro (`#e3f2fd`)
- **Prática**: Laranja claro (`#fff3e0`)
- **Roles**: Roxo claro (`#f3e5f5`)

### Ícones Úteis
- 🚀 Início/Objetivo
- 📚 Aprendizado
- 🛠️ Habilidades
- 🎯 Prática
- 📊 Métricas
- 👥 Comunidade
- 💻 Técnico
- 📝 Conteúdo

## 🔄 Atualizando os Diagramas

1. **Clone o repositório**
2. **Edite os arquivos .md**
3. **Teste no Mermaid Live Editor**
4. **Faça commit das mudanças**
5. **Veja a renderização no GitHub**

---

**💡 Lembre-se**: Os diagramas são ferramentas para facilitar o entendimento. Adapte-os às suas necessidades!
