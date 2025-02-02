# CEZPEM - CMS - Frontend


[![Netlify Status - dev](https://api.netlify.com/api/v1/badges/43e86ce0-ccff-4e1c-a8e0-413d2a85d2fd/deploy-status/?branch=main)](https://app.netlify.com/sites/devcezpem/deploys)

[![Netlify Status - main](https://api.netlify.com/api/v1/badges/43e86ce0-ccff-4e1c-a8e0-413d2a85d2fd/deploy-status/?branch=dev)](https://app.netlify.com/sites/devcezpem/deploys)

**Centro Zoia Prestes de Educação Multidisciplinar**  
Frente de massas de educação do coletivo [@soberana.tv](https://soberana.tv).

## Sobre o projeto
Este repositório contém o código-fonte do frontend do [CeZPEM.com.br](https://cezpem.com.br).

## Links
- Gerenciador de conteudo: https://decapcms.org/
- Framework para criar o site: https://gohugo.io/
- Tarefas: https://cezpem.atlassian.net/

## Contribuindo
1. Certifique-se de ter permissão para criar branches neste repositório.  
2. Crie uma branch para sua funcionalidade ou correção: `git checkout -b minha-nova-funcionalidade`.  
3. Realize as alterações necessárias no código.  
4. Envie suas alterações para o repositório remoto: `git push origin minha-nova-funcionalidade`.  
5. Abra um pull request para revisão e aprovação.

# Hugo template for Decap CMS with Netlify Identity

This is a small business template built with [Hugo](https://gohugo.io) and [Decap CMS](https://github.com/decaporg/decap-cms), designed and developed by [Darin Dimitroff](https://twitter.com/deezel), [spacefarm.digital](https://www.spacefarm.digital).

## Getting started

Use our deploy button to get your own copy of the repository. 

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/decaporg/one-click-hugo-cms&stack=cms)

This will setup everything needed for running the CMS:

* A new repository in your GitHub account with the code
* Full Continuous Deployment to Netlify's global CDN network
* Control users and access with Netlify Identity
* Manage content with Decap CMS

Once the initial build finishes, you can invite yourself as a user. Go to the Identity tab in your new site, click "Invite" and send yourself an invite.

Now you're all set, and you can start editing content!

## Local Development

Clone this repository, and run `yarn` or `npm install` from the new folder to install all required dependencies.

Then start the development server with `yarn start` or `npm start`.

## Layouts

The template is based on small, content-agnostic partials that can be mixed and matched. The pre-built pages showcase just a few of the possible combinations. Refer to the `site/layouts/partials` folder for all available partials.

Use Hugo’s `dict` functionality to feed content into partials and avoid repeating yourself and creating discrepancies.

## CSS

The template uses a custom fork of Tachyons and PostCSS with cssnext and cssnano. To customize the template for your brand, refer to `src/css/imports/_variables.css` where most of the important global variables like colors and spacing are stored.

## SVG Social Icons

The social media icons are in `site/assets/img`.
Make sure you use consistent icons in terms of viewport and art direction for optimal results.
For an icon named `icons-facebook.svg`, refer to the SVG `social-icon` partial like so:

```
{{ partial "social-icon" (dict "link" "#" "svg" "icons-facebook" "alt" "Kaldi on Facebook") }}
```
