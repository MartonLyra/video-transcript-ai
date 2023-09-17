## Projeto Rocketseat - Video Transcript usando IA
by [Marton Lyra](https://github.com/MartonLyra/video-transcript-ai)

Instrutor: [Diego Fernandes](https://blog.rocketseat.com.br/author/diego/)

Projeto criado do zero por Marton Lyra em Setembro de 2023, seguindo instruções do instrutor.


Objetivo: receber um vídeo do usuário via upload e, usando inteligência artificial, faremos um transcript do audio para texto seguido de solicitações à IA como, por exemplo, solicitar sugestões de títulos e descrições para o vídeo.


## Aula 01 - Desenvolvendo o Front-End

#### Configurando o ambiente e estrutura do projeto

- [13m00s] O primeiro passo foi gerar o projeto usando o [ViteJs](https://vitejs.dev/), uma ferramenta para gerar a estrutura inicial de vários tipos de projetos. Para isso, usei o template **React** e **TypeScript** como linguagem principal.
- [14m45s] Uma vez criado a estrutura, baixei as dependências usando o pnpm, excluí alguns arquivos desnecessários e configurei outros.
- [17m50s] Vamos usar os componentes do [RadixUI](https://www.radix-ui.com/RadixUI), que são vários componentes prontos, funcionais, porém sem estilo.
- [17m00s] Estaremos usando o [Tailwind CSS](https://tailwindcss.com/), uma biblioteca onde descrevemos componentes diretamente no class do HTML. Apesar dele deixar o HTML um pouco mais poluído, isso não chega a ser problema já que o React é bem dividido em componentes.
- [19m40s] Também vamos usar o [shadcn/ui](https://ui.shadcn.com/), uma biblioteca com vários componentes implementados usando themas. O [shadcn/ui](https://ui.shadcn.com/) é perfeito para agrupar as funcionalidades do [RadixUI](https://www.radix-ui.com/RadixUI) com o [Tailwind CSS](https://tailwindcss.com/). O [shadcn/ui](https://ui.shadcn.com/) possui todos os componentes do [RadixUI](https://www.radix-ui.com/RadixUI) e mais alguns, estilizados, usando um Style Guide, ou seja, um padrão entre eles. Excelente para buscar produtividade, principalmente se você não precisa se preocupar muito em personalizar o front, de forma exclusiva. Se sua aplicação precisa de um design bem específico, então esquece o shadcn/ui, que trás uma estilização própria, coda a aplicação usando o RadixUI e o Tailwind CSS.

- [20m40s] Quando instalamos o [shadcn/ui](https://ui.shadcn.com/), ele automaticamente já isntala o [RadixUI](https://www.radix-ui.com/RadixUI) e o [Tailwind CSS](https://tailwindcss.com/). Portanto, basta se preocupar em instalar o [shadcn/ui](https://ui.shadcn.com/).

- [21m00s] Para instalar o [shadcn/ui](https://ui.shadcn.com/), basta ir na [página de instalação](https://ui.shadcn.com/docs/installation) e, como estamos usando o [ViteJs](https://vitejs.dev/), clicar no ícone do Vite.

- [30m40s] Usei o VSCode com as seguintes extensões para desenvolver: [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker), [Prisma](https://marketplace.visualstudio.com/items?itemName=Prisma.prisma), [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss), [PostCSS Language Support](https://marketplace.visualstudio.com/items?itemName=csstools.postcss).

- [31m30s] Por padrão, o [shadcn/ui](https://ui.shadcn.com/) tem um <code>tema light</code>. Para mudar para o Dark, navegue até o site do [shadcn/ui](https://ui.shadcn.com/) e clique em [Themes](https://ui.shadcn.com/themes) e, no botão <code>Customize</code>, customizei diferente do instrutor, escolhendo o estilo (New York), cor (Verde), Mode (Dark), dentre outros. [32m30s] Uma vez personalizado, clique em <code>Copy code</code>, selecione o conteúdo da tag <code>.dark</code>, abre o arquivo no projeto [index.css](https://github.com/MartonLyra/video-transcript-ai/blob/main/src/index.css), e cole tudo dentro da tag :root, sem apagar a última linha <code>--radius</code>. Também pode excluir toda a tag <code>.dark</code>.


#### Agora vamos começar a construir a interface do projeto

- [33m30s] O arquivo [src/App.tsx](https://github.com/MartonLyra/video-transcript-ai/blob/main/src/App.tsx) é o arquivo principal do React. Aqui podemos escrever HTML, CSS, JavaScript, tudo junto, que é o grande poder do React.

- [34m30] O [shadcn/ui](https://ui.shadcn.com/) trás os componentes mais específicos como botões, select. Mas, por exemplo, um cabeçalho, nós temos que criar.

- [37m40s] Quando você define a cor de um texto ou objeto, você poderia, usando o <code>Tailwind CSS</code>, colocar a dor diretamente (exemplo: <code>text-zinc-400</code>). Porém, como estamos usando o shadcn-ui, ele tráz umas cores meio que padrão, para você utilizar de forma fácil em várias partes do projeto. Por exemplo: <code>text-muted-foregrount<c/ode> que é um texto discreto, sem muito destaque. A vantagem de usar os nomes do shadcn-ui é que, se um dia, você quiser colocar um thema de outra cor, dessa forma fica mais fácil de alterar.

- [39m20s] Vamos configurar o primeiro componente do shadcn-ui, o Button.

- [40m05s] 





Acabei de instalar o shadcn.
Continuar a aula 1 em 30m30s.