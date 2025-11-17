// Estrutura inicial do projeto Next.js para hospedagem na Vercel // Arquivos essenciais

// package.json { "name": "meu-site-financeiro", "version": "1.0.0", "private": true, "scripts": { "dev": "next dev", "build": "next build", "start": "next start" }, "dependencies": { "next": "14.1.0", "react": "18.2.0", "react-dom": "18.2.0" } }

// next.config.js module.exports = { reactStrictMode: true, };

// /app/layout.js export const metadata = { title: "Guia Financeiro - Organize sua Vida", description: "Aprenda a sair do vermelho, negociar dívidas e economizar.", };

export default function RootLayout({ children }) { return ( <html lang="pt-br"> <body className="bg-gray-100 text-gray-900">{children}</body> </html> ); }

// /app/page.js export default function Home() { return ( <main className="p-6 max-w-3xl mx-auto"> <h1 className="text-4xl font-bold mb-4">Guia Completo de Organização Financeira</h1> <p className="mb-4">Aprenda a sair das dívidas, economizar e construir estabilidade financeira.</p>

<section className="mb-8">
    <h2 className="text-2xl font-semibold mb-2">Como Sair do Vermelho</h2>
    <p>Siga estratégias práticas para recuperar o controle das suas finanças.</p>
  </section>

  <section className="mb-8">
    <h2 className="text-2xl font-semibold mb-2">Como Negociar Dívidas</h2>
    <p>Técnicas eficazes para reduzir juros e parcelar com segurança.</p>
  </section>

  <section className="mb-8">
    <h2 className="text-2xl font-semibold mb-2">Controle de Gastos</h2>
    <p>Aprenda a limitar despesas, criar categorias e organizar seu orçamento.</p>
  </section>

  <section className="">
    <h2 className="text-2xl font-semibold mb-2">Formas de Economizar</h2>
    <p>Dicas reais que funcionam no dia a dia para guardar mais dinheiro.</p>
  </section>
</main>

); }

// /styles/globals.css /* Caso use Tailwind (se quiser adicione depois): @tailwind base; @tailwind components; @tailwind utilities; */

body { font-family: Arial, sans-serif; }
