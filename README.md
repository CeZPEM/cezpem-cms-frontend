# CEZPEM - CMS - Frontend

**Centro Zoia Prestes de Educação Multidisciplinar**  

Iniciativa de educação popular do coletivo [@soberana.tv](https://soberana.tv)

## Último estado de deployment

Acesse o último deployment em: [cezpem.netlify.app](https://cezpem.netlify.app)

![Status do Netlify - branch main](https://api.netlify.com/api/v1/badges/43e86ce0-ccff-4e1c-a8e0-413d2a85d2fd/deploy-status/?branch=main)

Confira mais detalhes dos deployments em: [Netlify Deploys](https://app.netlify.com/sites/cezpem/deploys)

## 📌 Sobre o projeto  

Este repositório contém o código-fonte do frontend do site [CeZPEM.com.br](https://cezpem.com.br).  

## 🛠 Desenvolvimento local  

1. Clone este repositório:  
   ```sh
   git clone https://github.com/CeZPEM/cezpem-cms-frontend.git
   cd cezpem-cms-frontend
   ```

2. Instale as dependências:  
   ```sh
   yarn install
   ```

3. Inicie o servidor de desenvolvimento:  
   ```sh
   yarn start
   ```

## 🎨 Layouts  

O template é baseado em pequenos _partials_ independentes do conteúdo, que podem ser combinados de várias formas. As páginas pré-construídas demonstram algumas dessas combinações.  

Para visualizar todos os _partials_ disponíveis, consulte a pasta:  
📂 `site/layouts/partials`  

💡 Utilize a funcionalidade `dict` do Hugo para alimentar os _partials_ com conteúdo, evitando duplicação e inconsistências.

## 🎨 Estilos (CSS)  

O template usa um fork personalizado do **Tachyons** e **PostCSS** com `cssnext` e `cssnano`.  

Para personalizar cores, espaçamentos e outras variáveis globais, edite:  
📄 `src/css/imports/_variables.css`  

## 🖼 Ícones de redes sociais (SVG)  

Os ícones de redes sociais estão localizados em:  
📂 `site/assets/img`  

Para garantir consistência visual, utilize ícones com a mesma proporção de _viewport_ e direção artística.  

Exemplo de uso para um ícone chamado `icons-facebook.svg`:  

```hugo
{{ partial "social-icon" (dict "link" "#" "svg" "icons-facebook" "alt" "Kaldi no Facebook") }}
```

## 🔗 Links úteis  

- **Gerenciador de conteúdo**: [Decap CMS](https://decapcms.org/)  
- **Framework para criar o site**: [Hugo](https://gohugo.io/)  
- **Tarefas e gestão do projeto**: [Jira (CEZPEM)](https://cezpem.atlassian.net/)  
