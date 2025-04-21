<h1> 📚 Resumo das Aprendizagens em Django </h1>
<h2>Fundamentos do Django</h2>

- Projeto vs App: Entendi a diferença entre um projeto Django (estrutura global) e apps (módulos independentes), criando minha primeira app com python manage.py startapp galeria.

- Configuração Inicial: Aprendi a configurar timezone e linguagem no settings.py, além de proteger a SECRET_KEY usando python-dotenv e .env.
  
- Versionamento: Subi o projeto para o GitHub com .gitignore para evitar expor dados sensíveis.
<h2>Estrutura e Organização</h2>

- Templates:
  - Criei um base.html para evitar repetição de código (DRY - Don't Repeat Yourself).
  
  - Organizei templates em pastas específicas para cada app (templates/galeria/).
    
- Partials: Utilizei partials (como _header.html) para reusar componentes (cabeçalho, rodapé) em múltiplas páginas.
  
- Jinja2: Usei templates dinâmicos com sintaxe Jinja2 ({% extends %}, {% block %}) para incorporar lógica Python no HTML.
  
<h2>Rotas e Views</h2>

- URLs:
  - Configurei rotas no urls.py do projeto e da app, seguindo boas práticas de modularização.
    
  - Associei views a URLs para criar páginas personalizadas.
    
- Views: Desenvolvi funções em views.py para renderizar templates e passar dados contextuais.
  
<h2>Arquivos Estáticos (CSS, JS, Imagens)</h2>

- Estrutura:
  - Organizei arquivos estáticos em static/assets/ (imagens), static/styles/ (CSS).
    
  - Aprendi a usar {% static 'caminho' %} para carregar arquivos nos templates.
    
- Collectstatic: Configurei STATICFILES_DIRS e STATIC_ROOT no settings.py para coletar arquivos com python manage.py collectstatic.
  
<h2>Ambiente Virtual e Boas Práticas</h2>

- Virtualenv: Criei ambientes isolados com virtualenv para gerenciar dependências.
  
- Segurança: Protegi chaves sensíveis e usei .env para variáveis de ambiente.
  
- Servidor: Executei o servidor local com python manage.py runserver.
