# Falamigo — novo site

Este projeto reconstrói a página inicial a partir do HTML fornecido, mantendo a nomenclatura e as quatro edições mencionadas no código original, com novo layout responsivo e página de instalação.

## Arquivos
- `index.html`: página inicial
- `baixar.html`: instruções de acesso/instalação PWA
- `privacidade.html`: rascunho de página de privacidade — precisa ser completado e revisado
- `css/style.css`: identidade visual responsiva
- `js/main.js`: menu, ano do rodapé e registro do service worker
- `js/install.js`: botão de instalação quando o navegador oferece suporte
- `manifest.webmanifest`: metadados da aplicação web
- `service-worker.js`: cache básico para recursos do próprio site

## Testar e publicar
1. Extraia o ZIP.
2. Teste localmente com um servidor HTTP (não abrindo o HTML com duplo clique).
3. Faça o deploy da pasta do projeto no Netlify ou conecte-a a um repositório Git.
4. Teste a instalação em Android/Chrome e iPhone/Safari.
5. Revise textos, links, imagens e política de privacidade antes de publicar.

## Pontos importantes antes de colocar em produção
- O mascote e o ícone são referenciados pelo endereço antigo do Falamigo (`falamigo.netlify.app`). Para tornar o novo projeto independente, baixe esses arquivos do site antigo e coloque cópias locais em `assets/`, depois atualize os caminhos no HTML e no manifesto.
- Este projeto é um site/PWA; não é um APK nem um aplicativo publicado nas lojas.
- A instalação PWA depende de HTTPS, suporte do navegador, manifesto válido e ícones adequados. O ícone atual é referenciado externamente e deve ser copiado localmente para a versão final.
- O texto de privacidade é apenas um modelo. Deve refletir as práticas reais de dados do Falamigo.
- O código original menciona recursos de IA, funcionamento offline e funcionalidades específicas. Este site apresenta esses itens como proposta/descrição, não implementa essas funções dentro da página institucional.
- Revise as estatísticas e as fontes citadas no site original antes de reutilizá-las em produção.
