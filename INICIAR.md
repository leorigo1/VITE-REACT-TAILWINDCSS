Etapas de Instalação

1. Criar o projeto com Vite + React + TypeScript
npm create vite@latest nome-do-projeto -- --template react-ts
cd nome-do-projeto

Selecione React e Typescript.


2. Instalar dependências
npm install


Instalar e configurar o Tailwind CSS3. 

3. Instalar Tailwind e dependências
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p


4. Configurar o arquivo tailwind.config.js
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}


5. Importar Tailwind no CSS

No arquivo src/index.css, adicione:
@tailwind base;
@tailwind components;
@tailwind utilities;


6. Instalar o shadcn-ui CLI
npx shadcn-ui@latest init

Framework: selecione React
TypeScript?: Yes
Tailwind CSS?: Yes
Directory for components: components (padrão)
Alias para importações: por exemplo, @/components


Usar um componente do shadcn-ui
7. Instalar um componente
Exemplo para instalar um botão:
npx shadcn-ui@latest add button
Isso adicionará o componente em src/components/ui/button.tsx.


8. Usar no seu app
// App.tsx
import { Button } from "@/components/ui/button"

function App() {
  return (
    <div className="p-6">
      <Button variant="default">Clique aqui</Button>
    </div>
  )
}

export default App


9. Rodar o projeto
    npm run dev



 

